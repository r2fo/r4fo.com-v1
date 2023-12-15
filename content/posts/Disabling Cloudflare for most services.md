---
title: "Disabling ☁️Cloudflare for most services"
date: 2023-12-13T19:51:36+02:00
draft: false
language: en
featured_image: ../assets/images/featured/orangecloud.webp
summary: r4fo.com's infrastructure has outgrown the need for a third party MITM
description: r4fo.com's infrastructure has outgrown the need for a third party MITM
author: Admin
authorimage: ../assets/images/global/author.webp
categories: News
tags: News
---

Today, I have disabled Cloudflare's Proxy for most of my services. I have realized that my infrastructure has outgrown the need for a 24/7 [MITM](https://wikiless.r4fo.com/wiki/Man-in-the-middle_attack) by a third party. Cloudflare offers a lot of benefits to r4fo.com, including a [CDN](https://wikiless.r4fo.com/wiki/Content_delivery_network) and a [WAF](https://wikiless.r4fo.com/wiki/Web_application_firewall), but unfortunately with that comes the added privacy disadvantage.
<br>

Cloudflare's Proxy will still be enabled for these services, to protect them against bots wasting bandwidth and for CDN purposes:
- [Piped](https://piped.r4fo.com)
- [ProxiTok](https://proxitok.r4fo.com)
- [Libreddit](https://libreddit.r4fo.com)
- [SafeTwitch](https://safetwitch.r4fo.com)
- [Rimgo](https://rimgo.r4fo.com)