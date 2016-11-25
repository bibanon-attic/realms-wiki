Setting Up Moebooru
===================

Get configuration tips from here:

http://wiki.douglasqsantos.com.br/doku.php/deploying_a_rails_app_on_debian_jessie_with_capistrano_nginx_and_puma_en

## Create Moebooru User

https://github.com/moebooru/moebooru

Create a specific non-login daemon user just for moebooru (Though it will have bash shell for setup purposes temporarily). Then create a systemd service for it.

```
sudo git clone https://github.com/moebooru/moebooru.git /var/www/booru.eikonos.org
sudo useradd -s /bin/bash -d /var/www/booru.eikonos.org -r moebooru
sudo chown -R moebooru:moebooru /var/www/booru.eikonos.org
```

## Setup Postgresql

```
sudo rpm -ivh http://yum.postgresql.org/9.5/redhat/rhel-7-x86_64/pgdg-centos95-9.5-2.noarch.rpm
sudo yum install postgresql95 postgresql95-devel libpqxx libpqxx-devel
```

`libpqxx` is required for libpq-ruby to build.

Now log in and create the moebooru user:

```
# su - postgres
$ psql
postgres# create user moebooru_user with password 'the_password' createdb;
```

Finally, edit `/var/lib/pgsql/9.5/data/pg_hba.conf` from `ident` to `md5` (except for the UNIX socket line) to allow users to log in using a password (required by moebooru's config):

https://gist.github.com/groveriffic/4122225

> **Advisory:** If this postgresql server is on the same machine, make sure the firewall is configured to prevent remote access to postgresql ports. Also ensure that SSH keys are used instead of passwords. If this postgresql server is on another machine in the network/internet, make sure moebooru is connecting via SSL.

## Install Nodejs

NodeJS is necessary for the frontend. You should obtain the latest version, 6.x:

Run this script as root:

```
curl --silent --location https://rpm.nodesource.com/setup_6.x | bash -
```

https://nodejs.org/en/download/package-manager/

## Setup Rubinius

Currently, just running normal ruby MRI should be sufficient for most tasks, but Rubinius can add significant performance boosts.

First, if you have normal ruby MRI currently installed, you should uninstall it.

Add the Zonio repository to `/etc/yum.repos.d/zonio.repo` to add Rubinius:

```
[zonio]
name=Zonio $releasever - $basearch
baseurl=https://zonio.net/repos/epel/$releasever/$basearch
enabled=1
gpgcheck=1
gpgkey=https://zonio.net/repos/GPG-Key-Zonio
priority=5
```

Then, just install rubinius, and verify that:

```
sudo yum install rubinius rubinius-devel
ruby -v
```

Notice that you should not install normal ruby MRI afterwards. If you have a good reason to, follow these instructions:

https://zonio.net/rubinius_rpm_packages/

## SELinux Permissions

If using SELinux (which we highly recommend), you will need the following policies

needed for proxy pass

```
sudo chcon -Rt httpd_sys_content_t /var/www/ # allow nginx to access folders
sudo setsebool httpd_can_network_connect 1 -P # allows reverse proxy
sudo setsebool -P httpd_can_network_memcache 1 # allows memcache
```

needed to serve from moebooru user's directory, but only `shared/` and `public` folders

```
setsebool -P httpd_enable_homedirs 1
sudo semanage fcontext -a -t httpd_sys_content_t '/var/www/booru.eikonos.org/shared(/.*)?'
sudo restorecon -R -v /var/www/booru.eikonos.org/shared
sudo semanage fcontext -a -t httpd_sys_content_t '/var/www/booru.eikonos.org/public(/.*)?'
sudo restorecon -R -v /var/www/booru.eikonos.org/public
```

https://www.pckr.co.uk/selinux-nginx-and-reverse-proxying-2/

https://www.digitalocean.com/community/tutorials/an-introduction-to-selinux-on-centos-7-part-2-files-and-processes

The last step is to run the final allows.

```
sudo grep nginx /var/log/audit/audit.log | audit2allow -M nginx > nginx.te
```

View this and see that it is correct (such that no suspicious rule allows are inside). Then run:

```
sudo grep nginx /var/log/audit/audit.log | audit2allow -M nginx 
sudo semodule -i nginx.pp
```

http://axilleas.me/en/blog/2013/selinux-policy-for-nginx-and-gitlab-unix-socket-in-fedora-19/

## Setup Moebooru

Now, conduct the setup and get dependencies.

```
sudo yum install gcc gcc-c++ ImageMagick jhead libxslt-devel git libyaml-devel openssl-devel pcre-devel readline-devel
```

First, [do a bundle config for pg](http://stackoverflow.com/a/9235107) since we're using a specific postgresql version:

```
bundle config build.pg --with-pg-config=/usr/pgsql-9.5/bin/pg_config
```

Install the ruby packages for the moebooru user only (under the directory `./vendor/bundle`):

```
bundle install --path vendor/bundle
```

Create `config/database.yml` and `config/local_config.rb` from the `.example` files, and configure them accordingly. Then set `chmod 700` so only the moebooru user can read the database password.

```
chmod 600 /var/www/booru.eikonos.org/config/database.yml
```

Initialize database `with bundle exec rake db:reset` (there will be some errors reported which is expected)

Run `bundle exec rake db:migrate`

Now, you need to provide the correct permissions to the public folder:

```
chmod 755 /var/www/booru.eikonos.org/public
```

Start the server (`bundle exec unicorn` or `bundle exec puma` if using JRuby/Rubinius)

Finally, set moebooru to a non login user:

```
sudo chsh -s /bin/false moebooru
```

## Customize Header Image and Branding

By default, Moebooru comes with the Yande.re header image and branding, as the site developed the moebooru engine. You should definitely consider removing the original branding unless your site is private.

app/assets/images

public/favicon.ico

## Enable Memcached

Follow these instructions to install Memcached. You need at least 2GB free RAM to provide.

sudo yum install memcached

http://www.liquidweb.com/kb/how-to-install-memcached-on-centos-7/

Edit `/etc/sysconfig/memcached` and set `CACHESIZE=2048` (2GB RAM) if possible.

Then activate it by appending a bash variable to the puma command: `MB_MEMCACHE_SERVERS="<url-to-memcached>"` . Here are some examples.

TCP: `MB_MEMCACHED_SERVERS='127.0.0.1:11211' RAILS_ENV=production bundle exec puma -e production`

UNIX Socket: `MB_MEMCACHED_SERVERS='127.0.0.1:11211' RAILS_ENV=production bundle exec puma -C shared/puma.rb`

### SELinux Permissions

You will probably need to allow it through SELinux:

https://major.io/2011/09/07/getting-apache-php-and-memcached-working-with-selinux/

## Production Mode

By default, Moebooru runs in development mode, which can be slow. Here are the steps to set up Production mode.

### Preparation

First, you need to create the database, and pregenerate the javascript/css (do this every time you update):

```
RAILS_ENV=production bundle exec rake db:reset
RAILS_ENV=production bundle exec rake assets:precompile
```

Then, you need to provide the correct permissions to the public folder:

```
chmod 755 /var/www/booru.eikonos.org/public
```

### Serve static files with Nginx

Create an Nginx config under `/etc/nginx/conf.d/`. Make sure to change the `server_name`, and the `root /var/www/booru.eikonos.org/public` to `root /YOUR/MOEBOORU/PATH/public`.

> **Note:** If you are using a different port for puma, (by adding `-p 3000` to the serving command), also change the port accordingly below.

```
server {
    listen 80;
    server_name booru.eikonos.org;
    
    # directory of static assets, first generate with the command:
    # RAILS_ENV=production bundle exec rake assets:precompile
    root /var/www/booru.eikonos.org/public;

    try_files $uri/index.html $uri @app;

    location @app {
      proxy_set_header Host $host;
      proxy_set_header X-Real-IP $remote_addr;
      proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
      proxy_set_header X-Forwarded-Proto $scheme;
      # Fix the "It appears that your reverse proxy set up is broken" error.
      proxy_pass http://127.0.0.1:9292;
      proxy_read_timeout 90;
      proxy_redirect http://127.0.0.1:9292 http://$server_name;
    }
    
    error_page 500 502 503 504 /500.html;
    client_max_body_size 4G;
    keepalive_timeout 10;
}
```

### Run the Server

Finally, to run the server (default is port 9292), run the following command:

```
RAILS_ENV=production bundle exec puma -e production
```

* [Source: StackOverflow - Rails 4: assets not loading in production](http://stackoverflow.com/a/27318704)

## Serve with UNIX Socks in Production Mode

for even more effectiveness, use a UNIX sock: https://www.digitalocean.com/community/tutorials/how-to-deploy-a-rails-app-with-puma-and-nginx-on-ubuntu-14-04

Figure out the amount of CPU cores you have:

```
grep -c processor /proc/cpuinfo
```

Create the following folders in your application directory:

```
mkdir -p shared/pids shared/sockets shared/log
```

Place the following into `<app_dir>/shared/puma.rb`:

```
# Change to match your CPU core count
workers 8

# Min and Max threads per worker
threads 1, 6

app_dir = File.expand_path("../..", __FILE__)
shared_dir = "#{app_dir}/shared"

# Default to production
rails_env = ENV['RAILS_ENV'] || "production"
environment rails_env

# Set up socket location
bind "unix://#{shared_dir}/sockets/puma.sock"

# Logging
stdout_redirect "#{shared_dir}/log/puma.stdout.log", "#{shared_dir}/log/puma.stderr.log", true

# Set master PID and state locations
pidfile "#{shared_dir}/pids/puma.pid"
state_path "#{shared_dir}/pids/puma.state"
activate_control_app

on_worker_boot do
  require "active_record"
  ActiveRecord::Base.connection.disconnect! rescue ActiveRecord::ConnectionNotEstablished
  ActiveRecord::Base.establish_connection(YAML.load_file("#{app_dir}/config/database.yml")[rails_env])
end
```

Change the Nginx server config to the following:

```
upstream app {
    # Path to Puma SOCK file, as defined previously
    server unix:/var/www/booru.eikonos.org/shared/sockets/puma.sock fail_timeout=0;
}

server {
    listen 80;
    server_name booru.eikonos.org;
    
    # directory of static assets, first generate with the command:
    # RAILS_ENV=production bundle exec rake assets:precompile
    root /var/www/booru.eikonos.org/public;

    try_files $uri/index.html $uri @app;

    location @app {
      proxy_set_header Host $host;
      proxy_set_header X-Real-IP $remote_addr;
      proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
      proxy_set_header X-Forwarded-Proto $scheme;
      # Fix the "It appears that your reverse proxy set up is broken" error.
      proxy_pass http://app;
      proxy_read_timeout 90;
      proxy_redirect http://app http://$server_name;
    }
    
    error_page 500 502 503 504 /500.html;
    client_max_body_size 4G;
    keepalive_timeout 10;
}
```

Finally, to run the server, use the following:

```
bundle exec puma -C shared/puma.rb
```

## Systemd Service

https://github.com/puma/puma/blob/master/docs/systemd.md

Save this to `/usr/systemd/system/moebooru.service`. There are two versions, one for TCP and one for unix socket. Change the WorkingDirectory accordingly.

### TCP

```
[Unit]
Description=Moebooru's Puma HTTP Server
Requires=redis.service postgresql-9.5.service
Wants=postgresql-9.5.service memcached.service
After=network.target postgresql-9.5.service

# Uncomment for socket activation (see below)
# Requires=puma.socket

[Service]
# Foreground process (do not use --daemon in ExecStart or config.rb)
Type=simple

# Preferably configure a non-privileged user
User=moebooru

# Specify the path to your puma application root
WorkingDirectory=/var/www/booru.eikonos.org

# Helpful for debugging socket activation, etc.
# Environment=PUMA_DEBUG=1

# The command to start Puma
# Here we are using a binstub generated via:
# `bundle binstubs puma --path ./sbin`
# in the WorkingDirectory (replace <WD> below)
# You can alternatively use `bundle exec --keep-file-descriptors puma`
# ExecStart=<WD>/sbin/puma -b tcp://0.0.0.0:9292 -b ssl://0.0.0.0:9293?key=key.pem&cert=cert.pem

# Alternatively with a config file (in WorkingDirectory) and
# comparable `bind` directives
ExecStart=/bin/bash -c 'RAILS_ENV=production /usr/bin/bundle exec puma -e production'

Restart=always

[Install]
WantedBy=multi-user.target
```

### UNIX Socket

Two Systemd services are needed: one for the socket and one for the application. 

`/usr/systemd/system/moebooru.service`

```
[Unit]
Description=Puma HTTP Server
Requires=redis.service postgresql-9.5.service
Wants=postgresql-9.5.service memcached.service
After=network.target postgresql-9.5.service

# Uncomment for socket activation (see below)
# Requires=puma.socket

[Service]
# Foreground process (do not use --daemon in ExecStart or config.rb)
Type=simple

# Preferably configure a non-privileged user
# User=

# Specify the path to your puma application root
# WorkingDirectory=

# Helpful for debugging socket activation, etc.
# Environment=PUMA_DEBUG=1

# The command to start Puma
# Here we are using a binstub generated via:
# `bundle binstubs puma --path ./sbin`
# in the WorkingDirectory (replace <WD> below)
# You can alternatively use `bundle exec --keep-file-descriptors puma`
# ExecStart=<WD>/sbin/puma -b tcp://0.0.0.0:9292 -b ssl://0.0.0.0:9293?key=key.pem&cert=cert.pem

# Alternatively with a config file (in WorkingDirectory) and
# comparable `bind` directives
# ExecStart=<WD>/sbin/puma -C config.rb

Restart=always

[Install]
WantedBy=multi-user.target
```

Grab some code from here?

https://github.com/puma/puma/issues/976

## SSL Certificates

While this is beyond the scope of this guide, you should strongly consider using SSL certificates, which are now free with Let's Encrypt.

https://www.digitalocean.com/community/tutorials/how-to-secure-nginx-with-let-s-encrypt-on-centos-7