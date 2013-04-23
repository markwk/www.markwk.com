---
title: "Backup iPhoto Library to Amazon's S3: How's and Why's with Mac OS X"
author: Mark Koester
layout: post
blr_date:
  - 2013-04-23
categories:
  - Geek Talk
  - Mac OS X
  - AWS
  - Technology
  - Backups
comments: true
published: true
---

So, *More Geek Talk*: 

I've been on a bit of an obcessive exploration of new storage options for my data. There are really a ton of options. Some are both the best in terms of ease of use and in terms of price (i.e. Free). Others require a bit of an evaluation of price vs. quality. Once you get to a lot of data though, you're going to have pay something. 

In this post, I'd like to talk about an exploratory attempt at backing up my iPhoto Library to S3. So, you want your photos safely guarded in AWS S3?

(Admittedly I'm increasinly nervous about how my data is tied up with any vendor-specific program, i.e. Everything Apple, like iPhoto, but let's leave that point aside for now.)

<!--more-->

## Why's of Storing Your Data with Amazon's S3 vs Dropbox 

For personal data, I'm a big fan of Dropbox for managing my business and life critical documents. Dropbox is really simple and syncs well across multiple devices. I use to for doing writing on different devices in different places and times. It's also a great way to work with large files with a team. I don't really like Box or Google Drive as much, since both seemed less reliable and buggy, but perhaps that's just me. I think the price of $10/month for 60GB of storage is quite reasonable and that's probably enough space for me to also store the big stuff like photos and some videos. 

Before going with Dropbox, I wanted to explore Amazon's S3 option. At the time of writing, I'm already using S3 to host [my personal blog](http://www.markwk.com), which I [migrated to Octopress recently](http://www.markwk.com/2013/04/wordpress-migrations-to-octopress-blog.html). 

S3 is a file storage system for big data Amazon. You use "buckets" to host files and you get billed according to the amount you store per month and the number of times (i.e. requrests) you use to upload, update and read those files. It's largely still a developer-centered system, but there are a increasing number of client applications that make it easy to use (for example, CyberDuck lets you manage data like an FTP client). Many CMSs provide integration with S3 as a file storage system, [as does Drupal](http://drupal.org/project/amazons3). 

A number of websites use S3 to host their larger files like images and videos. Apparantly Dropbox is using as their backend storage too.

S3 storage enables you to store a lot of data, reduce costs for usage, provide good performance and pay-as-you-go.  

I'm still not sure that the cost saves with hosting with S3 will be worth it, but we'll get to the numbers later. Let's see how to sync your files with S3

## Setting Up Syncing iPhoto Library to S3: s3fs vs. s3cmd

So, you wanna backup your iPhoto library to S3? 

Well, there are a couple options for setting up s3 syncing. The most obvious would be to [mount an S3 as a local disk drive](http://blog.eberly.org/2008/10/27/how-i-automated-my-backups-to-amazon-s3-using-rsync/) and [run rsync](http://andrewwilkinson.wordpress.com/2011/01/14/rsync-backups-to-amazon-s3/). Technically, you'll need to install and use FUSE and [s3fs](https://code.google.com/p/s3fs/wiki/FuseOverAmazon). I got it to install using MacPorts and after a few fixes, it seemed to be working. But I ended up running into enough error messages that I got nervous. So, I went with [s3cmd](http://s3tools.org/s3cmd), which did work.

Like [deploying my Octopress blog to s3](http://www.markwk.com/2013/04/wordpress-migrations-to-octopress-blog.html), I ended up using s3cmd to sync files from a local directory to a specific s3 bucket. The idea here is to just sync changed files and to avoid the long time it takes to update every single file. There is probably a slicker way to do this but once you've got s3cmd working (I recommend using Homebrew to install!), the rest is pretty easy. 

Here's the command I am using:

{% codeblock %}
$ s3cmd sync --delete-remove /Users/<USERNAME>/Pictures/iPhoto\ Library s3://<YOUR-BUCKET-NAME>
{% endcodeblock %}

What this command will do 

By the way, you maybe want to set up a cron tab, as suggested [here](http://jacksoncage.se/posts/Sync-files-to-S3-on-Mac-OS-X/), to invoke this command and periodically update your data in the background. 

## Costs of S3 as a backup option

Besides the time it took to get everything set up and working, here is the breakdown of costs. 

My iPhoto Library is currently 32.9 GB and has apparantly 48,107 files. Let's calculate cost for uploading and stoarge

#### Uploading Costs

* It costs $0.005 per 1,000 requests
* So, for my 48,107 files it will cost $0.24 to upload. 

#### Storage Costs

* It costs $0.095 per GB for the first 1 TB / month of storage used
* So, 32.9 GB it will cost $3.04 per month. 

By the way, Amazon provides a nice cost calculator for you to check your numbers. [Try it here](http://calculator.s3.amazonaws.com/calc5.html).

## Conclusion: Cost of Ease. 

For now, my main objective was achieved: I now have a cloud backup of most of my images. Even though I've got the local copy and a usb drive backup already, as my father says, "It doesn't hurt to have one more backup," as he adds another burned DVD backup to the stack. 

I'm not sure I like have such a "weight" of data. It seems like I need to convert it to some kind of S3-hosted image gallery maybe. I suppose that's a hack for another day. 

While I'm not as obcessive as my dad about backing up my data, I think I do a decent job keeping things stored as needed. All the essential data is covered, and in the event of a disaster, I could be up and running pretty quickly on an alternative computer, I think. 

In terms of costs, I'm still not sure that the few bucks savings for directly using and storing on S3 makes up for the ease of use you get using Dropbox. I'm guessing they also got a lot more contingency plans set up for data storage, since that's really all that do.  Anyways, for now, geek out success, and for now, I'm happy that I can now back up another bit of data in the cloud, just in case things go wrong. 

I think sometimes though we tend to spend a lot of time trying to do something when if we spent a couple bucks we'd get a more reliable and better solution. 

Sometimes though it's not the solution we care about, but the fact we kinda sorta did it ourselves. *Be a maker. DIY.*