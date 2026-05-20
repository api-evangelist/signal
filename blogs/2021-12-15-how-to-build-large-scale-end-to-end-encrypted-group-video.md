---
title: "How to build large-scale end-to-end encrypted group video calls"
url: "https://signal.org/blog/how-to-build-encrypted-group-calls/"
date: "Wed, 15 Dec 2021 00:00:00 +0000"
author: ""
feed_url: "https://signal.org/blog/rss.xml"
---
Signal released end-to-end encrypted group calls a year ago, and since then we’ve scaled from support for 5 participants all the way to 40. There is no off the shelf software that would allow us to support calls of that size while ensuring that all communication is end-to-end encrypted, so we built our own open source Signal Calling Service to do the job. This post will describe how it works in more detail.
