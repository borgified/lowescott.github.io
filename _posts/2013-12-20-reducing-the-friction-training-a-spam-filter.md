---
author: slowe
comments: true
date: 2013-12-20 09:00:00+00:00
layout: post
slug: reducing-the-friction-training-a-spam-filter
title: 'Reducing the Friction: Training a Spam Filter'
wordpress_id: 3391
categories:
- General
- Macintosh
- Personal
tags:
- Automation
- Macintosh
- Personal
- Productivity
---

I'm back with another "Reducing the Friction" blog post, this time to talk about training an e-mail spam filter. As you may recall if you read one of the earlier posts (may I suggest [this one][1] and [this one][2]?), I use the phrase "reducing the friction" to talk about streamlining and simplifying commonly-performed tasks so as to allow you to improve your own personal efficiency and/or adopt more efficient habits or workflows.

I recently moved my e-mail services off Google and onto [Fastmail](http://www.fastmail.fm/). (I described the reasons why I made this move in [this post][3].) Fastmail has been _great_---I find their e-mail service to be much faster than what I was seeing with Google. The one drawback, though, has been an increase in spam. Not a huge increase, mind you, but enough to notice. Fastmail recommends that you help train your personal spam filter by moving messages into a folder you designate, and then telling their systems to consider everything in that folder to be spam. While that's not hard, it's also not very streamlined, so I took up the task of making it even easier and faster.

(Note that, as a Mac user, most of my tips focus on Mac applications. If you're a user of another platform, I do apologize---but I can only speak about what I use myself.)

To help make this easier, I came up with this bit of AppleScript:

{% gist lowescott/7990921 %}

(Click [here](https://gist.github.com/lowescott/7990921) if you don't see a code block above this paragraph.)

To make this work on your system, all you need to do is just change the two `property` declarations at the top. Set them to the correct values for your system.

As you can tell by the comments in the code, this script was designed to be run from within Apple's Mail app itself. To make that easy, I use a fantastic tool called [FastScripts](http://www.red-sweater.com/fastscripts/) (_highly recommended!_). Using FastScripts, I can easily designate an application-specific shortcut key (I use Ctrl-Cmd-S) to invoke the script from within Apple Mail. Boom! Just like that, you now have a super-easy way to both help speed up processing your e-mail as well as helping train your personal spam filter. (Note: if you are also a FastMail customer, refer to the FastMail help screens while logged in to get more details on marking a folder for spam learning.)

I hope this helps someone out there!

[1]: {% post_url 2013-06-21-reducing-the-friction-processing-e-mail %}
[2]: {% post_url 2013-07-19-reducing-the-friction-processing-e-mail-part-2 %}
[3]: {% post_url 2013-12-04-divorcing-google %}
