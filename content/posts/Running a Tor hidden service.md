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

Just 2 days after I dropped Cloudflare for most of my services, I have already made another big improvement: r4fo.com (this homepage) is **no longer** being hosted by Cloudflare Pages, I am now selfhosting it on my own server. This way I can 100% guarantee that no logs are being kept and decrease the amount of third parties again.

And to top it all off, I am now also running a [Tor](https://wikiless.r4fo.com/wiki/Tor_(network)) hidden service at [r4focoma7gu2zdwwcjjad47ysxt634lg73sxmdbkdozanwqslho5ohyd.onion](http://r4focoma7gu2zdwwcjjad47ysxt634lg73sxmdbkdozanwqslho5ohyd.onion). Using Tor Browser, you can now visit r4fo.com anonymously. And as a bonus, r4fo.com is now also censorship resistant.

All services will be available on the Tor hidden service aswell! When you visit ```r4fo.com``` through Tor Browser, it will automatically redirect you to ```r4focoma7gu2zdwwcjjad47ysxt634lg73sxmdbkdozanwqslho5ohyd.onion``` (sometimes it will ask you if you want to be redirected, just click yes)

Please note that this is still work in progress and the following instances currently don't work over onion:
- Wikiless
- Libremdb
- Quetre
- Breezewiki