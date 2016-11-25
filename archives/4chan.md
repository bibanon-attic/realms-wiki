> ### Note:
this is an updated miror of the [ArchiveTeam wiki's 4chan page](http://www.archiveteam.org/index.php?title=4chan)

[//]: #![](http://i.imgur.com/Gm7szlY.jpg)


4chan is said to be one of the most significant and "interesting" websites in existence. It has a unique anonymous imageboard posting system, and has a disproportionate influence on English-language internet culture.

The website eventually deletes threads after they reach a bump limit. However, numerous archive sites and wikis have taken up the task of saving threads and images. Numerous others have fallen. We need to keep watch on these fragile, community supported archives, since they can easily collapse without warning.


## Vital Signs

* **2015-10-07 - Archive.moe: 410 Gone** - Archive.moe announced their shutdown today effective immediately after hardware issues wiped their database. They are currently offering [a dump of their text database](https://archive.org/details/archive-moe-database-201506), that goes up to June 2015, the last working backup. Images are on the way, but due to the large size (over 10 TB) it's taking some time.
  * [An anon who has apparently been running his own personal archive of every board](https://desustorage.org/qa/thread/282229/#282933) has offered to upload the data from the four missing months, but it's going to take a while to finish uploading everything. As of this writing, /vp/ has been uploaded (check the thread for links). [[Bibliotheca Anonoma]] has offered to give assistance, no word on whether or not he's taken it up.
* 2015-09-19 [4plebs Purge](archives/4chan/4pleb) (Archived!) - Removing full images older than 18 months (before April 2014) as of September, 2015, due to low storage space. Obtained the data, now working to upload the whole set to the Internet Archive.

## Past

* dis.4chan.org - 4chan's 2ch-style text boards. All posts from the beginning of the forum's existence are archived, unlike most of 4chan. Therefore, it gives a rare historic snapshot of 4chan's past. 
** Taken down for good on July 26, 2015, [archived in full by a anonymous /prog/ user](http://bbs.progrider.org/prog/read/1397949784/34) ([archive.org](https://archive.org/details/@ghonsonb3120)).
* /rs/ - 4chan's filesharing link search board. All filesharing links ever posted to any 4chan board have been recorded here.
** As of 04-08-2014, Moot is retiring the Filesharing search board (/rs/) and the Discussion boards (dis.4chan.org). The Discussion boards are being hidden from the main site, but kept in a read-only state; this could be a good Warrior/Wget side project.
** Not sure if it is still available... Seems to be down with no archives ever made. Could have a few snapshots on the Internet Archive.

## Scripts

Some scripts you can use to archive 4chan threads yourself.

* [https://github.com/bibanon/BASC-Archiver BASC Archiver] - Python-based 4chan Thread Archiver for Windows/Mac OS X/Linux. Archives everything: Images, Thumbnails, Thread HTML, JSON, etc.
* [https://github.com/FoolCode/FoolFuuka FoolFuuka] - Make your own 4chan board archiver website. Fuuka will grab every single thread from 4chan and save it for later public access.

## Fuuka-based Archivers

: '''Fun Fact''': ''Asagi is the eldest of the Ayase sisters. Fuuka is the middle sister. The Ayase family lives next door to Yotsuba. Get it?'' - [https://github.com/eksopl/asagi#whats-with-the-name eksopl]

'''Fuuka''' is a 4chan board dumper that allows servers to archive entire boards on 4chan. [https://code.google.com/p/fuuka/ It was invented] by '''Anonymous of Russia''' (aka [https://web.archive.org/web/20100524173230/http://code.google.com/u/andrey.osenenko/ Andrey Osenenko]) and improved by [https://web.archive.org/web/20100525001818/http://code.google.com/u/eksopl/ eksopl] ([https://github.com/eksopl/fuuka Github]). [https://github.com/eksopl/asagi Asagi] is a re-implementation of the Fuuka dumper (in Java) with some significant improvements. Created by eksopl.

[https://github.com/FoolCode/FoolFuuka FoolFuuka] is a significantly improved fork of Fuuka & Asagi, (still being) developed by the FoolCode Team: with a better theme, better design, performance optimization, post-thread comments and even a fully functional imageboard, It is used by Archive.moe, and various others.

It would be a good idea to persuade these archivers to upload database dumps to the Internet Archive, just in the very likely case that some disaster befalls them.

The 4chan-X extension [https://github.com/MayhemYDG/archives.json maintains an updated list of all Fuuka Archivers], as well as their start and end dates. Very useful.

=== Boards not currently archived via Fuuka ===

* /j/ - Janitor & Moderator Discussion (staff board; obviously not archivable)
** Some parts of the board have been archived thanks to various leaks throughout the years, a collection of all known files from /j/ can be downloaded [https://mega.co.nz/#!EFVUGSZa!duVWgDwLD2FlXOOdwa9uWjQtO6AlSbKVt7nq2bI5-VY here] (dead as of 5/1/2016).

=== archive.fireden.net (Static Archive.moe Viewer) ===

[http://archive.fireden.net archive.fireden.net] runs a viewable version of Archive.moe's threads and thumbs, which were all uploaded to the Internet Archive (except for the period between 2015-06 to 2015-10, which was lost).

=== desustorage.org ===
{{Infobox project
| title = desustorage
| image = Desustorage.png
| URL = [https://desustorage.org/ desustorage.org]
| project_status = {{online}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

Status: <span style="color: green;">'''Online'''</span>
Saves Images?: <span style="color: green;">'''Yes'''</span>

This site was nominated by [[Bibliotheca Anonoma]] as the primary successor to archive.moe and is currently in the process of importing content from the late site. It currently archives /a/, /aco/, /c/, /co/, /d/, /fit/, /his/, /int/, /k/, /m/, /mlp/, /q/, /qa/, /r9k/, /tg/, /vr/ and /wsg/.

Desustorage also has a private Archiver of Last Resort running in parallel that archives all 4chan boards privately, as insurance against the possibility of a 4chan archiver site collapsing in the future.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
! Thumbnails
! Oldest Full Image
|-
| '''/a/''' - Animu & Mango
| [https://desustorage.org/a/search/order/asc/page/2/ 2008-02-03]
| '''desustorage.org''' <- Sunako's Asagi & archive.moe <- foolz.us <- easymodo.net <- green-oval.net
| Pending
| Pending
|-
| '''/aco/''' - Adult Cartoons
| [https://desustorage.org/aco/search/order/asc/page/2/ 2015-10-08]
| '''desustorage.org'''
| {{Yes}}
| {{Yes}}
|-
|'''/an/''' - Animals & Nature
|[http://desustorage.org/an/search/order/asc/ 2015-03-23]
|'''desustorage.org'''
|Pending
|Pending
|-
| '''/c/''' - Cute Animu
| [https://desustorage.org/c/search/order/asc/ 2012-04-02]
| '''desustorage.org''' <- archive.moe <- foolz.us <- thedarkcave.org
| Pending
| Pending
|-
| '''/co/''' - Comics and Cartoons
| [https://desustorage.org/co/search/order/asc/ 2012-05-21]
| '''desustorage.org''' <- archive.moe <- foolz.us
| {{Yes}}
|Pending
|-
|'''/d/''' - Hentai/Alternative
|[http://desustorage.org/d/search/order/asc/ 2013-03-04]
|Pending
|Pending
|Pending
|-
|'''/fit/''' - Fitness
|[http://desustorage.org/fit/search/order/asc/ 2010-10-12]
|Pending
|Pending
|Pending
|-
|'''/gif/''' - Adult GIF
|[http://desustorage.org/gif/thread/7997204/#7997204 2016-01-21]
|'''desustorage.org'''
|{{Yes}}
|{{Yes}}
|-
| '''/his/''' - History
| [https://desustorage.org/his/search/order/asc/ 2015-10-28] (From Birth)
| '''desustorage.org'''
| {{Yes}}
| {{Yes}}
|-
| '''/int/''' - International
| [https://desustorage.org/int/search/order/asc/ 2013-01-08]
| '''desustorage.org''' <- archive.moe <- foolz.us <- thedarkcave.org
| Pending
| Pending
|-
| '''/k/''' - Weapons
| [https://desustorage.org/k/search/order/asc/ 2012-07-13]
| '''desustorage.org''' <- archive.moe <- heinessen.com
| {{Yes}}
| Pending
|-
| '''/m/''' - Mecha
| [https://desustorage.org/m/search/order/asc/ 2009-03-27]
| '''desustorage.org''' <- archive.moe <- foolz.us <- easymodo.net
| Pending
| Pending
|-
| '''/mlp/''' - Pony
| [https://desustorage.org/mlp/search/order/asc/ 2012-03-27] (from birth)
| '''desustorage.org''' <- archive.horse & archive.moe <- heinessen.com
| {{Yes}}
| [https://archive.org/details/heinessen-mlp-images Internet Archive]
|-
|'''/q/''' - 4chan Feedback
|[http://desustorage.org/q/search/order/asc/ 2012-08-07](near birth to death)
|Pending
|Pending
|Pending
|-
| '''/qa/''' - Questions and Answers
| [https://desustorage.org/qa/search/order/asc/ 2015-01-23] (from birth)
| '''desustorage.org'''
| {{Yes}}
| {{Yes}}
|-
| '''/r9k/''' - ROBOT 9001
| [https://desustorage.org/r9k/search/order/asc/ 2012-06-02]
| '''desustorage.org''' <- archive.moe <- heinessen.com
| {{Yes}}
| Pending
|-
| '''/tg/''' - Traditional Games
| [https://desustorage.org/tg/search/order/asc/ 2010-02-23]
| '''desustorage.org''' <- archive.moe <- foolz.us <- easymodo.net
| {{Yes}}
| Pending
|-
|'''/trash/''' - Off Topic
|[http://desustorage.org/trash/thread/1/#1 2015-11-07](from birth)
|'''desustorage.org'''
|{{Yes}}
|{{Yes}}
|-
| '''/vr/''' - Retro Games
| [https://desustorage.org/vr/search/order/asc/ 2013-03-18] (from birth)
| '''desustorage.org''' <- archive.moe <- foolz.us
| {{Yes}}
| Pending
|-
| '''/wsg/''' - Worksafe GIF
| [https://desustorage.org/wsg/search/order/asc/ 2012-06-04] (from birth)
| '''desustorage.org''' <- archive.moe <- foolz.us
| {{Yes}}
| Pending
|}

Notice: With the exception of /a/ (restored through other means), all thread text for Archive.moe boards from June 2015 - October 2015 were lost. If anyone has this data, please [mailto:atc@archive.horse contact] [https://desustorage.org/desu/ atc] at [https://qchat.rizon.net/?channels=desustorage&uio=d4 Desustorage].


=== arch.b4k.co ===
{{Infobox project
| title = b4k
| image = B4kco.png
| URL = [http://arch.b4k.co/ arch.b4k.co]
| project_status = {{online}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

Status: <span style="color: green;">'''Online'''</span>
Saves Images?: <span style="color: blue;">'''Thumbnails Only'''</span>

This site currently archives /g/, /mlp/ and /v/. It was designed as a temporary archive, but is now the primary archiver for the high volume board, /v/.

=== boards.fireden.net ===
{{Infobox project
| title = fireden
| image = fireden.png
| URL = [https://boards.fireden.net/ boards.fireden.net]
| project_status = {{online}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

Status: <span style="color: green;">'''Online'''</span>
Saves Images?: <span style="color: green;">'''Yes'''</span>

This site currently archives /a/, /cm/, /ic/, /sci/, /tg/, /v/, /vg/, /y/. It was designed as a temporary archive, but is now a major archiver for the high volume boards, /v/ and /vg/.

=== rbt.asia/rebeccablacktech.com ===

{{Infobox project
| title = rebeccablacktech
| image = rbt-asia.png
| URL = [http://rbt.asia rbt.asia]
| project_status = {{online}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

Status: <span style="color: green;">'''Online'''</span>
Saves Images?: <span style="color: green;">'''Yes'''</span>

A Fuuka archiver for /cgl/, /g/ and /mu/. /soc/ moved to [[#fgts.jp|fgts]], /con/, /qa/ and /w/ moved to [[#archive.nyafuu.org|nyafuu]].

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Full Images
! Pedigree
|-
| '''/cgl/''' - Cosplay & EGL
| [https://rbt.asia/cgl/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_media_hash=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2012-05-06]
| {{Yes}}
| '''rbt.asia''' <- ???
|-
| '''/g/''' - Technology
| [https://rbt.asia/g/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_media_hash=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2011-11-11]
| {{Yes}}
| '''rbt.asia''' <- installgentoo.net
|-
| '''/mu/''' - Music
| [https://rbt.asia/mu/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_media_hash=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2013-05-30]
| {{Yes}}, Temp.
| '''rbt.asia'''
|}

=== warosu.org ===

{{Infobox project
| title = warosu.org
| image = warosu.png
| URL = [http://warosu.org warosu.org]
| project_status = {{online}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

Status: <span style="color: green;">'''Online'''</span>
Saves Images?: <span style="color: red;">'''Partially'''</span> (all boards except /g/)

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Full Images
|-
| '''/3/''' - 3DCG
| [https://warosu.org/3/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2014-01-12]
| {{Yes}}
|-
| '''/biz/''' - Business & Finance
| [https://warosu.org/biz/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2014-03-15]
| {{Yes}}
|-
| '''/cgl/''' - Cosplay & EGL
| [https://warosu.org/cgl/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2014-03-15]
| {{Yes}}
|-
| '''/ck/''' - Cooking
| [https://warosu.org/ck/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2012-12-01]
| {{Yes}}
|-
| '''/diy''' - Do-It-Yourself
| [https://warosu.org/diy/?task=search2&ghost=yes&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2011-10-22] (from birth)
| {{Yes}}
|-
| '''/fa/''' - Fashion
| [https://warosu.org/fa/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2013-03-13]
| {{Yes}}
|-
| '''/g/''' - Technology
| [https://warosu.org/g/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2013-03-13]
| {{No}}
|-
| '''/ic/''' - Artwork/Critique
| [https://warosu.org/ic/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2013-10-28]
| {{Yes}}
|-
| '''/jp/''' - Otaku Culture
| [https://warosu.org/jp/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2013-10-05]
| {{Yes}}
|-
| '''/lit/''' Literature
| [https://warosu.org/lit/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2011-06-26]
| {{Yes}}
|-
| '''/sci/''' - 
| [https://warosu.org/sci/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2012-07-02]
| {{Yes}}
|-
| '''/tg/''' - Traditional Games
| [https://warosu.org/tg/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2013-04-01]
| {{Yes}}
|-
| '''/vr/''' - Retro Games
| [https://warosu.org/vr/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2013-04-01]
| {{Yes}}
|}

=== archive.4plebs.org ===

{{Infobox project
| title = archive.4plebs.org
| image = archive-4plebs.png
| URL = [http://archive.4plebs.org archive.4plebs.org]
| project_status = {{online}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

Status: <span style="color: green;">'''Online'''</span>
Saves Images?: <span style="color: green;">'''Yes'''</span>

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
|'''/tv/''' - Television & Film
|[http://archive.4plebs.org/tv/search/order/asc/ 2013-04-03]
|'''4plebs.org'''
|-
| '''/x/''' - Paranormal
| [http://archive.4plebs.org/x/search/order/asc/ 2013-04-01]
| '''4plebs.org''' 
|}

Note: The /sp/ archive was indirectly inherited from Foolz.us/Archive.moe, as they stopped archiving the board after it got spammed with CP in a user revolt. Archive.moe posted backups, but the board was not archived for much of late 2014/early 2015. Eventually, totally.not4plebs.org imported the /sp/ archive and started again in mid-2015, and was later merged into 4plebs.org. Unfortunately, many thumbnails were lost in the transfer to Archive.moe from Foolz.us.

==== Image Purges ====

4plebs has been forced to purge full images at various points in it's lifetime, due to low storage space.

Currently, 4plebs plans to purge all full images from before April 2014 (18 months). This is about 240GBs of images. We need to receive the whole set from them and upload it to the Internet Archive for safekeeping.

''More info/Project Page'': [[4chan/4plebs]]

=== archive.nyafuu.org ===

{{Infobox project
| title = archive.nyafuu.org
| image = archive-nyafuu.png
| URL = [http://archive.nyafuu.org archive.nyafuu.org]
| project_status = {{online}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

Status: <span style="color: green;">'''Online'''</span>
Saves Images?: <span style="color: blue;">'''Yes'''</span>

'''Start Date:''' ~2011
'''Temporary Shutdown Date:''' [https://github.com/MayhemYDG/archives.json/commit/4c0b13295329b5246f61ee2d5ba4a2dc4855be88 2014-08-27]
'''Restoration Date:''' 2015-02-11

A Fuuka archiver for /c/, /e/, /w/, /wg/, /wsr/, and /news/ which provides full image archiving, created by [https://github.com/voh VoH]. /e/ is NSFW. 

It temporarily shut down on August 27, 2014, and all the boards were [https://github.com/MayhemYDG/archives.json/commit/832ead70a62f6785611e093f922d94d9fdb58cd5 inherited safely by archive.loveisover.me.]

Now that Nyafuu has come back (as of 2015-02-11), loveisover.me has returned all archives back to Nyafuu.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/c/''' - Anime/Cute
| [http://archive.nyafuu.org/c/search/order/asc/ 2011-06-08]
| '''nyafuu.org''' ~ '''loveisover.me''' <- nyafuu.org
|-
| '''/e/''' - Ecchi
| [http://archive.nyafuu.org/e/search/order/asc/ 2012-10-13]
| '''nyafuu.org''' ~ '''loveisover.me''' <- nyafuu.org
|-
| '''/w/''' - Anime/Wallpapers
| [http://archive.nyafuu.org/w/search/order/asc/ 2012-01-11]
| '''nyafuu.org''' <- loveisover.me <- nyafuu.org
|-
| '''/wg/''' - Wallpapers/General
| [http://archive.nyafuu.org/wg/search/order/asc/ 2013-04-10]
| '''nyafuu.org''' <- loveisover.me <- nyafuu.org
|-
| '''/wsr/''' - Worksafe Requests
| [http://archive.nyafuu.org/wsr/search/order/asc/ 2015-12-20] (from birth)
| '''nyafuu.org'''
|-
| '''/news/''' - Current News
| [http://archive.nyafuu.org/news/search/order/asc/ 2015-11-27] (from birth)
| '''nyafuu.org'''
|}

=== archive.loveisover.me ===

{{Infobox project
| title = archive.loveisover.me
| image = archive-loveisover-me.png
| URL = [http://deploy.loveisover.me deploy.loveisover.me]
| project_status = {{online}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

Status: <span style="color: green;">'''Online'''</span>
Saves Images?: <span style="color: green;">'''Yes'''</span>

During December of 2015 and to mid-February of 2016 the main page announced that it was transferring files to a different location and could take a few weeks because of a slow connection, it took a lot longer than that. They probably are not archiving during this time, but that is not certain.


A pure NSFW Fuuka archiver for /d/, /i/, /lgbt/, and /u/, created by Blade. It also inherited the [https://archive.loveisover.me/t/thread/522650/#585860 archive.mawa.re /t/ archive.]

[http://blog.loveisover.me/?cat=3 Has assumed responsibility of boards formerly curated by archive.nyafuu.org] /c/, /e/, /w/, /wg/, as of November 2014, but full image support (except for /e/) was temporarily disabled. 

Now that Nyafuu is coming back (as of 2015-02-11), loveisover.me has given them the archives of /c/, /e/, /w/, /wg/. It no longer hosts /w/ and /wg/, but still keeps /c/ and /e/.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/c/''' - Anime/Cute
| [http://archive.loveisover.me/c/search/order/asc/ 2011-06-08]
| '''nyafuu.org''' ~ '''loveisover.me''' <- nyafuu.org
|-
| '''/d/''' - Hentai/Alternative
| [http://archive.loveisover.me/d/search/order/asc/ 2013-03-04]
| '''loveisover.me''' <- (???)
|-
| '''/e/''' - Ecchi
| [http://archive.loveisover.me/e/search/order/asc/ 2012-10-13]
| '''nyafuu.org''' ~ '''loveisover.me''' <- nyafuu.org
|-
| '''/i/''' - Oekaki
| [http://archive.loveisover.me/i/search/order/asc/ 2011-11-05]
| '''loveisover.me''' <- (???)
|-
| '''/lgbt/''' - Lesbian, Gay, Bisexual, & Transgender
| [http://archive.loveisover.me/lgbt/search/order/asc/ 2014-04-12]
| '''loveisover.me'''
|-
| '''/t/''' - Torrents
| [http://archive.loveisover.me/t/search/order/asc/ 2012-06-08]
| '''loveisover.me''' <- mawa.re
|-
| '''/u/''' Yuri
| [http://archive.loveisover.me/u/search/order/asc/ 2013-06-23]
| '''loveisover.me'''
|-
| '''/w/''' - Anime/Wallpapers
| [http://archive.nyafuu.org/w/search/order/asc/ 2012-01-11]
| '''nyafuu.org''' <- loveisover.me <- nyafuu.org
|-
| '''/wg/''' - Wallpapers/General
| [http://archive.nyafuu.org/wg/search/order/asc/ 2013-04-10]
| '''nyafuu.org''' <- loveisover.me <- nyafuu.org
|}

=== List of Fuuka Archivers by board ===

{| class="sortable wikitable" border="1"
|-
! Board || 4plebs || Nyafuu || Love is Over || Rebecca Black Tech || warosu || Desustorage || fireden.net || arch.b4k.co || Total
|-
| '''/3/''' - 3DCG || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/a/''' - Anime & Manga || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{Yes}} || {{No}} || '''2'''
|-
| '''/aco/''' - Adult Cartoons || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/adv/''' - Advice || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/an/''' - Animals & Nature || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/asp/''' - Alternative Sports || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/b/''' - Random || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/biz/''' - Business & Finance || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/c/''' - Anime/Cute || {{No}} || {{Yes}} || {{Maybe}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''3'''
|-
| '''/cgl/''' - Cosplay & EGL || {{No}} || {{No}} || {{No}} || {{Yes}} || {{Yes}} || {{No}} || {{No}} || {{No}} || '''2'''
|-
| '''/ck/''' - Food & Cooking || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/cm/''' - Cute/Male || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || '''1'''
|-
| '''/co/''' - Comics & Cartoons || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/d/''' - Hentai/Alternative || {{No}} || {{No}} || {{Maybe}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''2'''
|-
| '''/diy/''' - Do It Yourself || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/e/''' - Ecchi || {{No}} || {{Yes}} || {{Maybe}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''2'''
|-
| '''/f/''' - Flash || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/fa/''' - Fashion || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/fit/''' - Fitness || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/g/''' - Technology || {{No}} || {{No}} || {{No}} || {{Yes}} || {{Yes}} || {{No}} || {{No}} || {{Maybe|Thumbs only}} || '''3'''
|-
| '''/gd/''' - Graphic Design || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/gif/''' - Adult GIF || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/h/''' - Hentai || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/hc/''' - Hardcore || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/his/''' - History & Humanities || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/hm/''' - Handsome Men || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/hr/''' - High Resolution || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/i/''' - Oekaki || {{No}} || {{No}} || {{Maybe}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/ic/''' - Artwork/Critique || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{Yes}} || {{No}} || '''2'''
|-
| '''/int/''' - International || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/jp/''' - Otaku Culture || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/k/''' - Weapons || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/lgbt/''' - LGBT || {{No}} || {{No}} || {{Maybe}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/lit/''' - Literature || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/m/''' - Mecha || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/mlp/''' - Pony || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{Maybe|Thumbs only}} || '''2'''
|-
| '''/mu/''' - Music || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/n/''' - Transportation || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/news/''' - News || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/o/''' - Auto || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/out/''' - Outdoors || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/p/''' - Photography || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/po/''' - Papercraft & Origami || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/pol/''' - Politically Incorrect || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/qa/''' - Question & Answer || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{Yes}} || {{No}} || {{No}}|| '''2'''
|-
| '''/r/''' - Request || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/r9k/''' - ROBOT9001 || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/s/''' - Sexy Beautiful Women || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/s4s/''' - Shit 4chan Says || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}}|| {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/sci/''' - Science & Math || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{Yes}} || {{No}} || '''2'''
|-
| '''/soc/''' - Cams & Meetups || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/sp/''' - Sports || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/t/''' - Torrents || {{No}} || {{No}} || {{Maybe}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/tg/''' - Traditional Games || {{Yes}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{Yes}} || {{Yes}} || {{No}} || '''4'''
|-
| '''/toy/''' - Toys || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/trash/''' - Off Topic || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/trv/''' - Travel || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/tv/''' - Television & Film || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/u/''' - Yuri || {{No}} || {{No}} || {{Maybe}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/v/''' - Video Games || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{Maybe|Thumbs only}} || '''2'''
|-
| '''/vg/''' - Video Game Generals || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || '''1'''
|-
| '''/vp/''' - Pokémon || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''0'''
|-
| '''/vr/''' - Retro Games || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{Yes}} || {{No}} || {{No}} || '''2'''
|-
| '''/w/''' - Anime/Wallpapers || {{No}} || {{Yes}} || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || '''2'''
|-
| '''/wg/''' - Wallpapers/General || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/wsg/''' - Worksafe GIF || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || {{No}} || '''1'''
|-
| '''/wsr/''' - Worksafe Requests || {{No}} || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/x/''' - Paranormal || {{Yes}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || '''1'''
|-
| '''/y/''' - Yaoi || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{No}} || {{Yes}} || {{No}} || '''1'''
|}

== Selective Archives ==

These websites archive a selection of threads that users vote to retain, or rehost archives that would otherwise have disappeared.

=== The Second 4archive.org ===

{{Infobox project
| title = The Second 4archive.org
| image = 4chanarchives-cu-cc.png
| URL = [http://4archive.org 4archive.org]
| project_status = {{online}}
| archiving_status = {{saved}}
| irc = 4chanarchives
}}

: ''The site originally used the domain 4chanarchives.cu.cc until December 19th, 2015. The admin of the First 4archive.org bequeathed the domain to the Bibliotheca Anonoma, who provided it to 4chanarchives.cu.cc.''

The Second '''[http://4archive.org 4archive.org]''' was created by Bloo in mid-2015. It currently is the only site displaying 4chan threads from the First 4archive, which closed on May 2015. It also scrapes certain boards on 4chan regularly using a heavily modified version of the 4archive Lumen framework and [http://pastebin.com/X9UVR6fc some custom PHP scripts]. 

This site is notable as it is one of the few self-sustaining, for profit 4chan archivers (using ads). It's a different approach, but at least it keeps the admin motivated enough to deal with floods of DMCA reports for spicy content. There hasn't been an archiver like it since the Chanarchive, and at the very least, 4archive.org welcomes as many users and as much data as possible.

* The admin aims to regularly archive all threads from all NSFW boards on 4chan, and some SFW boards. This is achieved by scraping the 4chan API's `archive.json` and `boards.json`. Using this method, 1TB of images and 9 million posts have been archived in November 2015. See the [https://i.imgur.com/WXcf4OY.png 4chanarchives.cu.cc Archiving Diagram] for more information.
* In the future there will be an efficient system built from scratch for user submitted thread archival. This will be a definite improvement over Fuuka and Asagi, which predate the 4chan API, and has subpar CPU/RAM performance these days.
* When it comes to ads, SFW ads will appear on the frontpage and SFW boards (/a/, /v/, /trv/, etc.), while NSFW ads will only appear on NSFW boards (/b/, /h/, /s/, /u/, etc.).
* Just like it's predecessor, the First 4archive, all full size images are saved using Imgur's subscription paid plan. Bloo has also rescued more than 632k images from Imageshack (which was shutting down their free service) to Imgur via MashapeAPI.
* The admin is working on setting up a 1:1 version of Archive.moe, just as it was before the day it died. He has plans to someday convert the 4Archive's DB to fit the Fuuka DB structure.

--------

''The admin is online 24/7 on '''irc.rizon.net at #4chanarchives''' and #bibanon (nickname: Bloo_SemiAFK)''

* [http://pastebin.com/SbR1EF9t 4chanarchives.cu.cc Description by Bloo]
* [https://i.imgur.com/WXcf4OY.png 4chanarchives.cu.cc Archiving Diagram]
* [http://pastebin.com/X9UVR6fc Source code of 4chanarchives' thread.php]

=== Swfchan ===

[http://swfchan.org Swfchan] is a massive Flash archive that scrapes and archives flashes from the 4chan /f/ board (among other places). 163831 have been saved as of 2015-02-11. 

These flashes are an important artistic record of the culture back in the day. 

However, it's funding situation is a bit precarious and relies heavily on pop-up ads and donations to stay alive. It's worth making a contingency backup of the site someday.

=== Dagobah ===

[http://dagobah.net/ Dagobah], another Flash archive strongly associated with 4chan. Also has a ton of 2ch flashes by extension.

=== 4chan Flash archive ===

{{Infobox project
| title = 4chan Flash archive
| image = 4chanflash.png
| URL = [https://4chan.org/flash 4chan.org/flash]
| project_status = {{online}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

A small archive of Flash files related to 4chan culture. Run by 4chan and updated very rarely by the staff. The archive was originally started to stop users from posting the same flashes over and over again; any file on the page is not allowed to be posted on /f/.

=== Sup/tg/ ===
{{Infobox project
| title = Suptg
| image = suptg.png
| URL = [http://suptg.thisisnotatrueending.com suptg.thisisnotatrueending.com]
| project_status = {{online}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

A site created by /tg/ members in 2009, it has a considerable community of its own, providing reviews and RPG materials. sup/tg/ has a uniquely crated archive with full image support. Unlike most other archives listed, moderators conduct routine purges of low-rated threads, a process they refer to as "graveyarding". The only other site that had a similar policy was Chanarchive, but they deleted threads while they were incoming.

=== 4chandata/4chanarchive ===
{{Infobox project
| title = 4chandata
| image = 4chandata.png
| URL = [http://4chanarchive.net 4chanarchive.net], formerly [http://4chandata.org 4chandata.org]
| project_status = {{online}}, inactive
| archiving_status = {{inprogress}}
| irc = ???
}}

A considerably wide cross-section of 4chan's SFW boards, starting at August 8 2012. Ironically, despite being an imageboard archive, the site itself is unwilling to host images due to the possibility of legal issues surrounding content. While there is content overlap with the Fuuka-based archivers, the site's good to include for the sake of completeness. 4chandata was supplanted by 4chanarchive.net, and both sites appear to be in a precarious hosting situation with archiving coming to a sudden halt on November 20th 2014.

* On 2015-02-25, an ArchiveBot session was started for both 4chanData.org and 4chanarchive.net, to scrape all thread text and upload it to the Wayback Machine before it disappears for good.
* [https://archive.org/details/2013_10_25_4chandata 100GB 4chandata.org Image Archive] - An anon [http://badcheese.com/~steve/atlogs/?chan=archiveteam&day=2013-10-28 uploaded a full backup] of over 100GBs of image data from this site before the images were deleted permanently.

=== 4walled & nik.bot.nu ===

Two successors to 4scrape that inherited it's data.

* [4walled] - Archives /hr/, /w/, /wg/ but images only.
* [https://nik.bot.nu/ nik.bot.nu] - Archives images from various imageboards around the world, including 4chan.

=== Fybertech 4archive ===

Status: <span style="color: green;">'''Online'''</span>
Archived?:<span style="color: green;">'''Yes'''</span>, currently up to 2015-02-16. Archive again in two months.

Fybertech has one of the largest collections of 2008-2014 4chan threads, outside of the fallen Chanarchive and the modern 4archive. It archives any thread referenced in it's IRC channel, apparently.

* [https://archive.org/details/fybertech Internet Archive - FyberTech Archive 2015-02-16] The Bibliotheca Anonoma has made a contingency backup of all 9GBs of threads (up to 2015-02-16) to the Internet Archive.

=== MLP Generals Archive ===

Every /mlp/ general thread ever made.

https://fg.b4k.co/mlpg/archive

=== Wikis ===

* '''[[Encyclopedia Dramatica]]''' - The quintessential 4chan wiki.
* '''[[Insurgency Wiki]]''' - Once, it was almost equal to ED in power and influence. Now, thousands of collapses and failures have reduced it to a broken mess. It would have been gone entirely if it was not for the Bibliotheca Anonoma, which happened to be examining Partyvan.info 2 days before it's collapse.
* '''[https://github.com/bibanon/bibanon/wiki Bibliotheca Anonoma]''' - A wiki designed to save the greatest treasures from around the internet. It strives to provide an index to the archives below to assess their value and display great works to the public. Because what good is a massive mess of information without a guide? 
* '''[http://youtsubasociety.org Yotsuba Society]''' - A place dedicated to studying the culture of 4chan. Maintains a wiki that strives to restore Wikichan to it's former state. <s>As of 1/16/14, the archival portion of the site is down.</s> The archives have been moved in their entirety to the [http://purl.stanford.edu/tf565pz4260 Stanford Digital Library].
* '''[[Wikichan]]''' - The first major 4chan wiki, holding tons of important stories and content. It is the model for many 4chan archive projects to come. The entire wiki collapsed spectacularly several times without recourse, and is the prime example of the problems that occur when a major 4chan archive goes down.
* '''[http://www.lurkmore.com/view/Main_page LURKMORE Wiki]''' - Rarely updated wiki that shifted focus to camgirls; still holds reference material and anecdotes to early 4chan culture.
* '''[https://web.archive.org/web/20110420045345/http://www.lurkmoarpedia.com/wiki/Main_Page Lurkmoarpedia]''' - Some sort of ED clone; not to be confused for LURKMORE.
* '''[http://dramatica.org.ua/%D0%93%D0%BE%D0%BB%D0%BE%D0%B2%D0%BD%D0%B0_%D1%81%D1%82%D0%BE%D1%80%D1%96%D0%BD%D0%BA%D0%B0 Dramatica Ukraine]'''

== Handmade Archives ==

4chan thread archives made thanks to the commands: "Right-click, Save As." 

If you want to do this in the future, please use the [http://github.com/bibanon/BASC-Archiver BASC-Archiver] (saves everything, full images, thumbnails, HTML, JSON, even child threads). "Right-click, Save As" isn't all that efficient and fails to save the full sized images, so please use the script.

=== Yotsuba Society Archives ===

The Yotsuba Society's 4Chan Archive, including separate Imageboard threads /a/, /cgl/, /vg/. 

According to the included [https://stacks.stanford.edu/file/druid:tf565pz4260/A%20message%20from%20Jkid.txt Message from Jkid:] "The following .rar consists of every thread collected from 4chan from my personal archives which were intergrated into the (Yotsuba Society Archives from the Start in 2011) from 2008 to August 2013. Some of these files predate the fuuka archivers that currently exist today to archive almost every thread of every board with the exception of /b/ for obvious reasons. 

From 2011 to August 2013 the Yotsuba Society Archives existed to preserve threads from 4chan and every other imageboard in the English chanverse, plus some threads from the Russian and Japanese chanverse. At it's peak, the Archives were the most visited part of the Yotsuba Society website, and the most popular part of the site were the direct downloads of the moot video archive." The message also includes information about the history of this collection.

* [http://purl.stanford.edu/tf565pz4260 Stanford Digital Repository - Yotsuba Society 4chan Thread Archives]

=== Penfifteen Archive ===

In 2013, [http://rx.vyrd.net/ Vyrd discovered that] some anon (whose native language is Finnish) had this curious, undocumented public archive of very, very early handarchived threads from 4chan (along with many other period-appropriate .swfs, videos, and images), spanning all the way from 2004-2008.

Apparently this may have simply been a personal home server that made it's files publicly accessible.

This repository is known as the Penfifteen Archive, and is the most important discovery of early 4chan threads to date. [http://github.com/bibanon/bibanon/wiki The Bibliotheca Anonoma] has preserved it in the Internet Archive for future generations to enjoy.

* [https://archive.org/details/studionyami-com_penfifteen-2012-03-05 Internet Archive - Penfifteen Archive]

=== 4chan /soc/ Saved Thread Torrent ===

The ArchiveTeam grabbed this torrent containing a massive amount of hand-archived /soc/ threads.

* [https://ia902704.us.archive.org/13/items/4ChanSOCArchive/ Internet Archive - 4chan /soc/ Archive]
* [https://ia902704.us.archive.org/13/items/4ChanSOCArchive/Chan-Archive_torrent.txt List of Threads]

== History of the Fuuka Archiver ==

The ability to archive every thread on a 4chan board was the most influential innovation in 4chan's infrastructure. This idea was a violently controversial shift of consciousness in it's heyday, because it nullifies one of the drawbacks (or benefits) of 4chan: ''the ability to forget.'' 

While 2channel, based on a textboard, could archive years worth of threads for future generations, 4chan threads get constantly pruned due to the expense of storing image data. Moot, [https://github.com/bibanon/bibanon/wiki/Moot%27s-Final-4chan-Q&A-Transcript#130---140 as he states in his Farewell Livestream], developed the ''Salmon Ladder Observation'' as an explanation for early 4chan's success. Essentially, like Alaskan Salmon climbing a rocky stream, only the strongest memes would be remembered and reposted, while poor content was forgotten entirely. Based on this principle, 4chan became the center of Internet Culture from 2005-2007, constantly generating memetic content by bumping the best and saging the worst. Thus, Moot was not opposed to archival by democratic vote, but was uncomfortable with the idea of complete board archival: ''Moot knew indefinite archival would transform 4chan's culture entirely.''

Thus, from 2006-2013, the 4chanarchive/Chanarchive was built upon this same principle, requiring at least 5 users to vote for a thread to be archived. The 4chanarchive held nearly 500GBs worth of 4chan threads spanning 6-8 years. In 2012, the 4chanarchive was transferred to Edgeworth E. Euler (E), who was involved with the new Encyclopedia Dramatica (recovered by Anonymous' OpSaveED). Unfortunately, around 2013, Edgeworth E. Euler mysteriously went MIA, taking his server access keys to the grave. The admins were legally powerless to rescue the site when the hard drives failed, resulting in the complete, unrecoverable loss of the Chanarchive.

After the collapse of the Chanarchive, users of 4chan started to realize that loss of memory was detrimental to their board's subculture. The most gravely affected board was /x/, which lost all of it's creepypasta, and /b/, which saw it's legendary raids and stories disappear into the sunset. Notably, /a/ and /jp/, which used a full Fuuka Archive, made it through intact (unfortunately, the early threads only have thumbnails). As a result, the idea of complete board archival was no longer looked down upon. Most of the larger boards gained their own Fuuka archives and some wikis in the aftermath.

In his final livestream, Moot states that the spirit of 4chan has changed over time, and accepts that today's users want the ability to continue discussion and have general threads. Moot noted that 4chan was becoming more than just a "zany, fun place to hang out, to be creative": ''4chan was now a keystone tool for socialization between anonymous interest groups.'' To ease the burden on it's servers and increase performance, Moot released the 4chan API for use by archivers and mobile apps. Closed threads now live on for at least 7 days on certain boards. And not long after Moot's retirement, (thanks to falling costs of server storage space), all 4chan boards have gained their own Fuuka archive.

=== Fuuka Archiver Variants ===

* [https://github.com/eksopl/fuuka Fuuka] - The original board dumper, written in Perl with an included front-end written by AoRF and maintained by eksopl afterwards.
** A customized version of the original Fuuka code is still utilized by RebeccaBlackTech.
* [https://github.com/eksopl/asagi Asagi] - Re-implementation of the Fuuka dumper in Java, with some significant improvements.
* [https://github.com/FoolCode/FoolFuuka FoolFuuka] - Re-implementation of the fuuka front-end with some significant improvements, including an improved theme. Originally created by the FoolCode Team for the Foolz Archive, it is now the preferred engine for today's Fuuka Archivers. The Asagi dumper is used to actually retrieve the threads.

=== Anonymous of Russia ===

Today, FoolFuuka is the primary scraping engine used to archive 4chan. The Fuuka engine, needed to scrape 4chan efficiently and effectively, did not come out of nowhere. It evolved through hard work and constant refactoring by hundreds of individuals over the course of 8 years and counting.

It was first invented by '''Anonymous of Russia Federation (AoRF)''' (aka [https://web.archive.org/web/20100524173230/http://code.google.com/u/andrey.osenenko/ Andrey Osenenko]) in December 2007 to archive all /a/ threads on his home server, ''The /a/rchive'': http://no-info.no-ip.info/ . 4chan's /a/ was a friendly environment to start an indefinite archiver, as archival allowed general threads to maintain continuity, and helped speedsub groups that used the board for group coordination. Unfortunately, due to ''unknown offenses'', [https://archive.moe/a/thread/9300010/#9302402_2 his ISP was subnet banned] and that server went offline. All three months of /a/ threads from 2007-2008 were lost.

* [https://archive.moe/a/thread/9300010/#9300010 Archive.moe - Discussion on Earliest Attested /a/ thread]

=== Easymodo ===

{{Infobox project
| title = easymodo.net
| image = easymodo.png
| URL = [https://web.archive.org/web/*/http://archive.easymodo.net/ archive.easymodo.net]
| project_status = {{Offline}}
| archiving_status = Inherited by Foolz.us/Archive.moe
| irc = ???
}}

'''Start Date:''' Sometime in 2008 (older than /jp/)
'''Shutdown Date:''' Late 2011

AoRF passed on the source code for his site to a fellow /a/non called [http://archiveteam.org/index.php?title=Talk:4chan#Eksopl.27s_Story_of_Fuuka_and_Easymodo Eksopl] in a RAR-embedded image. Eksopl spruced up the code in English and built the new /a/rchive at http://archive.doesntexist.org/ . When /jp/ was made in 2008, Eksopl set up a second server to archive it from birth (it did not yet support multiple boards).

In October 2008, the /a/non who supplied Eksopl with his servers could no longer support the cost of bandwidth. Eksopl made a partnership with Taro (who ran 4scrape, which archived 4chan images from boards) to host the /a/rchive. Since the archive.doesntexist.org domain was a free DynDNS URL which didn't support CNAMEs, Eksopl gave the /a/rchive a spare domain: easymodo.net.

'''Easymodo''' archived /a/, /jp/ (from birth), /m/, /sci/, /tg/, and /tv/.  Eksopl's two archives of /a/ and /jp/ are the oldest Fuuka archives that still exist. These archives were inherited by the Foolz Archive, and are now under the care of Archive.moe.

In early 2009, AoRF returned to improve Easymodo's source code, and gave it a new name: '''Fuuka'''. One of Fuuka's defining features: "Ghost Posting", was added. (This feature allows /a/nons to write comments on old threads years afterwards). AoRF set up a test server at http://no-info.no-ip.info/ again to stress test the Fuuka engine. When the new and improved Fuuka was ready for release, Eksopl used his own servers to host Easymodo, using the same domain name and same archive data.

Eventually, /m/ and /tg/ would also be archived by Easymodo. However, on June 2010, the old /a/rchive was straining Eksopl's servers, so he transferred /a/ to green-oval.net, a fellow archive built for /tv/ and /g/. Green-oval started having troubles in July 2011; By then Easymodo was better equipped, so it took over Green-oval's /a/ archives. However, to reduce server strain, the search function was disabled for /a/. 

While Eksopl eventually implemented SphinxSearch into Fuuka, Easymodo shut down in Oct 2011, with /a/, /jp/, /m/, and /tg/ archived. When Easymodo shut down, [https://archive.today/Ec1nf Eksopl made it's archives public in a torrent.] '''To whomever still has the Easymodo archive dumps: Please upload it to the Internet Archive. VoH, the admin of Nyafuu, supposedly has the data from the torrent, but it is in a hard drive in a currently inaccessible (to him) location. This will be updated with any further news/info.''' (Unfortunately, Eksopl no longer has it.) These archives were essential when Archive.moe accidentally lost it's thumbnails, and should not be lost ever again.

* [https://archive.today/Ec1nf Source: Easymodo Info Page]
* Eksopl gives [http://archiveteam.org/index.php?title=Talk:4chan#Eksopl.27s_Story_of_Fuuka_and_Easymodo a full history of Easymodo and the early days of the Fuuka Archiver here.]
* [https://twitter.com/MayhemYDG/status/565326134607609857 Mayhem] states that the reason the [https://archive.today/Ec1nf Easymodo Info Page] states for /a/: ''"Easymodo <- Green-Oval <- Easymodo"'' is because [https://archive.moe/a/search/text/easymodo/order/asc/ Easymodo came first], [https://archive.moe/a/search/text/%22green%20oval%20net%22/order/asc/ transferred it's /a/ archive] around 2010 to [https://github.com/MayhemYDG/4chan-x/commit/73dadbfe2718b62fa4ec539012f28b3bc925c509 Green-Oval later on], and [https://archive.moe/a/thread/51438731/#51439167 then had to take it back when Green-Oval shut down].
* Unfortunately, due to robots.txt, there are no Wayback Machine snapshots of Easymodo. If you are running an archive, please do not use robots.txt: don't commit digital suicide.

=== green-oval.net ===

'''Start Date:''' Feb 2010
'''End Date:''' Jul 2011?

Green-oval.net was a Fuuka archiver that used AoRF/Eksopl's source code to archive /tv/ and /g/. It later adopted /sci/. However, on June 2010, the old /a/rchive was straining Eksopl's servers, so he transferred /a/ to green-oval.net, a fellow archive originally built for /tv/ and /g/. When Green-oval started having troubles in July 2011, Easymodo took over it's /a/ archives. Installgentoo.net inherited it's /tv/ and /g/ archives, which are now under the care of RebeccaBlackTech.

* [https://web.archive.org/web/20110222001503/http://green-oval.net/cgi-board.pl Internet Archive - Green-oval.net]
* [https://web.archive.org/web/20110715235446/http://green-oval.net/cgi-board.pl/tv/? Green-oval.net hotlinked it's /a/ archive to Easymodo.]

=== Foolz Archive ===

{{Infobox project
| title = Foolz Archive
| image = aprilfoolz.png
| URL = [http://archive.foolz.us archive.foolz.us]
| project_status = {{Offline}}
| archiving_status = {{partial}}, Inherited by Archive.moe
| irc = ???
}}

When Easymodo announced that it's longtime /a/ archive would be shut down, '''Woxxy''' (part of the Foolz Scanlation Team) managed to obtain Easymodo's backups and continue where it left off. Later on, the FoolCode developers created, (and are still maintaining) **FoolFuuka**, a significantly improved version of the original Fuuka Archiver.

Foolz also assumed the boards formerly archived by The Dark Cave, InstallGentoo.net (/g/, /diy/, /sci/), and Deniable Plausibility (/v/, /vg/).

While Foolz.us was one of the first Fuuka Archivers to retain full-size images, it would periodically prune these images to save space.

On August 14, 2014, Foolz.us announced that [https://blog.foolz.us/2014/08/14/foolz-archives-farewell/ the service would shut down.] The entire archive was spun off and transferred to the newly-built [https://blog.foolz.us/2014/08/17/new-archive-owner-found/ Archive.moe.]

Unfortunately, a mishap occurred where most of the thumbnails obtained by Archive.moe were lost forever: By the time the staff noticed that the transfer failed, foolz.net was already deleted. ''(need more info on this)''

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/a/''' - Animu & Mango
| [https://archive.moe/a/search/order/asc/page/2/ 2008-02-03]
| '''archive.moe''' <- foolz.us <- easymodo.net <- green-oval.net
|-
| '''/biz/''' - Business and Finance
| [https://archive.moe/biz/search/order/asc/ 2010-10-12] (from birth)
| '''archive.moe''' <- foolz.us
|-
| '''/c/''' - Cute Animu
| [https://archive.moe/c/search/order/asc/ 2012-04-02]
| '''archive.moe''' <- foolz.us <- thedarkcave.org
|-
| '''/co/''' - Comics and Cartoons
| [https://archive.moe/co/search/order/asc/ 2012-05-21]
| '''archive.moe''' <- foolz.us
|-
| '''/diy/''' - Do It Yourself
| [https://archive.moe/diy/search/order/asc/ 2011-10-23]
| '''archive.moe''' <- foolz.us <- installgentoo.net
|-
| '''/gd/''' - Graphic Design
| [https://archive.moe/gd/search/order/asc/ 2014-07-12]
| '''archive.moe''' <- foolz.us
|-
| '''/int/''' - International
| [https://archive.moe/int/search/order/asc/ 2013-01-08]
| '''archive.moe''' <- foolz.us <- thedarkcave.org
|-
| '''/jp/''' - Otaku Culture
| [https://archive.moe/int/search/order/asc/ 2008-02-20] (from birth)
| '''archive.moe''' <- foolz.us <- easymodo.net
|-
| '''/m/''' - Mecha
| [https://archive.moe/m/search/order/asc/ 2009-03-27]
| '''archive.moe''' <- foolz.us <- easymodo.net
|-
| '''/mlp/''' - Pony
| [https://archive.moe/mlp/search/order/asc/ 2012-03-27] (from birth)
| '''archive.moe''' <- foolz.us
|-
| '''/out/''' - Outdoors
| [https://archive.moe/out/search/order/asc/ 2012-03-18] (from birth)
| '''archive.moe''' <- foolz.us <- thedarkcave.org
|-
| '''/po/''' - Papercraft and Origami
| [https://archive.moe/po/search/order/asc/ 2010-10-20]
| '''archive.moe''' <- foolz.us <- thedarkcave.org
|-
| '''/q/''' - 4chan Feedback
| [https://archive.moe/po/search/order/asc/ 2010-10-20] (from birth)
| '''archive.moe''' <- foolz.us (board closed 2013-09-18)
|-
| '''/sp/''' - Sports
| Around 2012-06-12?
| [https://twitter.com/ArchiveMoe/status/545305930582069249 ''abandoned''], dump at [https://archive.org/details/archive.moe-sp-archive-2014.12.16 Internet Archive] <- archive.moe <- foolz.us
|-
| '''/sci/''' - Science
| [https://archive.moe/sci/search/order/asc/ 2013-10-01]
| '''archive.moe''' <- foolz.us <- installgentoo.net <- easymodo.net <- green-oval.net + gentoomen
|-
| '''/tg/''' - Traditional Games
| [https://archive.moe/tg/search/order/asc/ 2010-02-23]
| '''archive.moe''' <- foolz.us <- easymodo.net
|-
| '''/tv/''' - Television and Film
| [https://archive.moe/tv/search/order/asc/ 2010-02-10]
| '''archive.moe''' <- foolz.us <- installgentoo.net <- green-oval.net + gentoomen
|-
| '''/v/''' - Video Games
| [https://archive.moe/vg/search/order/asc/ 2012-02-12]
| '''archive.moe''' <- vidya.moe <- foolz.us <- deniableplausibility.net
|-
| '''/vg/''' - Video Games Generals
| [https://archive.moe/vg/search/order/asc/ 2012-02-16] (from birth)
| '''archive.moe''' <- vidya.moe <- foolz.us <- deniableplausibility.net
|-
| '''/vp/''' - Pokemon
| [https://archive.moe/vp/search/order/asc/ 2013-03-13]
| '''archive.moe''' <- foolz.us
|-
| '''/vr/''' - Retro Games
| [https://archive.moe/vp/search/order/asc/ 2013-03-18] (from birth)
| '''archive.moe''' <- foolz.us
|-
| '''/wsg/''' - Worksafe GIF
| [https://archive.moe/wsg/search/order/asc/ 2012-06-05] (from birth)
| '''archive.moe''' <- foolz.us
|}

* [https://web.archive.org/web/20140816124831/https://archive.foolz.us/ Foolz.us - Final Snapshot before Shutdown]
* [https://github.com/bibanon/bibanon/wiki/4chan-History-Timeline#dates-of-board-additions Bibliotheca Anonoma - Board Addition Dates]
* [http://archive.easymodo.net/ Source: Easymodo Info Page]

== Closed Archives ==

4chan archives that have shut down, but either have dumps available or transferred their archives to other sites.

=== archive.installgentoo.com ===

Archived /g/ and /t/, started giving 403 errors in June 2014. No idea who has the data.

It was closed because of storage constraints.

=== FullFuuka ([http://4ch.be 4ch.be]) ===

This public site archives ''all 4chan boards'' with thumbnails only and publishes public dumps weekly to the Internet Archive.

Sadly 4ch.be has stopped archiving since 2016-02-27, the weekly dumps are still available on [https://archive.org/details/4ch.be archive.org].

=== cliché.net/4chan ===

{{Infobox project
| title = cliché.net/4chan
| image = Archiver.png
| URL = [https://www.cliché.net/4chan cliché.net/4chan]
| project_status = {{offline}}
| archiving_status = {{saved}} BibAnon has it, not yet uploaded.
| irc = ???
}}

Someone's past personal project. It was very slow, so any burst in traffic would've knocked the site offline, as it was the owner's personal computer. Images began to stop loading on the web view (although they were still downloaded), so that, along with the fact that the owner hadn't been actively working to remove illegal content, led to the owner removing the archive from public view.
<br><br>Nyafuu has imported all of its data as of 4/23/2016.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/e/''' - Ecchi
| [https://www.xn--clich-fsa.net/4chan/cgi-board.pl/e/?task=search2&ghost=yes&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2010-03-13]
| '''nyafuu.org <- ''' cliché.net/4chan
|}

=== Archive.moe ===

{{Infobox project
| title = Archive.moe
| image = archive-moe.png
| URL = [http://archive.moe archive.moe]
| project_status = {{offline}}
| archiving_status = {{partial}} (database up to 06-2015 uploaded, images coming soon)
| irc = ???
}}

Archive.moe was a union of archivists that inherited the boards of Archive.Foolz.us. 

Unfortunately, when it was founded and while Foolz was transferring data to them in 2014, [https://twitter.com/ArchiveMoe/status/512991440608043009 a mishap occurred] whereby the vast majority of thumbnails, let alone full images from before 2014, were lost. Some of /a/'s images were recovered using dumps from Easymodo, but the ramifications of this failed transfer have deeply negative effects for generations down the line.

They announced their shutdown on 2015-10-07, after a server outage wiped their database, with the admin believing he is no longer fit for the job.

A static version with thumbs (and some full images) can be viewed at [http://archive.fireden.net fireden.net].

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
! Thumbnails
! Oldest Full Image
|-
| '''/a/''' - Animu & Mango
| [https://archive.moe/a/search/order/asc/page/2/ 2008-02-03]
| '''archive.moe''' <- foolz.us <- easymodo.net <- green-oval.net
| {{Yes}}, Restored
| ???
|-
| '''/aco/''' - Adult Cartoons
| All text data lost
| '''archive.moe'''
| {{Yes}}
| {{Yes}}, All
|-
| '''/biz/''' - Business and Finance
| [https://archive.moe/biz/search/order/asc/ 2014-02-13] (from birth)
| '''archive.moe''' <- foolz.us
| {{Yes}}
| {{Yes}}, All
|-
| '''/c/''' - Cute Animu
| [https://archive.moe/c/search/order/asc/ 2012-04-02]
| '''archive.moe''' <- foolz.us <- thedarkcave.org
| {{Yes}}
| ???
|-
| '''/co/''' - Comics and Cartoons
| [https://archive.moe/co/search/order/asc/ 2012-05-21]
| '''archive.moe''' <- foolz.us
| {{Yes}}
| ???
|-
| '''/diy/''' - Do It Yourself
| [https://archive.moe/diy/search/order/asc/ 2011-10-23]
| '''archive.moe''' <- foolz.us <- installgentoo.net
| {{Yes}}
| ???
|-
| '''/g/''' - Technology
| [https://archive.moe/g/search/order/asc/ 2010-02-07]
| rbt.asia & archive.moe <- installgentoo.net
| rbt.asia preferred
| {{No}}
|-
| '''/gd/''' - Graphic Design
| [https://archive.moe/gd/search/order/asc/ 2013-03-18]
| '''archive.moe''' <- foolz.us
| style="background:#F99;vertical-align:middle;text-align:center;" | Lost before 2014
| ???
|-
| '''/h/''' Hentai
| [https://archive.moe/h/search/order/asc/ 2012-01-25]
| '''archive.moe''' <- foolz.us
| style="background:#F99;vertical-align:middle;text-align:center;" | Lost before 2014
| ???
|-
| '''/i/''' - Oekaki
| [https://archive.moe/i/search/order/asc/ 2011-11-05]
| '''archive.moe''' <- foolz.us
| {{Yes}}
| {{Yes}}, All
|-
| '''/int/''' - International
| [https://archive.moe/int/search/order/asc/ 2013-01-08]
| '''archive.moe''' <- foolz.us <- thedarkcave.org
| style="background:#F99;vertical-align:middle;text-align:center;" | Some Restored
| ???
|-
| '''/jp/''' - Otaku Culture
| [https://archive.moe/jp/search/order/asc/ 2008-02-20] (from birth)
| '''archive.moe''' <- foolz.us <- easymodo.net
| {{Yes}}
| ???
|-
| '''/k/''' - Weapons
| [https://archive.moe/k/search/order/asc/ 2012-07-13]
| '''archive.moe''' <- heinessen.com
| {{Yes}}
| ???
|-
| '''/m/''' - Mecha
| [https://archive.moe/m/search/order/asc/ 2009-03-27]
| '''archive.moe''' <- foolz.us <- easymodo.net
| style="background:#F99;vertical-align:middle;text-align:center;" | Some Restored
| ???
|-
| '''/mlp/''' - Pony
| [https://archive.moe/mlp/search/order/asc/ 2012-03-27] (from birth)
| '''archive.moe''' <- heinessen.com
| {{Yes}}
| [https://archive.org/details/heinessen-mlp-images Internet Archive]
|-
| '''/out/''' - Outdoors
| [https://archive.moe/out/search/order/asc/ 2013-03-18] (from birth)
| '''archive.moe''' <- foolz.us <- thedarkcave.org
| {{Yes}}
| ???
|-
| '''/po/''' - Papercraft and Origami
| [https://archive.moe/po/search/order/asc/ 2010-10-20]
| '''archive.moe''' <- foolz.us <- thedarkcave.org
| {{Yes}}
| {{Yes}}, All
|-
| '''/q/''' - 4chan Feedback
| [https://archive.moe/q/search/order/asc/ 2012-08-08] (from birth)
| '''archive.moe''' <- foolz.us (board closed 2013-09-18)
| style="background:#F99;vertical-align:middle;text-align:center;" | Some Restored
| ???
|-
| '''/qa/''' - Questions and Answers
| [https://archive.moe/qa/search/order/asc/ 2015-01-23] (from birth)
| '''archive.moe'''
| Partial?
| Partial
|-
| '''/r9k/''' - ROBOT 9001
| [https://archive.moe/r9k/search/order/asc/ 2012-06-02]
| '''archive.moe''' <- heinessen.com
| {{Yes}}
| ???
|-
| '''/s4s/''' - Shit 4chan Says
| [https://archive.moe/s4s/search/order/asc/ 2013-10-01]
| '''archive.moe''' <- (???)
| {{Yes}}
| {{Yes}}, All
|-
| '''/sci/''' - Science
| [https://archive.moe/sci/search/order/asc/ 2010-05-12]
| '''archive.moe''' <- foolz.us <- installgentoo.net <- green-oval.net/gentooman
| {{Yes}}
| ???
|-
| '''/tg/''' - Traditional Games
| [https://archive.moe/tg/search/order/asc/ 2010-02-23]
| '''archive.moe''' <- foolz.us <- easymodo.net
| {{Yes}}
| ???
|-
| '''/tv/''' - Television and Film
| [https://archive.moe/tv/search/order/asc/ 2010-02-01]
| '''archive.moe''' <- foolz.us <- installgentoo.net <- green-oval.net/gentooman
| style="background:#F99;vertical-align:middle;text-align:center;" | Some Restored
| ???
|-
| '''/u/''' - Yuri
| [https://archive.moe/u/search/order/asc/ 2011-06-04]
| '''archive.moe''' <- foolz.us
| style="background:#F99;vertical-align:middle;text-align:center;" | Lost before 2014
| ???
|-
| '''/v/''' - Video Games
| [https://archive.moe/v/search/order/asc/ 2012-02-12]
| '''archive.moe''' <- foolz.us
| style="background:#F99;vertical-align:middle;text-align:center;" | Lost before 2014
| Partial
|-
| '''/vg/''' - Video Games Generals
| [https://archive.moe/vg/search/order/asc/ 2012-02-16] (from birth)
| '''archive.moe''' <- foolz.us
| style="background:#F99;vertical-align:middle;text-align:center;" | Lost before 2014
|-
| '''/vp/''' - Pokemon
| [https://archive.moe/vp/search/order/asc/ 2013-03-13]
| '''archive.moe''' <- foolz.us
| {{Yes}}
| ???
|-
| '''/vr/''' - Retro Games
| [https://archive.moe/vr/search/order/asc/ 2013-03-18] (from birth)
| '''archive.moe''' <- foolz.us
| {{Yes}}
| ???
|-
| '''/wsg/''' - Worksafe GIF
| [https://archive.moe/wsg/search/order/asc/ 2012-06-04] (from birth)
| '''archive.moe''' <- foolz.us
| {{Yes}}
| ???
|}

* [https://web.archive.org/web/20140816124831/https://archive.foolz.us/ Foolz.us - Final Snapshot before Shutdown]
* [http://archiveteam.org/index.php?title=Talk:4chan#Primary_Source_from_a_FoolFuuka_Developer Primary Source: FoolCode Developer Adm|nymous]
* [https://web.archive.org/web/20140214074227/http://archive.thedarkcave.org/ Wayback Machine - The Dark Cave]
* [https://github.com/bibanon/bibanon/wiki/4chan-History-Timeline#dates-of-board-additions Bibliotheca Anonoma - Board Addition Dates]
* [http://archive.easymodo.net/ Source: Easymodo Info Page]

=== totally.not4plebs.org ===

{{Infobox project
| title = totally.not4plebs.org
| image = Not4plebs.png
| URL = [http://totally.not4plebs.org totally.not4plebs.org]
| project_status = {{offline}}
| archiving_status = {{saved}}
| irc = ???
}}

Status: <span style="color: green;">'''Online'''</span>
Saves Images?:<span style="color: green;">'''Yes'''</span>

A Fuuka archiver covering /sp/, picking up where archive.moe left off after the April Uprising. They have integrated the [https://archive.org/details/archive.moe-sp-archive-2014.12.16 Internet Archive] collection to kick off their archival efforts.

totally.not4plebs.org eventually merged it's /sp/ archive with 4plebs.org itself.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/sp/''' - Sports
| [http://totally.not4plebs.org/sp/search/order/asc 2012-06-11]
| '''4plebs.org''' <- not4plebs.org <- (late 2014 threads lost) <- archive.moe
|}

===4archive===
{{Infobox project
| title = 4archive
| image = 4archive.png
| URL = [http://4archive.org 4archive.org]
| project_status = {{offline}}
| archiving_status = {{saved}}
| irc = ???
}}

Another site that saves threads on a unique platform, starting at January 17 2014. This site is notable as it was the only site archiving /b/ until 2015. Images are stored separately through Imgur and Imageshack.

Unfortunately, this site shut down on May 7, 2015. The admin provided a MySQL Dump, which the [[Bibliotheca Anonoma]] mirrored to the Internet Archive here:

* [Internet Archive - 4Archive SQL Dump](http://archive.org/details/4archive)

=== installgentoo.net ===

{{Infobox project
| title = installgentoo.net
| image = installgentoo.png
| URL = [https://web.archive.org/web/20130204001648/http://archive.installgentoo.net/ archive.installgentoo.net]
| project_status = {{Offline}}
| archiving_status = Inherited by rbt.asia, Archive.moe, and warosu.org
| irc = ???
}}

Status: <span style="color: blue;">'''Transferred'''</span>
Saves Images?: <span style="color: red;">'''Partially'''</span>

Start Date: 2011-10-??
End Date: 2014-02-??

Archived /diy/, /g/, /sci/ throughout it's lifetime. All boards were inherited from Green-Oval and Gentoomen.

It also apparently ran /pol/ for some time, according to this link: https://warosu.org/jp/thread/S8052074#p8055433

It shut down around Feb. 2014 due to hosting problems, but thankfully dumps of all boards were made public and were inherited by rbt.asia, Foolz.us (now Archive.moe), and warosu.org.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/diy/''' - Do It Yourself
| [https://archive.moe/diy/search/order/asc/ 2011-10-23]
| '''archive.moe''' <- foolz.us <- installgentoo.net
|-
| '''/g/''' - Technology
| [https://rbt.asia/g/?task=search2&ghost=&search_text=&search_subject=&search_username=&search_tripcode=&search_email=&search_filename=&search_datefrom=&search_dateto=&search_media_hash=&search_op=all&search_del=dontcare&search_int=dontcare&search_ord=old&search_capcode=all&search_res=post 2011-11-11]
| '''rbt.asia''' <- installgentoo.net <- gentoomen.org <- green-oval.net
|-
| '''/sci/''' - Science
| [https://archive.moe/sci/search/order/asc/ 2010-05-12]
| '''archive.moe''' <- foolz.us <- installgentoo.net <- gentoomen.org <- green-oval.net
|-
|}

* [http://archiveteam.org/index.php?title=Talk:4chan#Primary_Source_from_a_FoolFuuka_Developer Primary Source: FoolCode Developer Adm|nymous]
* [https://web.archive.org/web/20130204001648/http://archive.installgentoo.net/ Internet Archive - installgentoo.net]
* [https://archive.today/Ec1nf Source: Easymodo Info Page]

=== archive.mawa.re === 

Status: <span style="color: blue;">'''Transferred'''</span>
Archived?: <span style="color: red;">'''Yes'''</span> (by loveisover.me)

Start Date: [https://archive.loveisover.me/t/thread/522650/#585860 2014-01-19]
End Date: [https://github.com/MayhemYDG/archives.json/commit/65eeac16d7e9ccd09e16f17e3829f6e42248b55b 2013-09-07]

Archived /t/. It was shut down by it's owner, but the backups were transferred to loveisover.me.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/t/''' - Torrents
| [http://archive.loveisover.me/t/search/order/asc/ 2012-06-08]
| '''loveisover.me''' <- mawa.re
|}

=== archive.heinessen.com ===
Status: <span style="color: blue;">'''Some Lost, Some Transferred'''</span>
Saves Images?: <span style="color: red;">'''Partially'''</span> (all boards except /mlp/ and /x/)

Archived /an/, /fit/, /k/, /mlp/, /r9k/, /toy/, /x/. Also used the alternate domains archive.maidlab.jp and xfiles.to .

Closed on November 2014 due to personal reasons, but the /r9k/, /mlp/, and /k/ archives were made public. The /fit/ archive was privately released to '''imcute.yt''' and other undisclosed individuals.

Unfortunately, the admin decided to delete the /an/, /toy/, and /x/ archives without providing backups. These archives date all the way back to 2012.

* imcute.yt inherits all the boards that Heinessen archives, (except for /k/ and /x/), but only inherited history for /fit/ and /mlp/. 
* 4plebs.net did not inherit it's /x/ archive, but their own archive dates back to 2013.
* Archive.moe inherited the Heinessen /k/ archive. They also made public [https://archive.org/details/heinessen-mlp-images Heinessen's 282GB archive of all full-size images from /mlp/], which was then uploaded to the Internet Archive.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/an/''' - Animals & Nature
| (2012?) Lost
| X- heinessen.com (not backed up)
|-
| '''/fit/''' - Fitness
| [http://imcute.yt/fit/search/order/asc/ 2010-10-12]
| '''imcute.yt''' <- heinessen.com
|-
| '''/gif/''' - Adult GIF
| (2012?) Lost
| X- heinessen.com (not backed up)
|-
| '''/int/''' - International
| (2012?) Lost
| X- heinessen.com (not backed up)
|-
| '''/k/''' - Weapons
| [https://archive.moe/k/search/order/asc/ 2012-07-13]
| '''archive.moe''' <- heinessen.com
|-
| '''/mlp/''' - Ponies
| [http://imcute.yt/mlp/search/order/asc/ 2012-08-08]
| '''archive.moe''' & '''imcute.yt''' <- heinessen.com
|-
| '''/r9k/''' - ROBOT9000
| [http://imcute.yt/r9k/search/order/asc/ 2014-11-10]
| '''archive.moe''' <- heinessen.com
|-
| '''/toy/''' - Toys
| (2012?) Lost
| X- heinessen.com (not backed up)
|}

----

*[https://archive.org/details/archive.heinessen.com-torrent Archive.org Torrent Dump] - The owner offered [http://archive.heinessen.com/heinessen.torrent a torrent dump] of /r9k/ /k/ and /mlp/ temporarily, covering SQL dumps and thumbnails. It is now permanently archived at Archive.org. It's 38.9GB so watch out.
*[https://archive.org/details/heinessen-mlp-images Archive.moe's /mlp/ Full Image Archive from Heinessen] - A 282GB archive of all full-size images from /mlp/, provided by Archive.moe before they expunged them.
* [http://ar.vyrd.net/ Source: ar.vyrd.net]

=== vidya.moe ===

Status: <span style="color: blue;">'''Transferred'''</span>

A short-lived archive for /v/ and /vg/. Shortly before it was shutdown it was revealed that [https://web.archive.org/web/20140816124824/https://blog.foolz.us/2014/08/15/our-secret-vidya-moe/ it was actually run by Foolz Archive], launched after they found a way to continue offering public access to /v/'s archive, and run from a different domain due to fears that Foolz's userbase would react negatively to the archive being re-enabled. All of its content was transferred with the rest of Foolz's data to archive.moe.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/v/''' - Video Games
| [https://archive.moe/vg/search/order/asc/ 2012-02-12]
| '''archive.moe''' <- vidya.moe <- foolz.us <- deniableplausibility.net
|-
| '''/vg/''' - Video Games Generals
| [https://archive.moe/vg/search/order/asc/ 2012-02-16] (from birth)
| '''archive.moe''' <- vidya.moe <- foolz.us <- deniableplausibility.net
|-
|}

=== archive.thedarkcave.org ===

Status: <span style="color: blue;">'''Transferred'''</span>

An archiver for /c/, /int/, /out/ (since birth), and /po/. All archives were transferred safely to Foolz in [http://archiveteam.org/index.php?title=Talk:4chan#archive.thedarkcave.org June 2014.]

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/c/''' - Cute Animu
| [https://archive.moe/c/search/order/asc/ 2012-04-02]
| '''archive.moe''' <- foolz.us <- thedarkcave.org
|-
| '''/int/''' - International
| [https://archive.moe/int/search/order/asc/ 2013-01-08]
| '''archive.moe''' <- foolz.us <- thedarkcave.org
|-
| '''/out/''' - Outdoors
| [https://archive.moe/out/search/order/asc/ 2012-03-18] (from birth)
| '''archive.moe''' <- foolz.us <- thedarkcave.org
|-
| '''/po/''' - Papercraft and Origami
| [https://archive.moe/po/search/order/asc/ 2010-10-20]
| '''archive.moe''' <- foolz.us <- thedarkcave.org
|}

* [https://web.archive.org/web/20140214074227/http://archive.thedarkcave.org/ Wayback Machine - The Dark Cave]

===  boards.deniableplausibility.net ===

An archiver for /v/ and /vg/. It may have started and suddenly stopped sometime in Summer 2014. 

Foolz already archived the same date range, so nothing of value was lost. Though it would be nice if someone had the archives from this site, it could be used to restore /v/ and /vg/ thumbnails on Archive.moe.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/v/''' - Video Games
| (guess) A few days (1-3) prior to 6/22/14
| deniableplausibility.net
|-
| '''/vg/''' - Video Games Generals
| (guess) Around 7/4/14
| deniableplausibility.net
|}

* [https://web.archive.org/web/20140625165901/http://boards.deniableplausibility.net/ Wayback Machine - DeniablePlausibility]

== Lost Archives ==

Archives of which there are no backups of, and only a few web scrapes from the Internet Archive.

=== fgts.jp ===

{{Infobox project
| title = fgts.jp
| image = fgts-jp.png
| URL = [https://fgts.jp fgts.jp]
| project_status = {{offline}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

Status: <span style="color: red;">'''Offline'''</span>
Saves Images?: <span style="color: green;">'''Yes'''</span>

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
|-
| '''/asp/''' - Alternative Sports
| [https://fgts.jp/asp/search/order/asc/ 2015-04-18]
|-
| '''/b/''' - Random
| [https://fgts.jp/b/search/order/asc/ 2015-04-18]
|-
| '''/cm/''' - Cute/Male
| [https://fgts.jp/cm/search/order/asc/ 2015-04-18]
|-
|'''/gd/''' - Graphic Design
|[https://fgts.jp/gd/search/order/asc/ 2015-05-07]
|-
| '''/h/''' - Hentai
| [https://fgts.jp/h/search/order/asc/ 2015-04-18]
|-
| '''/hc/''' - Hardcore
| [https://fgts.jp/hc/search/order/asc/ 2015-04-18]
|-
| '''/hm/''' - Handsome Men
| [https://fgts.jp/hm/search/order/asc/ 2015-04-18]
|-
| '''/n/''' - Transportation
| [https://fgts.jp/n/search/order/asc/ 2015-04-18]
|-
|'''/out/''' - Outdoors
|[http://fgts.jp/out/search/order/asc/ 2015-08-06]
|-
| '''/p/''' - Photography
| [https://fgts.jp/p/search/order/asc/ 2015-04-18]
|-
|'''/po/''' - Papercraft & Oragami
|[http://fgts.jp/po/search/order/asc/ 2014-08-13]
|-
| '''/qa/''' - Question & Answer    
| [https://fgts.jp/qa/search/order/asc/ 2015-04-18]
|-
| '''/r/''' - Adult Requests
| [https://fgts.jp/r/search/order/asc/ 2015-04-18]
|-
|'''/s/''' - Sexy Beautiful Women
|[http://fgts.jp/s/search/order/asc/ 2015-03-02]
|-
| '''/soc/''' - Cams & Meetups
| [https://fgts.jp/soc/search/order/asc/ 2015-04-18]
|-
| '''/toy/''' - Toys
| [https://fgts.jp/toy/search/order/asc/ 2015-04-18]
|-
| '''/vp/''' - Pokémon
| [https://fgts.jp/vp/search/order/asc/ 2015-10-07]
|-
| '''/y/''' - Yaoi
| [https://fgts.jp/y/search/order/asc/ 2015-04-18]
|}

fgts.jp suffered an irrecoverable hard drive crash in April 2015, causing all data archived before then to be lost. On the flip side, it will be importing Archive.moe's /vp/ archive.

At 11:08 AM EST, Bui closed fgts.jp. Read the full message here: https://archive.is/78Buf https://i.imgur.com/XH7AUKU.png

=== 4zip ===

{{Infobox project
| title = 4zip
| image = 4archive.png
| URL = [http://4zip.org 4zip.org]
| project_status = {{offline}}
| archiving_status = {{notsaved}}
| irc = ???
}}

A site that saves threads using the shiny new [https://github.com/4archive/4archive 4archive Lumen framework], starting in mid-2015. This site is notable as users submit threads to archive, and full size images are stored separately through Imgur and Imageshack.

Unfortunately, it shut down sometime between October 2015 and January 2016, and there are no backups. There are some threads scraped on the Internet Archive.

* [http://web.archive.org/web/*/http://4zip.org/* Internet Archive - 4zip.org Snapshots] - Some scrapes by the Internet Archive on 4zip.org.
* [http://web.archive.org/web/20151009220014/http://4zip.org/v/thread/312351215 4zip.org - /v/ Archive.moe shutdown thread]

=== imcute.yt ===

{{Infobox project
| title = imcute.yt
| image = imcute-yt.png
| URL = [http://imcute.yt imcute.yt]
| project_status = {{Offline}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

Status: <span style="color: red;">'''Offline'''</span>
Saves Images?:<span style="color: green;">'''Yes'''</span>

A Fuuka archiver that started with /gif/, /int/, /jp/, /out/, presumably around 2014-08-09.

It's resumed archiving all boards originally covered by Heinessen (/an/, /fit/, /gif/, /mlp/, /r9k/, /sp/, /toy/) except /k/ and /x/. Unfortunately, only /fit/ and /mlp/ contain Heinessen's full archival history prior to 2014, since the rest were not backed up. (though Heinessen's /r9k/ history was inherited by Archive.moe).

It used to archive /sp/, but stopped in the aftermath of the /sp/ April Uprising.

The owner, tali, abandoned archival and did not provide backups before deleting all data. What a tragedy.

{| class="wikitable sortable"
! Board
! Date of Oldest Thread
! Pedigree
|-
| '''/an/''' - Animals & Nature
| [http://imcute.yt/an/search/order/asc/ 2014-10-15]
| '''imcute.yt'''
|-
| '''/fit/''' - Fitness
| [http://imcute.yt/fit/search/order/asc/ 2010-10-12]
| '''imcute.yt''' <- heinessen.com
|-
| '''/gif/''' - Adult GIF
| [http://imcute.yt/gif/search/order/asc/ 2014-08-09]
| '''imcute.yt'''
|-
| '''/int/''' - International
| [http://imcute.yt/int/search/order/asc/ 2014-10-18]
| '''imcute.yt'''
|-
| '''/mlp/''' - Ponies
| [http://imcute.yt/mlp/search/order/asc/ 2012-08-08]
| '''imcute.yt''' <- heinessen.com
|-
| '''/out/''' - Outdoor
| [http://imcute.yt/out/search/order/asc/ 2014-07-12] (from birth)
| '''imcute.yt'''
|-
| '''/qa/''' Q & A
| [http://imcute.yt/qa/search/order/asc/ 2015-01-23] (from birth)
| '''imcute.yt'''
|-
| '''/r9k/''' - ROBOT9000
| [http://imcute.yt/r9k/search/order/asc/ 2014-11-10]
| '''imcute.yt'''
|-
| '''/toy/''' - Toys
| [http://imcute.yt/toy/search/order/asc/ 2014-07-12]
| '''imcute.yt'''
|}

=== WorldAthleticProject ===

Status: <span style="color: red;">'''Offline'''</span>
Archived?: <span style="color: red;">'''No'''</span>

Start Date: (sometime before Aug. 22 2013)
End Date: [https://github.com/MayhemYDG/4chan-x/commit/4dc8d013f3883e1bf854bd507471436068e90af7 2013-10-23]

'''WorldAthleticProject''' was an archiver for the boards /cm/, /s/, /con/, /e/, /h/, /hc/, /soc/, /s4s/, /d/, /pol/, /adv/, /trv/, /lgbt/, /r/, /u/, and /y/.

This archiver also attempted to make a Fuuka vertabrim archive of /b/. Unfortunately, given that /b/tards are a feisty bunch and post CP from time to time (and deletions are difficult to transfer to the archiver), despite having a decent report system, the owner probably wiped all data in a panic when the partyvan came to his door.

Apparently reports aren't enough, you need to log users as well, as fgts,jp will tell you [https://fgts.jp/_/articles/b/ in their archive.]

This is the most significant loss of data since the Chanarchive. We need to catalog what was lost (check archival start dates), and possibly recover some bits via Internet Archeology on the Wayback Machine.

* [http://archive.today/PH7Rk Archive.today - Snapshot of /s4s/ 2013-10-18]
* [https://web.archive.org/web/20130822093339/http://fuuka.worldathleticproject.org/ Wayback Machine - http://fuuka.worldathleticproject.org]
** [https://web.archive.org/web/*/http://fuuka.worldathleticproject.org/b/thread/* Wayback Machine - 68 Surviving Threads from 2013's /b/]
** [https://web.archive.org/web/20130927131643/http://fuuka.worldathleticproject.org/soc/ Wayback Machine - Single Page Snapshot of /soc/ 2013-10-18]

=== nth.pensivenonsen.se ===

Status: <span style="color: red;">'''Offline'''</span>
Archived?: <span style="color: red;">'''No'''</span>

Start Date: May 10, 2013
End Date: Jun 16 2013

This archive was built by an anon after Foolz stopped archiving /vg/ for a few months. He obtained the backups of /vg/ from Foolz and rehosted it on his own server. However, he had inadequate hardware for the large amount of traffic, search didn't always work, and eventually when Foolz gained better infrastructure, they were able to start archiving /vg/ again, so this archive closed.

It is unknown whether the data gathered here was transferred to Foolz, or simply lost.

* [https://web.archive.org/web/20130622041116/http://nth.pensivenonsen.se/meta/ Internet Archive - nth.pensivenonsen.se/meta]
* [https://web.archive.org/web/20130622063316/http://nth.pensivenonsen.se/meta/thread/120/#q120 Internet Archive - Admin's Announcement of Handover]

=== Foolzashit ===

Status: <span style="color: red;">'''Offline'''</span> 

Start Date: (before June 2013)
End Date: (around Nov. 2013)

Foolzashit was an archiver for /adv/, /asp/, /cm/, /e/, /i/, /lgbt/, /n/, /o/, /p/, /s/, /s4s/ (since it's inception), /t/, /trv/, /y/ .

Unfortunately, it was lost in it's entirety and backups were not made, so all /s4s/ posts predating Nov. 2013 (when 4plebs.org began archiving) are lost.

* [https://archive.today/archive.foolzashit.com Archive.today - archive.foolzashit.com Snapshots]
* [https://web.archive.org/web/20131015052010/http://archive.foolzashit.com/ Wayback Machine - Foolzashit Snapshots]
** [https://web.archive.org/web/20130815041545/http://archive.foolzashit.com/s4s/ Wayback Machine - One Page Snapshot of /s4s/]
** [https://web.archive.org/web/*/https://archive.foolzashit.com/s4s/thread/* Wayback Machine - 3 Complete /s4s/ Threads]

=== Chanarchive ===

{{Infobox project
| title = Chanarchive (formerly 4chanarchive)
| image = chanarchive.png
| URL = [http://chanarchive.org Chanarchive.org], formerly [http://4chanarchive.org 4chanarchive.org]
| project_status = {{offline}}
| archiving_status = {{nosavedyet}}
| irc = ???
}}

4chan's primary archive site. Since 2006, significant 4chan threads have been archived on the 4chanarchive, creating a database of over 500GBs.

On 10/3/2012, Chanarchive without warning, temporarily shut down (almost permanently though.) On a 4chan thread, the owner stated that the site was banned from paypal and had their funds frozen, making it impossible to pay it's massive expenses. However, the operators of [[Encyclopedia Dramatica]]  stepped in, and offered to host chanarchive.org, which was accepted by the site's creator/then-owner, "Capsized." 

<s>The site is still online as of 2/26/13, but no backups have been made as of yet.</s> As of 1/16/14 the site is down and ED has given no indication to it returning. Internet Archive has intermittent captures of the site.

[https://encyclopediadramatica.es/Chanarchive#Death_of_Chanarchive Zaiger, one former mod, stated] that a hard drive containing parts of the site got corrupted, and was irreparable. The Chanarchive Team was thus unable to restore the site, or even a backup.

The Bibliotheca Anonoma is attempting to resurrect some portions of the site through Internet Archeology, by [https://github.com/bibanon/bibanon/wiki/Chanarchive sifting through the Wayback Machine's many snapshots of 4chanarchive/Chanarchive.] Not everything will be saved, and images are mostly lost, but a significant portion of the threads can at least be read.

{{Navigation box}}
