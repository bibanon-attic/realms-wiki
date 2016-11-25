
[Eikonos](http://booru.eikonos.org) is an Image Tag Database devoted to archiving and organizing screencaps and memetic images from around the internet. There is a special focus on 4chan, Something Awful, and 2channel.

## Sections

* [Staff](/services/eikonos/staff) - Staff managing and obtaining images for Eikonos.
* [Tag Structure](/services/eikonos/tags) - Moebooru comes with tag collections designed for the organization of anime images. We need to modify this to suit our needs.
* [Engines](/services/eikonos/engines) - The various danbooru-style image tag databases to choose from.
  * [Moebooru](/services/moebooru) - How we set up our production version of the Moebooru Image Tag Engine, and how you can too.
* [Logo](/services/eikonos/logo) - The Logo of Eikonos.

## Using Eikonos

### Wiki

The Wiki on Eikonos uses Textile. If you're unfamiliar with the language, just use pandoc or something to convert Markdown to Textile. 

It's not the best wiki ever, but it's designed to work to provide a description for the tags/collections. Stick to the BA Wiki here for deeper articles.

### Apps

To have a better experience on mobile, pick up these third-party apps (which make use of the API):

* iPhone
  * [Mignori](http://www.mignori.com) - An excellent app that allows you to favorite posts on your phone and sort them into tagged collections, without having to download them.
  * [Anime Boxes](https://itunes.apple.com/us/app/anime-boxes/id525540312?mt=8)
* Android
  * [Nori](https://github.com/tjg1/nori) - [Download](https://github.com/tjg1/nori/releases) - It's no longer on Google Play, but it works and is open source.
  * [Crumby](http://www.getcrumby.com/tagged/crumbyapp) - Old, but still works fine for everything other than Gelbooru. I need to repost the app here.

### API

> **Note:** The hash-string for Eikonos is `john-freeman`, used to encrypt requests sent to the server.

Eikonos uses the Moebooru engine, which is compatible with the Danbooru API. Check out [the API documentation here.](http://booru.eikonos.org/help/api)

* Python
  * [pybooru](https://github.com/LuqueDaniel/pybooru/) - A great library you can use to mass upload if you have tons of tags to link with images.

```
from pybooru import Pybooru

client = Pybooru(site_url='http://booru.eikonos.org', username='your-username', password='your-password', hash_string='john-freeman--{0}--')

client.comments_create(post_id=id, comment_body='Comment content')
```