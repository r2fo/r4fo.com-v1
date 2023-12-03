---
title: "🔒 Privacy Policy"
date: 2023-11-1T0:0:0+1:00
draft: false
language: en
description: Privacy Policy
featured_image: ../assets/images/featured/privacypolicy.png
---

### Last updated: 3 December 2023 @ 18:06 CET
View the [changelog](#changelog) at the bottom of this page

<p class="mb-8 font-normal text-gray-500 dark:text-gray-400 sm:text-xl">I run these services so people don't get exposed to ads, tracking and fingerprinting from big platforms. Logically, ...</p>

<p class="mb-8 font-light text-white-500 dark:text-white-400 sm:text-xl">
    I do <strong style="color: red;">not</strong> collect any personal information<br>
    I do <strong style="color: red;">not</strong> sell any data<br>
    I do <strong style="color: red;">not</strong> share any data, except with the <a href="#third-parties">Third Parties</a> mentioned below<br>
</p>
<hr>
<p class="mb-8 font-normal text-black-500 dark:text-black-400 sm:text-xl">You may contact me at <a href="mailto:privacy@r4fo.com">privacy@r4fo.com</a> if you have any questions regarding this privacy policy</p>
<hr>

## Data collected by the Operator
### This website (r4fo.com)
- Hosted by Cloudflare Pages, to ensure uptime in case of server maintenance.
- I do not collect any data, but Cloudflare probably does
- <a href="https://www.cloudflare.com/privacypolicy/">Their privacy policy</a>.

### Nginx

- By default, all access and error logs in Nginx are sent to <code><a href="https://wikiless.r4fo.com/wiki/Null_device">/dev/null</a></code>.
- ⚠️ Logging may temporarily be enabled to combat abuse or to debug errors. These logs contain your IP address, user agent, query and timestamp. These logs will be erased almost immediately (within 1-3 hours). I will inform you about any logging through the below text. 
- Currently logging is **❌ DISABLED** (for a history you can view the [changelog](#changelog) below)
- 🔄 Cloudflare Proxy is **✅ ENABLED**, unless otherwise noted

### Piped (piped.r4fo.com)
- I only collect the following essential data if you have create an account: username, password (<a href="https://wikiless.r4fo.com/wiki/Cryptographic_hash_function#:~:text=A%20common%20use%20of%20hashes,in%20a%20file%20or%20database">hashed</a>) and channel subscriptions.
- I do not view the database, but you have to trust me on my word

## Third Parties {#third-parties}
- Piped is hosted on a server provided by <strong style="color: hsl(184,73%,29%);">Netcup</strong>. [Their privacy policy](https://www.netcup.eu/kontakt/datenschutzerklaerung.php)
- All other services are hosted on a server provided by <strong style="color: red;">Oracle Cloud Infrastructure</strong>. [Their privacy policy](https://www.oracle.com/legal/privacy/services-privacy-policy.html)
- <strong style="color: orange;">Cloudflare</strong> is used for <strong style="color: hsl(210, 92%, 56%);">CDN and security</strong>. Cloudflare may log traffic that looks suspicious, normal users do not have to worry since only bots and abusers fall into this. These WAF logs include: IP Address, User Agent and Query. Cloudflare discards these WAF logs after 14 days. [Their privacy policy](https://www.cloudflare.com/privacypolicy/)
- <strong style="color: hsl(270, 60%, 70%);">Crowdsec</strong> is used for <strong style="color: hsl(210, 92%, 56%);">security</strong>. Crowdsec is open source and runs locally. In case of abuse, it reports the IP address to Crowdsec Threat Intelligence. Again, normal users do not have to worry since Crowdsec only reports back abusive IP Addresses. [Their privacy policy](https://www.crowdsec.net/privacy-policy)

## Changelog {#changelog}
[3 Dec 2023] r4fo.com is now being hosted by Cloudflare Pages, previously by GitHub Pages <br>
[2 Dec 2023] Status page is now selfhosted <br>
[25 Nov 2023] Created privacy policy