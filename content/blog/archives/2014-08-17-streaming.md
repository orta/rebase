---
layout: post
title: on streaming
categories:
- "on"
uuid: 3EFFF477-860D-49BD-AFE4-F48935A1
---

<center>
  <img src ="/rebase/assets/images/streaming.jpg">
</center>

### Motivations

I like the idea of streaming. I think it shows a lot of the _behind the scenes_ action. The things that we create and put on show tend to be the process of many many hours of work. Whilst opening your source up gives an insight to incremental stages of the development process. It doesn't really show the infinite steps in-between.

When getting started in a  new environment, a lot of the problems are about trying to get acclimatised to tools & processes. When I was learning ruby I used to watch every peepcode, a tutorial video web-series, bought now by pluralsight. It started out a lot like NSScreencast, a series of videos around specific topics. By the end though, it had transformed into showing how some of the most prominent developers in the community would solve problems. You can see them all on [pluralsight here](http://beta.pluralsight.com/search/?searchTerm=play%20by%20play). This gives you an insight into the tools and how they manipulate them, with modern dev tools being so flexible everyone has their own flow. I want to share mine.

### Technical

I've been using [twitch.tv](http://twitch.tv) for hosting the stream, there are other options but twitch has won streaming. I regularly watch video games streamed on it, and now with [google buying](http://www.theguardian.com/technology/2014/may/19/twitch-youtube-live-games-google-acquisition-pokemon) it will solidify that position.

From the client side I use [OBS ( Open Broadcast Software )](https://obsproject.com) - a solidly made [open source](https://github.com/jp9000/obs-studio) tool for streaming. It's cross-platform, and feels like it, but it's by far the easiest software to use. It has one-click settings for twitch.tv by default and all you have to do is put in your stream key.

By default it cannot get audio from your system, so you can't share music. You can [fix this](https://obsproject.com/forum/resources/setting-up-mac-desktop-sound-capture-with-wavtap.79/) by installing WavTap. Note the application has to be running even though it is installing a kext. Audio levels can be a bit tricky. Not found a good answer for that yet.

From a non-technical perspective it was only really feasible for me to stream once I had dual monitors set up. This means notifications and private chats can be kept on the other screen as well as the twitch chat.
