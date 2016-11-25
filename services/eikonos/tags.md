Types
=====

Danbooru and Yande.re follow very structured tag systems that enforce a quality set of tags on their image uploads. This makes it easy to find images that people can think of.

Universal Tags
------------------

### Metadata

* Title - The name of the image.
* Filename - The filename of the image.
* Date - The time the image was posted to 4chan or uploaded.
* MD5Sum  - The md5 hash of the image.
* Origin - The original site where the image came from, if any.

### Categories

Tags also are sorted into one of 4 types on Moebooru. We've modified them to fit our needs in `config/init_config.rb` and `config/local_config.rb`.

* (0) **General** - All tags not sorted into other sections. 
* (1) **Community** - Website, online culture, or online community where the content originated. **This tag type (1) is special among all** because it can be set up to detect URLs that fit certain criteria ([originally designed to detect artists](https://yande.re/help/artists)), and can have "members" (which we use for community subsections).
  * **Examples** - e.g. 4chan, 8chan, Something Awful, 2channel, Reddit, Tumblr.
  * **Members**/subsections - Communities can have "members", which encompasses subsections of these websites, such as 4chan's /b/, /a/, /pol/, 8chan's /v/. Or subreddits. Just specify these in the Members field
  * **Danbooru Name** - Artist: The person who actually drew the work of art. The Members section was originally designed to represent doujin circles made up of multiple artists.
* (3) **Contributor** - The original website, location, or contributor of the content in particular. Content often gets spread all around the internet and is often lost to its original community, surviving only in memory on the rest of the internet or in private collections. 
  * **Examples** - Sources can be content aggregators (Reddit, Tumblr, Funnyjunk), blogs/personal websites, or even the people who contributed the data to the Bibliotheca Anonoma.
  * **Danbooru Name** - Copyright: From which anime/tv show/manga/game.
* (4) **Category** - What type of content does this represent? Is there a greater subculture or genre that it falls under?
  * * **Examples** - Subcultures such as Anime, Vaporwave, Touhou. Also story genres such as feels/baww, walk_the_dinosaur, Greentext. There could also be movements such as /b/day, Chanology.
  * **Danbooru Name** - Character: A character in the series.
* (5) **Author** - If applicable, the author of a work could be attributed. Usually this might not be used as 4chan is anonymous, but prominent anons do pop up from time to time.

Pools
=====

Danbooru implemented Pools to group together related images, such as Touhou or Kancolle, or manga and doujins, so that they wouldn't be separated and would be easier for people to browse through. These can be useful for various purposes.

## Types of Pools

* **Album** - A group of photos that are related by virtue of being collected and graciously donated by an anon. They are named and have a short wiki description of their contents.
* **Meme** - A group of photos that are related to a certain major meme.

Reaction Images
---------------------

Reaction Images are anything used by 4chan in lieu of words. Because a picture is a thousand words. Reaction images should have tags describing what feeling it describes. May cross over with the meme tags when reaction images are derivatives of a well-known meme

Memes
---------

Memes are remixable, evolvable, and propogatable ideas or inside jokes that get across the Internet. 
One base meme is often used to derive many other memes. The "source material" tag category should be replaced with one denoting which memes a image is derived from, or which ones it contains

Screencaps
---------------

Screencaps will need to be processed with OCR. We could even set up Google Custom Search or our own Sphinx server.

### Stories

Stories should have a story tag, and possibly a multi-thread post tag. Multiple screencap images should be put in a pool. Possibly add some small tags specifically made for that particular story so that people can find it more easily.

### Greentext

Greentext stories, along with whatever replies there are, should have a dedicated viewer. 

Charts and Infographics
----------------------

4chan is famed for it's charts and tier lists.

* /g/ tech lists
* /mu/ album lists
* /a/ anime lists
* /v/ tier lists.

How Tagging Works
=================

There are a lot of things to learn about tagging from the original sites the engine was made for. Really think about why the tagging system was invented, and how quality is maintained to ensure that people are able to find the obscure things they want without knowing a single word of Japanese.

## Guidelines

These are rulebooks that set how users should tag their photos. They're quite dense, but the purpose is to make sure that photos can be easily rediscovered by other users.

* [Danbooru Wiki]()
  * [Guidelines](https://danbooru.donmai.us/wiki_pages/43043)
  * [How to Upload](https://danbooru.donmai.us/wiki_pages/10933)
* [Gelbooru Wiki]()
  * [Help](http://www.gelbooru.com/index.php?page=help&topic=post)
  * [How to Upload](http://www.gelbooru.com/index.php?page=wiki&s=view&id=6645)
  * [How to Tag](http://gelbooru.com/index.php?page=wiki&s=view&id=2533)
  * [Tag Checklist](http://gelbooru.com/index.php?page=wiki&s=view&id=16877) - What NOT to tag.
* [Yandere](https://yande.re/wiki/show?title=help%3Ahome)
  * [Cheatsheet](https://yande.re/help/cheatsheet)
* [Konachan](https://konachan.com)
  * [Moebooru Help](http://konachan.com/help/)

## Pools and Inheritance

Danbooru uses Pools and Inheritance to gather related images together. E.g. a manga, or webcomics, or remixed memes. These are accomplished through metatags.

## Metadata

* Copyright - Tells you what work it came from. E.g. kancolle
* Character - Tells you what characters are featured.
* Author - Tells you who made it.

## Descriptive

* blonde/brunette/ - Describes aspects of a certain character depicted in the work.
* multiple_girls - Arithmetic facts about the image.

## Situational

*  - What is apparently going on in the picture?
* Dutch Angle - How is the picture presented?
* Ukiyo-e/Watercolor - How was the picture made?