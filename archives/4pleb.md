> ### Note:
this is an updated miror of the [ArchiveTeam wiki's 4chan  4pleb page](http://www.archiveteam.org/index.php?title=4chan/4plebs)

{{Infobox project
| title = archive.4plebs.org
| image = archive-4plebs.png
| URL = [http://archive.4plebs.org archive.4plebs.org]
| project_status = {{online}}
| archiving_status = {{saved}}
}}

Status: <span style="color: green;">'''Online'''</span>
Saves Images?: <span style="color: green;">'''Yes'''</span>

4plebs is shedding all full-sized images dating before April 2014, about 240GBs worth of data, due to storage limits. We need to retrieve this data and put it on the Internet Archive for safekeeping. 

The Bibliotheca Anonoma has recieved the pruned images from 4plebs via tar piping, and will be uploading to the Internet Archive shortly.

== List of Boards ==

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/adv/''' - Advice
| [http://archive.4plebs.org/adv/search/order/asc/ 2014-01-12]
| '''4plebs.org''' 
|-
| '''/f/''' - Flash
| [http://archive.4plebs.org/f/search/order/asc/ 2014-03-15]
| '''4plebs.org''' 
|-
| '''/hr/''' - High Resolution
| [http://archive.4plebs.org/hr/search/order/asc/ 2012-12-01] (around birth)
| '''4plebs.org''' 
|-
| '''/o/''' - Auto
| [http://archive.4plebs.org/o/search/order/asc/ 2013-03-13]
| '''4plebs.org''' 
|-
| '''/pol/''' - Politically Incorrect
| [http://archive.4plebs.org/pol/search/order/asc/ 2013-10-28]
| '''4plebs.org''' 
|-
| '''/s4s/''' - Shit 4chan Says
| [http://archive.4plebs.org/s4s/search/order/asc/ 2013-10-05]
| '''4plebs.org''' 
|-
| '''/sp/''' - Sports
| [http://archive.4plebs.org/sp/search/order/asc 2012-06-11]
| '''4plebs.org''' <- not4plebs.org <- (late 2014 threads lost) <- Archive.moe <- foolz.us
|-
| '''/tg/''' Traditional Games
| [http://archive.4plebs.org/tg/search/order/asc/ 2011-06-26]
| '''4plebs.org''' 
|-
| '''/trv/''' - Travel
| [http://archive.4plebs.org/trv/search/order/asc/ 2012-07-02]
| '''4plebs.org''' 
|-
| '''/x/''' - Paranormal
| [http://archive.4plebs.org/x/search/order/asc/ 2013-04-01]
| '''4plebs.org''' 
|}

== Method 1: Web Scraping ==

Using wget, we just scrape the images off the server. It's not elegant, but it works, and thankfully [http://img.4plebs.org/boards/o/image/to_be_removed_in_order.txt the admin has provided some image lists.] (change board name in URL to view another list) This will take about a month at least, and that's assuming we're scraping in parallel. The following bash script is used:

<pre>
!/bin/bash
board="tg"
wget http://img.4plebs.org/boards/$board/image/to_be_removed_in_order.txt
sed -e 's|^./|http://img.4plebs.org/boards/$board/image/|g' -i to_be_removed_in_order.txt
wget -b --tries=10 -nc -c -i to_be_removed_in_order.txt --user-agent="Bibliotheca Anonoma Website Archiver/1.1 (+http://github.com/bibanon/bibanon/wiki)" -w 1
</pre>

== Web Scraping ETA ==

Below are rough estimates for scraping time, procedurally calculated based on the amount of images listed. 

These were intentionally overestimated to ensure that my VPS actually had enough space and time, but actually the time estimates are off by a factor of 9, since it only took 15 hours to scrape 5GBs of data (from /s4s/), not 6 days. Maybe it should be 1.1 seconds, rather than 2? We used a delay just to be polite.

Assumes:

* 2 second Average Download Time (includes 1 second delay)
* 600KB Average filesize for regular boards
* 3MB Average filesize for high resolution boards
* 8MB Average filesize for /f/lashes

=== Total ===

* Total Amount of Images: 372123
* Total Estimated Size: 244789 MB (or) 240 GB
* Total Estimated Timespan:
* Parallel: 1 month (30 days)
* Sequential: 2063 hours (or) 85 days

=== /adv/ ===

Status: <span style="color: blue;">'''Scraping - 2015-09-20'''</span>

* Amount of Images: 12973
* Estimated Timespan: 72 hours (or) 3 days
* Estimated Size: 7601 MB (or) 8 GB
** Actual Timespan: 7h 18m 10s
** Actual Size: 3.3G

=== /hr/ ===

* Amount of Images: 11082
* Estimated Timespan: 61 hours (or) 2 days
* Estimated Size: 33246 MB (or) 33 GB

=== /f/ ===

Nothing to be pruned?

=== /o/ ===

* Amount of Images: 37437
* Estimated Timespan: 207 hours (or) 8 days
* Estimated Size: 21935 MB (or) 22 GB

=== /pol/ ===

* Amount of Images: 107115
* Estimated Timespan: 595 hours (or) 24 days
* Estimated Size: 62762 MB (or) 62 GB

=== /s4s/ ===

Status: <span style="color: blue;">'''Scraping - 2015-09-20'''</span>

* Amount of Images: 29504
* Estimated Timespan: 163 hours (or) 6 days
* Estimated Size: 17287 MB (or) 17 GB
** Actual Timespan: 15h 30m
** Actual Size: 5.7G

=== /sp/ ===

Nothing to be pruned?

=== /tg/ ===

* Amount of Images: 60556
* Estimated Timespan: 336 hours (or) 14 days
* Estimated Size: 35482 MB (or) 34 GB

=== /trv/ ===

Status: <span style="color: blue;">'''Saved! - 2015-09-21'''</span>

* Amount of Images: 1713
* Estimated Timespan: 9 hours
* Estimated Size: 1003 MB (or) 1 GB
** Actual Timespan: 1h 6m 32s
** Actual Size: 1.1G

=== /tv/ ===

* Amount of Images: 99399
* Estimated Timespan: 552 hours (or) 23 days
* Estimated Size: 58241 MB (or) 57 GB

=== /x/ ===

Status: <span style="color: green;">'''Saved! - 2015-09-20'''</span>

* Amount of Images: 12344
* Estimated Timespan: 68 hours (or) 2 days
* Estimated Size: 7232 MB (or) 7 GB
** Actual Timespan: 6h 55m 29s
** Actual Size: 3.4G

== Method 2: tar Piping ==

Web scraping does eat up bandwidth and take quite a long time. A better method is to pipe a tar archive from their host server to our (dedicated) server. Yes you heard that right, the tar backup is ''stored directly on the remote server'', not on the host server. 

That way, the host server doesn't have to store a redundant backup that could be massive. Instead, just spit it at our server directly.

<pre>
tar -c /path/to/dir | ssh remote_server 'tar -xvf - -C /absolute/path/to/remotedir'
</pre>

This would only take about a week or so to transfer 240GBs of data, and reduces the amount of overhead on the web server from requesting 330,000 files: we only send one continuous stream of data.

* [http://serverfault.com/questions/18125/how-to-copy-a-large-number-of-files-quickly-between-two-servers/18142#18142 Source: StackOverflow - Tar piping]
