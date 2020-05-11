---
title: Hello World, It's Me Again
description: This is a the first post in a series of posts about getting started all over again, oh and it's open source now. It may not be the prettiest website, but it sure is readable.
date: 2020-04-09
layout: post
---

I feel like I write one of these posts every so many years, but never commit past it.

This time around I'm rebuilding my personal portfolio/whatever site from the ground up for a handfull of reasons.

## Great for relearning web basics

I'm a full stack dev, but it hit me like a ton of bricks when I realized I probably couldn't start fresh without a long wind up period. So I spent a lot of time getting reeducated on what is currently modern web without the crutch of additional frameworks.

In my daily life I work on an existing web application, so not exactly much room to break ground into new web technologies and often times our CSS tends to be additive rather than redesigning full layout patterns with modern tech.

I spent some time reading through [Interneting Is Hard](https://www.internetingishard.com/) to reorient myself with what is available. I took the approach of starting from the beginning, just in case I may miss something. I am thrilled that aspects of front end design that used to be quite painful are now much more straightforward thanks to advances in CSS.

## Moving to Eleventy + Github Actions

I took the chance to learn how to use Eleventy as a static site generator, mostly due to how simple it looked and rather than reinvent the wheel it is working with existing formats so I can move this to another generator or roll my own if necessary.

I know I could have reduced my time for development greatly by using a full blown CMS, but that wouldn't be fun now would it?

Previously I had used Jekyll, but didn't really feel like it was jiving well with me. I recall iterating upon a boilerplate build & deployment system that worked upon a git hook. This ended up putting way too much stress on the dinky server I was using, at one point my hosting provider cut me off entirely.

In this current process, I am using Github Actions to do the build process upon receiving it to the master branch. It performs a build and sends just the new content up to my server - and then does some Docker container scaling to reload it without ever going offline. Kind of neat how stuff has progressed.

## Open Source, Work In Progress

This also gave me a chance to accept that I won't get this right or how I envision it from the get go. In fact, it'll be better if I just start producing content and develop a design around it instead. 

To quote Jeffrey Zeldman:

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Content precedes design. Design in the absence of content is not design, it&#39;s decoration.</p>&mdash; zeldman (@zeldman) <a href="https://twitter.com/zeldman/status/804159148?ref_src=twsrc%5Etfw">May 5, 2008</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> 

This is often my first problem: I get so caught up in how it looks I don't even consider how it will interact with the content I need it to present. I spent some time drafting small prototypes in codepen to get the ball rolling, but just enough for some basic type setting.

<p class="codepen" data-height="265" data-theme-id="light" data-default-tab="result" data-user="sprngr" data-slug-hash="BaBXzBO" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="Kitbash Layout Prototype">
  <span>See the Pen <a href="https://codepen.io/sprngr/pen/BaBXzBO">
  Kitbash Layout Prototype</a> by Michael Springer (<a href="https://codepen.io/sprngr">@sprngr</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>

The design itself is named "Kitbash", inspired by the manuals from my hobby of building model kits and the similarity of how development tends to be mashing up and remixing code as you would combine parts from several model kits to make something wholly unique. I felt the design of the manual was something great to take inspiration from, not in a skeuomorphic way but because they have to be clear about what they're presenting to the builder similar to how your design should be able to present your content to the reader without any issues.

While building this out, there were several aspects of the content I hadn't even considered. Rather than be discouraged, I'm publishing it anyway so I can iterate upon it later. This is a work in progress after all.

And in the spirit of helping others learn from what I've learned, this project is open source (at least the code, not my writing or images) on [Github](https://github.com/sprngr/sprngr.com).