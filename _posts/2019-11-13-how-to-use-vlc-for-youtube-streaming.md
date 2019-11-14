---
layout: post
title:  "How to use VLC for YouTube streaming on low-end computers"
date:   2019-11-14 11:14:00 -0700
---

Sometimes you want to watch a video on low-end hardware, like a Raspberry Pi or 
an old laptop. Browsing the web is already hard as it is on low-end hardware, 
but then it is made worse considering that Chromium/Firefox/Google Chrome does not have 
hardware acceleration on Linux! So for a lot of users, a good idea is to stream the
videos using VLC which has access to this. For example, the CPU usage of the 
Raspberry Pi goes from 95% to 20% using this method. Unfornatuately, if we want 
to search for videos, we would still have to go back to the browser to search for 
them, which is a pain as loading the pages can still take a long time, and the browser 
still uses lots of resources to access it. My solution is to use a very bare bones 
web browser that is good enoungh to copy and paste a video link into VLC's "network stream" 
option.

Lynx is a terminal based webbrowser, so it doesn't load CSS, graphics or JavaScript or 
any of that garbage. This means that you can browse the web on really low resources (15MB of RAM!), but 
this is only practical for text heavy and simple websites. With this, we can 
browse YouTube videos really quickly to copy the link and paste into VLC.
The downside here is that we would have to know what we want to watch since there 
is a lack of pictures, so this method is good to search for specefic videos we know about.

First install lynx using the package manager, on Ubuntu based distrobutions this is done with 
`sudo apt install lynx`. It may already be preinstalled. Go to `youtube.com` and then search 
for the video. Then go to the title and use `Shift + G`, right click and copy the whole link. 
Then go to VLC and `Media > Open Network Stream`. Paste the link and enjoy the video!

Also keep in mind, you can also download the video using `youtube-dl` and open the file if 
it's something you're going to watch frequently.