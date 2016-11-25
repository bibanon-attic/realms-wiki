The wiki is the center of the Bibliotheca Anonoma, a knowledgebase for archival and data showcases, editable by anyone. 

## Realms Wiki

The new engine is the Realms Wiki, a Python-based Git wiki engine inspired by Dillinger, Gollum, and Ghost.

### Benefits over Gollum

* **Responsive Theme.** - The pages resize to fit a smaller phone screen, and yet also look great on the desktop.
* **Based on Python**, a language the organization is familiar with. Modifying or extending the wiki engine becomes much easier.
  * Gollum was based on Ruby and an extension system was never produced for it.
* **Self-Hosted.** Realms Wiki can be deployed standalone to a Linux server with PostgreSQL as the database.
  * This is a significant improvement over hosting Gollum, which required an entire Ruby on Rails site to be built around it and provide authentication.
* **Collaborative Edit.** Realms Wiki makes collaborative edit and chat possible with multiple users at the same time. This makes writing wikipages a more social experience, like an Etherpad.

### Improvements

* **Home Page Template** - A wikipedia style home page template with tables would be better than just a bunch of bulleted lists taking up space, or a sidebar that eats 1/3rd of the screen.

### Issues

* **Lacks Image Upload support.** Since we have a free Amazon AWS plan, we should make use of S3 image upload.
* **No sidebar, header, or footer.** Better navigation systems would help users move around the wiki without having to return to the Front page. This is one thing Github Gollum does better.
* **Anonymous users can delete pages.** Anonymous edit is fine, but allowing anonymous users to delete pages is a recipe for disaster.
* **Normal users can delete pages.** This should not be allowed either.
* **Lacks Administrator Accounts.** Administrators should be set up to delete users and be the only ones to delete pages. Whoever is UID=1 should become the first admin.

## Usage

### Directory Structure

* Pages should be organized into a subfolder directory structure, along with an index page with the same name as a folder. There are main 
  *  `/stories/cool-story-bro/1`, for [the first chapter](/stories/cool-story-bro/1) of [Cool Story Bro](/stories/cool-story-bro). This folder also has [an index page](/stories/cool-story-bro) describing and linking to the pages in question: `/stories/cool-story-bro`

## Import Sources

* [Github Gollum Wiki](http://github.com/bibanon/bibanon/wiki) - Since 2012, the Bibliotheca Anonoma has used a Github Gollum wiki. However, this wiki has various limitations and problems that have made it unsuitable for further work.
  * View the [Gollum Migration Plan](/wiki/gollum) for more details on how to import from it.
* [Trello](http://trello.com/bibanon) - Gollum became unworkable as time went on, the organization began to rely on Trello as an informal wiki. Unfortunately, this misuse of the kanban board system clogged the lists with immobile and stagnant cards.
  * A migration plan is written at the [Kanban page.](/services/kanban)
* IRC Logs - The Bibliotheca Anonoma publishes IRC logs at ~6 month intervals, which detail how the organization responded to events or issues.