---
title: The Why and How of Data Hoarding
date: 2022-07-09 10:17:05
---

![](/hoarding.jpg)

# What's that?

[Data hoarding](https://en.wikipedia.org/wiki/Digital_hoarding) is simply hoarding applied to data. I am a chonic data hoarder. I stumble across something mildly large and useful on the internet, and all of the sudden I want 3 copies of it stored on all my devices. I also like the idea of being the one guy in a 30 mile radius who thought to download wikipedia in the rare event that the internet disappears (but humanity itself somehow does not). So what do I hoard?

# Music

Music will probably be the most controversial section of this article, so I will tackle it first and in the most detail. Most of the points in this section apply to every other medium one might hoard.

I have a somewhat large (3-4 GB) collection of music on my computer. This isn't large relative to how much disk space most people have available, but in the realm of audio files it kind of a lot. I keep all my music in `~/music`. Usually, I listen to it with a shortcut that opens the folder in [`mpv`](https://mpv.io/), but sometimes I will use [`cmus`](https://cmus.github.io/). I do sometimes use spotify, but only to discover new music via the Discover Weekly feature.

So why download all your music? Well, part of it for me is because of my aforementioned data hoarding.

But there *are* practical reasons for doing this.

## The benefits

One such reason is offline listening. There are situations where using the internet simply isn't an option, such as on a plane, while camping, or if your internet happens to go down. Because the music is stored directly on disk, there is also no such thing as buffering or waiting for you music to load.

Morever, if you don't pay for Spotify Premium, Spotify will give you ads. These ads are [notoriously annoying](https://www.youtube.com/watch?v=BvQ571eAOZE), and they are the primary reason people purchase Premium. However, a little-known fact is you don't actually have to pay for Premium to get rid of the ads. You can just install a blocker such as [uBlock](https://ublockorigin.com/), or use [Brave](https://brave.com/).

If you just download your music, however, there is no threat of Spotify circumventing uBlock in the future, and there is no need to pay. Completely free forever.

Now you might be thinking:

> But Carter! I only listen to music on my phone in the car! I can't download my music there!

If you listen to music on your phone in the car, frankly that's just another argument for downloading your music, because cell service can be flaky when you are driving especially if you live in a more rural area like me.

So I recommend you download all your music to your computer, sync your music folder to your phone with a piece of software like [Syncthing](https://syncthing.net/), then actually play the music on your phone with an offline player (I recommend [BlackPlayer](https://play.google.com/store/apps/details?id=com.musicplayer.blackplayerfree&hl=en_US&gl=US) if you're on Android). I won't explain how to set up Syncthing or BlackPlayer, as you can find plenty of tutorials on that yourself, I just wanted to point you towards some good options (of course these aren't the only ones you have to choose from).

And finally, downloading your music literally makes you more independent, which is always desirable, especially when there is such a widespread deficit of independence in the modern digital world.

## Getting your music

If you are a Spotify user, I recommend [`spotdl`](https://github.com/spotDL/spotify-downloader). If you have `pip` installed, You can install it with:

```sh
pip install spotdl
```

Change directory to the location you'd like to download your music to. Then give `spotdl` the url to your playlist:

```sh
spotdl [playlist-url]
```

SpotDL will download the playlist asynchronously (i.e. several songs at a time). I believe the way it works is it finds the closest match for each song on Youtube, then uses `youtube-dl` to save it as an mp3 in the current directory.

# Books, Academic Articles (technically illegal ™)

You can download almost any book or textbook completely free on [Library Genesis](https://libgen.fun/) and [Z-Library](https://z-lib.org/).

Most academic papers and articles are available at [Sci-Hub](https://sci-hub.se/), simply paste the link to the article (or a DOI) in the input box.

Keep in mind, the links here are subject to change, as the existence of these sites is explicitly illegal so the owners are constantly domain hopping.

# Websites via Kiwix

Kiwix is a way to download websites and other content for offline viewing. These include Wikipedia (~95 GB), technical information, public domain books, etc. My current collection of `.zim` files amounts to a whopping 351 GB.

If you're a noob, just use the [Kiwix client](https://www.kiwix.org/en/) to download what you want. If you want to torrent the `.zim` files and maintain a `library.xml` manually, you can view all content offered by Kiwix [here](https://wiki.kiwix.org/wiki/Content_in_all_languages). You can host your own Kiwix server using [`kiwix-serve`](https://www.kiwix.org/en/downloads/kiwix-serve/).

# Videos

You can also use tools like `youtube-dl` to download videos (or whole channels) for offline viewing. I recommend `yt-dlp`, which is just a fork of `youtube-dl` with new features that is more actively maintained. Again, I won't explain how to use these tools, I'm just pointing you in the right direction.

# See Also

1. [DataHoarder - Reddit](https://www.reddit.com/r/DataHoarder/)
2. [Open access - Wikipedia](https://en.wikipedia.org/wiki/Open_access)
3. [Sci-Hub - About](https://sci-hub.se/about)

#### Disclaimer: For Legal reasons, this article is a joke.
