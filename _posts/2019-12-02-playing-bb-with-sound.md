---
layout: post
title:  "Playing bb with Sound"
date:   2019-12-02 1:55:00 -0700
---

Long ago, when computers were slowly evolving, a popular thing to do 
was to create little demos to demonstrate how capable the hardware was. 
These were called demoscenes and many are still being made today, 
which you can checkout on [pouët.net](https://pouet.net). Here are a few 
YouTube videos of really cool demoscenes that you can checkout!

 - [bb](https://youtu.be/FLlDt_4EGX4)
 - [dope](https://youtu.be/_yJ5M3BY2Ts)
 - [Second Reality](https://youtu.be/rFv7mHTf0nA)
 - [WE ARE NEW](https://youtu.be/L8onlB0F1_A)
 - [Comaland](https://youtu.be/90AEamQCLog)
 - [Chaos Theory](https://youtu.be/ZfuierUvx1A)
 - [Offscreen Colonies](https://youtu.be/PaNYOzwlVC8)
 - [fermi paradox](https://youtu.be/JZ6ZzJeWgpY)
 - [on](https://youtu.be/XF4SEVbxUdE)

One of the most well known demoscenes is `bb`, which has some problems running on modern 
Linux distros where it freezes a few seconds in when you have the sound playing.
A way to bypass this is to play the music without sound and use an external program 
to play the music.

To play it with sound, use `bb & sleep 24;mplayer /usr/share/bb/bb.s3m` 
and immediately press `n` to not play the music, as we are using a different method. 
You could also make it an alias and save it in your bash profile or whatever as 
`alias bbmusic='bb & sleep 24;mplayer /usr/share/bb/bb.s3m'`.

And that's pretty much it! Enjoy the coolness of `bb` running in real time on your computer!

