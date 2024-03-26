---
title: Twitch Bot
description: An extensible Javascript based combination chatbot and Twitch client built for a private streamer.
date: 2023-02-01
layout: post
tags:
    - chatbot
---

I had been contacted to build a chatbot for a 24/7 livestream.

I designed an extensible Javascript based combination chatbot and Twitch client to allow simple interfacing between the Twitch eventing API, chat, and the client’s proprietary streaming software during their 24hr daily streams, handling over 100 active users at a time.

The chatbot handles synchronizing events between what was occurring on the live stream and corresponding user chat inputs and channel redemption queue, rate limiting & queuing user based actions, and automating ban of known bot users.

The core functionality for the bot leveraged shell scripts, NodeJS, and the [Twurple](https://twurple.js.org/) API wrapper.
