## Wikilinks

Realms uses a special type of wikilink, which needs to be converted from Gollum's [[wikilink syntax]].

### Requirements

* Wikilinks must be all in lowercase, and spaces replaced with `-`.
  * `[Wiki Article](/wiki-article)`

## Stories

* Stories must be under the stories subfolder. If a story has multiple pages, it must follow the formats below:
  * `[Damaged Goods](/stories/damaged-goods)` - The index page of the story "[Damaged Goods](/stories/damaged-goods)".
  * `[Damaged Goods Chapter 1](/stories/damaged-goods/1)` - The first chapeter of the story "Damaged Goods".

### Page Navigation

At the bottom of every page, there should be a navigation table with the following specs:

* top bar is a link to the story
* left column is previous page, middle column is current page, right column is next page

We need to design one in HTML.