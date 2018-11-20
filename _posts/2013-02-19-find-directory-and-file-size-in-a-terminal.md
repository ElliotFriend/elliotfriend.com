---
layout: post
status: publish
published: true
title: Find Directory and File Size in a Terminal
author:
  display_name: elliotfriend
  login: elliotfriend
  email: elliot@voris.me
  url: ''
author_login: elliotfriend
author_email: elliot@voris.me
wordpress_id: 237
wordpress_url: http://elliot.voris.me/?p=237
date: '2013-02-19 16:40:32 -0600'
date_gmt: '2013-02-19 21:40:32 -0600'
categories:
- Technology
tags:
- technology
- work
comments: []
---
Here's a really handy command that I tend to forget exists.

If you're running out of disk space, it can be really hard to track down a
runaway file. Here's a way you can get some more information.

```bash
du -hs /path/to/directory/or/file
```

This helped me figure out once where my **114GB** log file was taking up all my
space! Super handy!

_EDIT:_ I will point out that if you are trying to find the size of all files or
directories in a given directory, use the asterisk to target them all:

```bash
du -hs /home/elliot/*
```
