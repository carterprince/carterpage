---
title: Welcome to the Blog (why I don't like Eleventy)
date: 2022-06-28 21:12:37
---

I spun this site up using [Hugo](https://www.11ty.dev/), and the [XMin](https://github.com/yihui/hugo-xmin) theme by [Yihui Xie](https://yihui.org/) (alongside some tweaks). This site is hosted by [Netlify](https://www.netlify.com/).

## Eleventy

Originally, this site was created with [Eleventy](https://www.11ty.dev/). I found eleventy too buggy and unstable for my taste. Even when I did encounter bugs, tolerating them was difficult; as Eleventy's obscurity made finding solutions to my problems a hassle. Hugo, on the other hand, frankly [just works](https://yewtu.be/watch?v=nVqcxarP9J4), has a [larger community](https://star-history.com/#11ty/eleventy&gohugoio/hugo&Date) to fall back on when I have problems, as well as lots of already existing code to steal (see [here](https://themes.gohugo.io/)).

The first thing you learn about Eleventy is that it's written in Javascript. Rather than being a single, pre-compiled binary like Hugo, Eleventy requires you to use `npm` packages and maintain a `package.json`, things I consider ontologically evil (joking, but there are [real reasons](https://drewdevault.com/2021/11/16/Cash-for-leftpad.html) for opposing it). I should not have to 1) install an `eleventy-plugin-rss` package and 2) add it to my `package.json` then 3) add it to my `.eleventy.js` `require`s to get one, maybe two simple javascript functions needed to get an RSS feed working. I do not want to have to keep track of these two files. Hugo, however, is written in Go, which is a very sane language all around, and because Go produces standalone binaries (meaning, of course, 0 dependencies) it simplifies things a lot for the end user. So naturally, Hugo comes with RSS feeds built in, so no wrangling with dependencies (although I don't see why Eleventy couldn't also come with them built in, seems stupid not to. Perhaps this just goes to show that separating/compartmentalizing projects out into a billion subcomponents sounds at best strange in theory and is at best hell in practice).

Further, if your site's framework requires constant maintenence and tweaking, or even worse, you find it fun, that's just sucking up time you could be actually adding content to the site. You want your [stack to be as boring as possible](https://flaviocopes.com/boring-stack/).

So for the reasons listed above, I have abandoned Eleventy. Stay tuned.
