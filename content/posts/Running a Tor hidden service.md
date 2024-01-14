---
title: "Running a Tor Hidden Service + selfhosting r4fo.com"
date: 2023-12-15T17:40:36+02:00
draft: false
language: en
featured_image: ../assets/images/featured/torhiddenservice.webp
summary: Bye bye Cloudflare Pages!
description: Bye bye Cloudflare Pages!
author: Admin
authorimage: ../assets/images/global/author.webp
categories: News
tags: News
---

### Selfhosting the homepage
Just 2 days after I dropped Cloudflare for most of my services, I have already made another big improvement: r4fo.com (this homepage) is **no longer** being hosted by Cloudflare Pages, I am now selfhosting it on my own server. This way I can 100% guarantee that no logs are being kept and decrease the amount of third parties again.

### Running a Tor hidden service
And to top it all off, I am now also running a [Tor](https://wikiless.r4fo.com/wiki/Tor_(network)) hidden service at [r4focoma7gu2zdwwcjjad47ysxt634lg73sxmdbkdozanwqslho5ohyd.onion](http://r4focoma7gu2zdwwcjjad47ysxt634lg73sxmdbkdozanwqslho5ohyd.onion). The benefits of this Tor hidden service are that traffic is now end to end encrypted for Tor users, onion sites are more anonymous than clearweb sites and they're also censorship resistant.

*All services will be available through the Tor hidden service aswell! When you visit ```*.r4fo.com``` through Tor Browser, it will automatically redirect you to ```*.r4focoma7gu2zdwwcjjad47ysxt634lg73sxmdbkdozanwqslho5ohyd.onion``` (sometimes it will ask you if you want to be redirected, just click yes)

<br>

*Edit [15 Dec 2023 - 20:58]: Wikiless, Libremdb and BreezeWiki now also work over onion!* <br>
*Edit [18 Dec 2023 - 21:08]: Quetre now also works over onion!*