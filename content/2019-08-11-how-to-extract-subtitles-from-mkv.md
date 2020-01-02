---
layout: post
title:  "How to Extract Subtitles to a .srt from a .mkv file"
date:   2019-08-11 19:36:00 -0700
Category: blog
---

Sometimes, certain media devices can't read the subtitles that is built into an `.mkv` file.
Using this simple terminal command, this will extract the subtitles from an `.mkv` into a 
seperate `.srt` file that can be easily read. Be sure that the subtitle file and the video 
file share the same name to ensure that the subtitles will be used.

The first thing you have to do is to check which track the subtitles are on, this would 
usually be track 2, but might be different depending on other audio/subtitle tracks. In VLC 
go to `Tools > Codec Information` and check for the subtitle you want to extract. In this case, 
we are going to extract "track 2". Install `mkvtoolnix` (which is the package name on Ubuntu) 
and from the terminal use this command:

`mkvextract video.mkv tracks 2:savedfile.srt`

That's it. Hopefully this short guide will save you lots of time.
