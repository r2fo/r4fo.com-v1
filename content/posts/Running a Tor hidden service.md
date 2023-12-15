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

And to top it all off, I am now also running a [Tor](https://wikiless.r4fo.com/wiki/Tor_(network)) hidden service at [r4focoma7gu2zdwwcjjad47ysxt634lg73sxmdbkdozanwqslho5ohyd.onion](http://r4focoma7gu2zdwwcjjad47ysxt634lg73sxmdbkdozanwqslho5ohyd.onion). The benefits of this Tor hidden service are that traffic is now end to end encrypted for Tor users, onion sites are more anonymous than clearweb sites and they're also censorship resistant.

All services will be available on the Tor hidden service aswell! When you visit ```r4fo.com``` through Tor Browser, it will automatically redirect you to ```r4focoma7gu2zdwwcjjad47ysxt634lg73sxmdbkdozanwqslho5ohyd.onion``` (sometimes it will ask you if you want to be redirected, just click yes)
<br>

### ⚠️ Please be aware that the Tor hidden service is still work in progress and the following instances currently don't work on the onion domain:
- Wikiless
- Libremdb
- Quetre
- Breezewiki