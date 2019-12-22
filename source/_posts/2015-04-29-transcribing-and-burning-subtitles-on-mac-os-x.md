---
title: "Transcribing and Burning Subtitles to Videos on Mac OS X for Free"
layout: post
categories:
  - Subtitles
  - Language
  - Computer Tools
comments: true
published: true
---

{% img center /images/2015-resources/transcribe-subtitles-chinese-with-Aegisub.jpg %}

I want to show you how simple it is to transcribe the audio text into a subtitles file and then burn that translation directly onto a video file. I'll do this all by using free, open source software on Mac OS X.  

Sometimes it’s really redeeming to take a problem (e.g. I want to add Chinese subtitles to a [cool video](https://vimeo.com/125780002)), then research it on the Web, download the necessary programs and then learn by doing and do it. 

Here is what you need to transcribe and burn subtitles to a video (mp4 or avi or whatever) on a Mac OS X

1. **[Aegisub](http://www.aegisub.org)**: an open source program for transcribing a syncing subtitles file (SRT) for a video’s audio
2. **[HandBrake](https://trac.handbrake.fr/wiki/Subtitles)**: an open source program for encoding videos from one format to another and allows for adding the SRT subtitles text directly onto the video 

The following is how I implemented these two programs to create Chinese subtitles on a video using free, open source programs on Mac OS X. Here is the resulting video: ["创业周末是什么？ in Chinese"](https://vimeo.com/125991124).

<!--more-->

## Here is the Story of How I Did It

This is exactly what I did for adding Chinese subtitles to a cool recent [video about Startup Weekend](https://vimeo.com/125780002). I used only free, open source programs on Mac OS X.

I heard about the video in the morning and then downloaded it. By mid-morning I had manage to transcribe it to English.

I then google translated that into Chinese, made some basic corrections and sent the rough version to a Chinese colleague for improvement. 

Then came the next set of challenges: How do you create the correct file format for movie subtitles? It turned out the standard format was .srt. 

{% img center /images/2015-resources/transcribe-subtitles-chinese-with-Aegisub-reduced.jpg %}

After lunch, I tried several programs before managing to download and install Aegisub, an open source program for transcribing videos and creating syncing subtitles. 

After I got the program working, I spent nearly an hour and a half syncing my English transcription to the 2 minute video. Probably the main challenge is figuring out the key areas of the UI and which buttons you need to use. Using Aegisub, I was now able to export a working SRT file. 

{% img center /images/2015-resources/subtitles-srt-example-english.jpg %}

By this point, I got back the Chinese translation and redid the SRT for Chinese. Using VLC, I was able to watch the video using either English or Chinese subtitles. 

{% img center /images/2015-resources/subtitles-srt-example-chinese.jpg %}

Then came the next obstacle: How to “burn” these subtitles onto the video file, instead of merely linked via a sidecar SRT file? 

Using HandBrake, an open source video encoder program, I managed to create reduced versions of the original video. In turn, I tweaked various settings in order to, in turn, create a version of the video with the Chinese subtitles “burned” onto the video / image layer. 

{% img center /images/2015-resources/burn-subtitles-to-video-using-handbrake.jpg %}

## Summary: Tweaking and Posting to Chinese Social Media

By evening I had managed to do a basic English transcription of the video's audio into English. Using Aegisub, I created a synced SRT file for the video's English subtitles. With Google translate and a friend, we translated this into Chinese. 

The next step was a process of tweaking until the 2 minute video's audio and video matched will with the subtitles. I now understand why creating subtitles takes so long and have a much greater appreciation for volunteer translators around the world. 

In spirit of sharing and remixing, I shared the SRT file with the original poster to then add to his Vimeo video and to help future translators, so now we have the original video with subtitles. 

Finally I burned those subtitles onto the video and submitted it to a few Chinese video sites like [QQ Video](http://v.qq.com/page/b/s/3/b0152e88ts3.html) and [YouKu](http://v.youku.com/v_show/id_XOTQxNzcwNjE2.html?from=y1.7-1.2). 

I then took those videos and embedded them onto a UP Global's WeChat channel post to share with the Chinese community: [创业周末是什么](http://mp.weixin.qq.com/s?__biz=MzA5MzMxMTI3NQ==&mid=205274908&idx=1&sn=075c51cfe4574afc053e5a94dc7315fc#rd) 

[{% img center /images/2015-resources/startup-weekend-transcribed-video-to-chinese.jpg %}](https://vimeo.com/125991124)