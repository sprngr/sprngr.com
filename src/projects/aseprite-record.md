---
title: Aseprite Record
description: An Aseprite utility script for recording snapshots in app to build pixel art time lapses.
date: 2020-04-15
layout: post
tags:
    - plugin
    - open-source
---

This project started out of a desire to see if I could build a way to leverage APIs within Aseprite to support creation of timelapses without the need for a secondary application like a screen recorder.

After digging through the API documentation, I found that it was possible for me to come up with a system to take snapshots of the current state as a flattened layer, and save it in a way that let me maintain an index. Later on this would receive a contribution that tracks a separate indexing file, reducing complexity when identifying the next iterator.

This was able to be tied to a keyboard shortcut or menu option, and seemed pretty sufficient.

At a later point, the API received an update exposing signals for actions taken within a file. This allowed support for a non-blocking method of automating the snapshot process, therefore making it not only much more functional but customizable as to when the trigger occurs.

<iframe src="https://itch.io/embed/583873?linkback=true&amp;bg_color=f9f9f9&amp;fg_color=1C1D1E&amp;link_color=1C1D1E&amp;border_color=f9f9f9" width="552" height="167" frameborder="0"><a href="https://sprngr.itch.io/aseprite-record">Record for Aseprite by sprngr</a></iframe>

[Github Repo](https://github.com/sprngr/aseprite-record)
