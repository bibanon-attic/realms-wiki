The Bibliotheca Anonoma works together, shares ideas, and socializes through the magic of group chat. 

## Before Group Chat

Before the introduction of a reliable group chat system with daily attendees, the organization was simply a one man show.

## Chat Systems

Our organization uses a rather complex combination of group chat systems designed to leverage the benefits and reduce the downsides of each.

The organization uses both IRC and Discord at the same time. Messages are transferred between the systems with the use of a bridge: [Itabashi](http://github.com/bibanon/itabashi).

### IRC

### Discord

### Itabashi - Discord Bridge

> It is named for the city of 板橋 (Banqiao), the county seat of New Taipei City in Taiwan. The kanji was coined by the Japanese, and means "Planked Bridge". 

**板橋 (Itabashi)**  bridges an IRC and Discord channel together, syncing messages back and forth using a bot.

It was developed for the Bibliotheca Anonoma to coordinate operations between its Discord and IRC channels.

For generations past, IRC has been an indispensable tool of communication. It's a system well suited to the computer age, and the various channels on a network make it easy to jump around and bring people together.

However, for the next generation of users who live in a mobile device focused world, IRC is increasingly frustrating and inadequate for their usage. 

Popular replacements such as Slack and Discord have been developed for cross-platform support, push notifications for all users, and significantly lower barriers to entry.

Unfortunately, Slack in particular leads to isolated walled communities that are disconnected literally, and figuratively from the Great big IRC networks. This occurs by design: corporate developers deliberately meet in private to build a proprietary, NDA-protected product before the competition finds out.

But this isn't how open-source development works. And as such, open source projects have been driven by IRC and remain the mainstay userbase. However, IRC just isn't platable to modern mobile users used to group chat. And IRCCloud is great, but costs money.

The solution we use is to run a bridge between the two chat worlds: of Discord (a popular, accessible group chat used by gamers), and IRC. 

### Future Alternatives

While we will still remain involved with IRC to some degree, a bridge between two systems can sometimes be unwieldy and cause issues upon desyncing.

There needs to be some open source, non-login chat system that is run on our own servers. Discord is quite great and popular, but it is fully proprietary.

Consider qwebirc such as Rizon's implementation [qchat.](https://www.rizon.net/chat)


### IRC Bot

Currently in semi-active development we are working with our own IRC bot, [Akabane](/akabane) to aid in our archival tasks.