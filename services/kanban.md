Kanban Methodology
------------------

> _The term Kanban (看板) refers to the Japanese word for a signboard._

The [Kanban](http://leankit.com/learn/kanban/kanban-board/) Methodology was developed as part of the [Toyota Production System](https://en.wikipedia.org/wiki/Toyota_Production_System): to ensure efficiency on the production line, discover bottlenecks in the supply chain, and avoid accumulating excess inventory.

Traditionally, a Kanban board is presented with sticky notes organized into sequential sections on a tackboard: for example, To Do, Doing, and Done. 

In the digital age, online collaborative tools such as [Trello](http://trello.com) have been constructed to assist software development across the Internet.

## Ideals

* **Boards should have a single project or goal in mind.** - The board should reflect the team that is assigned to use it.
* **Cards should be dynamic, not static content.** - If the card provides useful information, that information should be put into the wiki, not left on the board.
* **Each card should be assigned to a team member and monitored by a group leader.** - A card needs to be taken on by someone once it enters the Doing list, and they would take responsibility for completing it b a certain

## Current Use by the Bibliotheca Anonoma

Trello is currently a central component of the Bibliotheca Anonoma's workflow, but it is not currently being used to full effectiveness.

### Problems

* **A Kanban Board is not a Wiki!** - A kanban board is meant to hold dynamic cards that move around in the course of a day. Once cards start piling up, the lists become unreadable and unusable.
  * Due to the ineffectiveness of Github Gollum, the Bibliotheca Anonoma began to use Trello as a static information repository beginning in 2015.
  * While this was very effective for sequential timelines with image cards: [Fansub Evolution](https://trello.com/b/s3eNd4zD/fansub-evolution), the cards could not simply be archived out of view, and started to stagnate or clog the board.
* **Cards need to be assigned to team members and given Deadlines.**
  * While we all have a life, we are all able to squeeze out a bit of free time in a week. Also, sometimes people are in want of tasks, but it's not clear what needs to be done when.
  * There needs to be a person in charge of reminding people whether tasks were missed, and pushing back deadlines or reassigning tasks if necessary.
* **Tasks assigned to a user should be clearer.** - There needs to be some sort of way to see all the cards currently assigned to a user, and when deadlines are coming up.
  * Trello has a calendar sync system, which can be integrated to Sunset.

## Board Redevelopment

Bulleted lists are the boards to keep, subbullets are the ones to merge in.

* [Content to Import](https://trello.com/b/ohziwjHI/content-to-import) - Incoming data that needs to be processed into wikipages. This board should encompass all data worth writing about, not just stories. So instead of having separate boards, we should have tags denoting which type the card falls under (Stories, Art, Video, etc.)
  * [Internet Folklife](https://trello.com/b/Wk718GRA/internet-folklife) - Should be folded into Content to Import, but remain as a tag to attach to cards.
  * [Field Research](https://trello.com/b/HMb078yD/field-research) - Should be folded into Content to Import.
  * Genmaicha Web Scraping - Developed as a board to take request for the IRC interface to grab-site, which never got developed. Instead of doing this, assign any cards to archive to Gazlene.
* [Imageboard Archival](https://trello.com/b/z7oL1zWA/imageboard-archival) - A board that differs from the Content to Import board in that it holds collections of 4chan/imageboard data to archive. Maybe we can upload to the Internet Archive, blog about the data we've obtained, and then archive the card.
  * Any stagnant historical info cards here should be divested to the wiki.
* [Art and Compositions](https://trello.com/b/GO8xe3Wt/art-and-compositions) - A board that would differ from the Content to Import board in that the data should end up in our Image Tagging System, Eikonos (Moebooru has it's own wiki system for tags as well).
  * [Eikonos](https://trello.com/b/TOGpQZ9I/eikonos-image-tag-database) - A board that was also designed for importing data into the tagging system.

### Stagnant Content Boards

These boards contain cards with information of interest that are better off as real articles on the wiki.

* [Bibliotheca Anonoma General](https://trello.com/b/fOH2RCCu/bibliotheca-anonoma-general) - Really more of a board talking about the organization itself and the ideas we have: but that's what our wiki should have been doing in the first place.
* [Community Outreach](https://trello.com/b/Jmdrrs10/community-outreach) - More of a set of ideas about how to connect with the community, which is better outlined on a real page.
* [Design and Development](https://trello.com/b/PvSUmv84/design-and-development-basc) - Ideas and proposals for the organization, which probably should be built as wikipages first, then given active Kanban cards when we are actually doing them.
* [Imageboard Archive and Links Repository](https://trello.com/b/zlMpLGFI/imageboards-archive-links-repository) - Any sort of link repository should go on the wiki. This board was designed to keeping away stagnant cards from the Imageboards Archive board.

### Presentation Boards

Trello actually works great for presenting timelines or presentations.

* Timelines - Sequential lists denoting a certain slice of time, and cards explaining specific events within.
  * [Fansub Evolution](https://trello.com/b/s3eNd4zD/fansub-evolution) - A timeline of the entrance and exit of various English-language fansub groups.
* Presentations - It is also nice to view as a visual chart of various items and perhaps further details about them.
  * [Global Internet Folklife](https://trello.com/b/EHxRdvEG/global-internet-folklife) - Actually quite a nice presentation of various non-English Internet systems. Long rambling cards should be built into real wikipages though.
  * [Museum](https://trello.com/b/DI4Lt6Iy/museum) - A literal museum of all the physical things I've collected.

## Future Usage

### Problems with Trello

* Trello is quite a nice freeform kanban board system, but maybe it's got a little too much freedom and lacks structure.
* Trello doesn't really show what tasks a single user would have. It does have a calendar feature which can be synced to Google Calendar though.

### Alternatives to Trello

* Wekan (formerly Libreboard) - This is a total Trello clone. For a while it literally ripped the CSS off their site. In any case, it is very close to Trello, open source, and better yet, written in Python for easy modification.
  * The only barrier is that it lacks a mobile app, which makes it unsuitable for me.
* Meistertask

### Improvements

* **Replace the Static Cards with a real wiki.** - If Github Gollum is not working, it has to be replaced. We've set up Realms Wiki as a valid alternative, and it seems to work great.
  * [Gollum](https://github.com/github/gollum/) was the first Git-based wiki (introduced in 2012), and utilized the lingua franca of markup languages: markdown. It was also hosted and spam-proofed free by Github, which was critical in the organization's early days. However, it never has never added new features since that time, and Gollum's single page namespace became unwieldy at large scales.
* **When cards become static content, put them in Done, Archive, then push to the Wiki.**
  * For example, the original purpose of the Content to Import board in particular was to register incoming stories and make quick notes on them. Upon the completion of the story, another team member would pick up the card from the _To Wikify_ list and import the data into a wikipage. The card is then archived and put out of view.