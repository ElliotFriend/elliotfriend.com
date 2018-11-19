---
layout: post
status: publish
published: true
title: Fibonacci Sequence in Python
author:
  display_name: elliotfriend
  login: elliotfriend
  email: elliot@voris.me
  url: ''
author_login: elliotfriend
author_email: elliot@voris.me
wordpress_id: 267
wordpress_url: http://elliot.voris.me/?p=267
date: '2014-03-09 00:55:38 -0600'
date_gmt: '2014-03-09 06:55:38 -0500'
categories:
- Technology
tags:
- technology
- code
- python
comments: []
---
In case anyone ever wanted to know how to run the Fibonacci Sequence in Python, here's how I did it:

```
#!/usr/bin/env python
import sys

f_seq = [ 0, 1 ]

while len(f_seq) <= int(sys.argv[1]):
    f_seq.append(f_seq[-1] + f_seq[-2])

print f_seq
```

Now, all you have to do is run 'fibonacci.py 20', and it will give you all the numbers through F20 (starting at zero).

Update: I put this up on Github, and have made a couple changes since. [Check it out here!](https://github.com/ElliotFriend/bin/blob/master/fibonacci.py)
