---
title: Aseprite Record
description: An Aseprite utility script for recording snapshots in app to build pixel art time lapses.
date: 2019-04-01
layout: post
tags:
    - plugin
    - open-source
    - Lua
---

This project started out of a desire to see if I could build a way to leverage APIs within [Aseprite](https://www.aseprite.org/) to support creation of timelapses without the need for a secondary application like a screen recorder. At the time I had taken up an interest in creating pixel art and loved seeing artists share the in-progress animations of the work being created, a wonderful reminder of the effort that goes into these works.

![Screenshot of Plugin Menu](/img/projects/aseprite-record/aseprite-record_menu.png)

After digging through the Aseprite API documentation, I found that it was possible for me to come up with a system to take snapshots of the current state as a flattened layer, and save it in a way that let me maintain an index for ordering purposes. The reason for maintaining an order on the file names was to leverage Aseprite's built in functionality to open files with the same name prefix and digit optionally as a gif, treating each file as a frame. Later on this would receive a contribution that tracks a separate indexing file, reducing complexity when identifying the next iterator and not relying on file names.

This was able to be tied to a keyboard shortcut or menu option, and seemed pretty sufficient for the time though far from ideal.

### Example of producing a gif made with this utility
![Screenshot of Gif loading](/img/projects/aseprite-record/aseprite-record_gif.png)
![Example gif](/img/projects/aseprite-record/aseprite-record_example.gif)

At a [later point](https://www.aseprite.org/api/Changes#v1230), the Aseprite API received an update exposing signals for actions taken while editing a file. This allowed support for a non-blocking method of automating the snapshot process, therefore making it not only much more functional but customizable as to when the trigger occurs. The trigger was based off any time a change occurred to the sprite, which meant I was able to have it capture not just brush strokes but any copy/paste, resize, crop, etc events that occur. As an option for the user, they are able to set how many actions occur before a snapshot is taken - letting them increase or decrease the frequency of changes recorded.

![Automatic Control Palette](/img/projects/aseprite-record/aseprite-record_control.png)

At the time of writing the project has had over 6,600 downloads.

## Project Links
### Itch.io Project page
<iframe src="https://itch.io/embed/583873?linkback=true&amp;bg_color=f9f9f9&amp;fg_color=1C1D1E&amp;link_color=1C1D1E&amp;border_color=f9f9f9" width="552" height="167" frameborder="0"><a href="https://sprngr.itch.io/aseprite-record">Record for Aseprite by sprngr</a></iframe>

### Github Repository
<div class="github-card" data-github="sprngr/aseprite-record" data-width="400" data-height="177" data-theme="default"></div>
<script src="//cdn.jsdelivr.net/github-cards/latest/widget.js"></script>
