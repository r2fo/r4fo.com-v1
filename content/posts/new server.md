---
title: "Reflecting on the journey + new server"
date: 2024-02-03T22:12:36+02:00
draft: false
language: en
featured_image: ../assets/images/featured/server.webp
summary: Enhancing the resilience of my infrastructure
description: Enhancing the resilience of my infrastructure
author: Admin
authorimage: ../assets/images/global/author.webp
categories: News
tags: News
---

It's been a while since my last post, and quite a few things have changed. I feel like this is going to be a long post so firstly, I want to thank everyone for their support. Thanks to your contributions, I was able to raise enough funds to rent an additional server.

### Throwback
But before I go any further, let's take a moment to reflect on the journey. <br>
I found most Piped instances to be very unstable. One day they would work fine, the next day they were buffering forever. Luckily I had a domain laying around and a free server from Oracle. And that's how I started this selfhosting journey, as rafo.tech, back in Oktober 2023.

In the first weeks, the average bandwidth usage was hovering around 200 gigabytes a day, at most. And that already felt like a lot to me. Within a month, I ran out of bandwidth on the free Oracle server, prompting me to go find another provider (more on that [here](https://r4fo.com/posts/netcup-server-migration/)).

Fast forward to today, Piped alone consumes more than 2 terabytes per day, not to mention the Tor relay.
These are the bandwidth statistics of the last month:

(the text continues under these stats)
```
 eth0  /  daily

          day        rx      |     tx      |    total    |   avg. rate
     ------------------------+-------------+-------------+---------------
     2024-01-05     2.86 TiB |    2.87 TiB |    5.72 TiB |  582.68 Mbit/s
     2024-01-06     3.01 TiB |    3.03 TiB |    6.04 TiB |  615.13 Mbit/s
     2024-01-07     2.93 TiB |    2.95 TiB |    5.87 TiB |  598.10 Mbit/s
     2024-01-08     3.16 TiB |    3.23 TiB |    6.39 TiB |  650.31 Mbit/s
     2024-01-09     3.26 TiB |    3.28 TiB |    6.54 TiB |  665.83 Mbit/s
     2024-01-10     3.19 TiB |    3.19 TiB |    6.39 TiB |  650.11 Mbit/s
     2024-01-11     3.21 TiB |    3.22 TiB |    6.42 TiB |  654.05 Mbit/s
     2024-01-12     3.23 TiB |    3.24 TiB |    6.47 TiB |  658.72 Mbit/s
     2024-01-13     3.12 TiB |    3.18 TiB |    6.31 TiB |  642.13 Mbit/s
     2024-01-14     3.09 TiB |    3.12 TiB |    6.21 TiB |  632.14 Mbit/s
     2024-01-15     2.74 TiB |    2.82 TiB |    5.56 TiB |  565.58 Mbit/s
     2024-01-16     2.95 TiB |    3.00 TiB |    5.96 TiB |  606.61 Mbit/s
     2024-01-17     2.93 TiB |    2.97 TiB |    5.90 TiB |  600.51 Mbit/s
     2024-01-18     3.01 TiB |    3.02 TiB |    6.03 TiB |  613.69 Mbit/s
     2024-01-19     2.96 TiB |    2.99 TiB |    5.95 TiB |  605.45 Mbit/s
     2024-01-20     3.07 TiB |    3.07 TiB |    6.14 TiB |  624.92 Mbit/s
     2024-01-21     3.06 TiB |    3.07 TiB |    6.13 TiB |  623.61 Mbit/s
     2024-01-22     2.86 TiB |    2.84 TiB |    5.71 TiB |  580.89 Mbit/s
     2024-01-23     2.92 TiB |    2.89 TiB |    5.82 TiB |  592.01 Mbit/s
     2024-01-24     2.76 TiB |    2.74 TiB |    5.49 TiB |  559.41 Mbit/s
     2024-01-25     2.84 TiB |    2.84 TiB |    5.68 TiB |  578.68 Mbit/s
     2024-01-26     2.92 TiB |    2.95 TiB |    5.87 TiB |  597.60 Mbit/s
     2024-01-27     2.95 TiB |    2.96 TiB |    5.91 TiB |  601.76 Mbit/s
     2024-01-28     3.43 TiB |    3.43 TiB |    6.86 TiB |  698.13 Mbit/s
     2024-01-29     2.83 TiB |    2.83 TiB |    5.66 TiB |  576.36 Mbit/s
     2024-01-30     2.01 TiB |    2.01 TiB |    4.02 TiB |  408.91 Mbit/s
     2024-01-31     2.06 TiB |    2.09 TiB |    4.16 TiB |  423.18 Mbit/s
     2024-02-01     2.11 TiB |    2.13 TiB |    4.24 TiB |  431.38 Mbit/s
     2024-02-02     2.06 TiB |    2.03 TiB |    4.09 TiB |  416.38 Mbit/s
     2024-02-03     1.47 TiB |    1.46 TiB |    2.93 TiB |  345.47 Mbit/s
     ------------------------+-------------+-------------+---------------
      estimated     1.70 TiB |    1.69 TiB |    3.39 TiB |
```

### 🔁 Reverse Proxy
Even though all of this is 100% legal, I've heard many stories of fellow privacy hosters whose servers got terminated, all because some ignorant person thought their content was stolen. <br>
I've decided to not take chances anymore. I got a server from a provider called [IncogNET](https://incognet.io/), they know how to deal with such unique problems. <br>
From now on, all the problematic services will be proxied by my IncogNET server.

### 👾 Libreddit
But big changes aside, I recently found out that Libreddit (the Reddit private frontend), which was dead for a few months, has been forked into a new project called [RedLib](https://gothub.r4fo.com/redlib-org/redlib). So of course I replaced the old Libreddit instance with RedLib.

What does this mean for you? Well, not only does RedLib support more of the newer features that Reddit added over the last months. It also has some fixes to the API ratelimiting problem that Reddit themselves introduced to counter privacy.

### 🐦 Nitter
Speaking of such ratelimits, the [Nitter](https://gothub.r4fo.com/zedeus/nitter) project is now dead after Twitter discontinued guest accounts, that Nitter was using to scrape Twitter. That news comes at a bad time because I was planning on running a Nitter instance, now that I've got a shiny reverse proxy. Hopefully this gets resolved.
<br>

Edit (29/2/2024): I was able to create a working Nitter instance!

### 📝 Final notes
This post has become too long, so again I want to thank everyone for their support. R4fo.com is slowly getting better with the day thanks to you. Feel free to send me feedback or suggestions through [this page](https://r4fo.com/contact/).

If you want, you can ❤️ support me [here](https://r4fo.com/donate/). 🙏 I really appreciate any contribution! 