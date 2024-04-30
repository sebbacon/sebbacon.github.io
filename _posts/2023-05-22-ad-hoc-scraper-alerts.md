---
layout: post
title:  "Scraping and alerting with Github Actions"
date: 2023-05-22 
categories: coding
---

[Dave](http://evansd.net/) pointed out [this weird
trick](https://github.com/sebbacon/gha-page-change-monitor) some years ago, to
use Github actions as a free engine for checking websites and sending you email
alerts when they change.

I use it fairly frequently to track things online. The code in that repo assumes
the web page is available on the public internet.

I've written a variety of horrible scrapers to deal with websites that need you
to log in, but I've not satisfied myself they're safe to share, so I'm not
sharing them...

(The funkiest of these used Cypress, but for some reason, after hours of hacking, I was
unable to make that work inside Github Actions.)

