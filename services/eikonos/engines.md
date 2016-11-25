There are many different engines that support Danbooru style websites, but only a few of them are really suitable for large sites.

* **MoeBooru** (Current Pick) - Used by yande.re, and maintained in production. It is a full featured fork of Danbooru in Ruby with all the bells and whistles. Requires PostgreSQL.
  * https://github.com/moebooru/moebooru
* [Danbooru](https://github.com/r888888888/danbooru/releases) - The original. Still seeing heavily daily development to this day. Not sure whether it is better than Moebooru,
  * [It can be sort of deployed to docker.](https://github.com/r888888888/danbooru/issues/2139)
* [Shimmie2](https://github.com/shish/shimmie2) - PHP and MySQL version, which is easier to set up, but has fewer features.
* **Gelbooru** 0.3 (Future) - If the devs ever get enough funding to get their shit together, they will open source their new and improved Gelbooru engine. That would be awesome to use. Uses Python and is solid stuff.
* Gelbooru 0.2.x - [Safebooru](http://safebooru.org/index.php?page=post&s=list) uses this version, which runs on PHP.
* **MyImouto** - Port of Moebooru to PHP.
  * https://github.com/myimouto/myimouto

## Development

Stuff that needs heavy modification to make it work for us.

* [Flaskbooru](https://github.com/razage/flaskbooru) - A proof of concept python Flask based engine to use as a basis. Has sqlalchemy too, so it's portable. This is also easy to build a REST API with Eve.
  * https://github.com/humiaozuzu/awesome-flask
  * Know how to deploy a WSGI app. Tornado is good. http://flask.pocoo.org/docs/0.10/deploying/
* [Eve API](http://stackoverflow.com/questions/24134383/servicing-html-requests-with-eve) - Alternatively, we could use Eve docs to build an HTML template system that is on top of the API, rather than the other way around. Maybe we should keep the logic separate though, they are different.
* [CookieCutter Flask](https://github.com/sloria/cookiecutter-flask) - Signfiicantly more integrated with SQLAlchemy and Twitter-Bootstrap. You do the same thing over and over anyway, use known good methods.
  * [CookieCutter FlaskRESTFul](https://github.com/sendgridlabs/cookiecutter-flaskrestful)
* [Enferno](http://enferno.io/) - Quick and easy forms, administration, accounts, and auths on top of Flask.
  * It's dead simple: https://medium.com/project-enferno/moonwalking-with-project-enferno-402937628745
* [Quokka CMS](https://github.com/quokkaproject/quokka) - A full CMS based on Flask and MongoDB. Seems like a CMS is overkill for what I do.

## Database Considerations

* PostgreSQL - High performance open source SQL server with REST API and NoSQL-style features. Even beats MongoDB.
* MariaDB/MySQL - A popular choice for compatibility reasons with Websites. But not all that great.
* MongoDB - NoSQL database, the first and with all it's NoSQL features.

## Moving to Gelbooru 0.3.x in the Future

The Gelbooru engine is based on PHP, and is currently being funded for full time development. 0.3.x will be open source one day in the future. Unfortunately, that day isn't today, but it would be cool to check it out.

Slayerduck2 states that Konachan, which has only 20% of the images of Gelbooru, uses the same amount of CPU power. 

That shows just how resource intensive Ruby is due to Moebooru.

