---
title: "Post-Evernote: How to Migrate Your Evernote Notes, Images and Tags into Plain Text Markdown"
layout: post
categories:
  - Smart Notes 
  - Evernote
  - Plaintext
  - Tech Guide
  - Migration
  - Note-taking
  - Organization
date:   2018-12-11
comments: true
published: true
permalink: /migrate-evernote-plaintext.html
---



**14,147**. That’s the number of notes I had in Evernote. 

A few weeks later, only a few thousands notes remained in Evernote. In their place, I now have **11,278 plaintext files** and a completely new way to write, learn and organize my work. 

Over the years, my personal usage of Evernote had grown to cover more than just note-taking and journaling. I had come to depend on Evernote as the "Swiss Army knife" of my productivity tool kit. For example, I had used [Evernote as my task manager](http://www.markwk.com/gtd-with-evernote.html), [Evernote as a read-it later app](http://www.markwk.com/2016/11/tracking-article-reading.html) like Pocket or Instapaper, and even [Evernote as a sales and networking CRM](http://www.markwk.com/evernote-crm.html). Evernote's mission to "capture everything" had largely became how I used the tool.  

Unfortunately, a few cracks started to appear with Evernote and my usage. First, my Evernote notes had become a bit of a monster, both conceptually and organizationally and in terms of the total number of notes. I felt a desire to to refine my note taking process and to slim down the number of notes I had. Second, Evernote as a product and company had seen better days. 

The problems with Evernote as a company and as a product are not really the point of this post. But a quick summary of Evernote problems will often include: pricing changes, feature bloat, privacy around your notes, significant corporate changes, lack of product additions, and poor product performance (at least for me on Desktop). 

Personally I rarely had much of an issue with the product or paying for a great product, like Evernote.  But these concerns had built up over time and formed into on-going questions like: **What's going on with Evernote? Is it time to leave? How can I migrate? What should I migrate to?**

A couple of months ago I finally decided to explore some Evernote alternatives and how I might migrate my notes.  There are some solid Evernote replacements but I elected to switch to my notes to plain text files. Though Evernote's corporate and product issues played a part in my decision too, my shift to plaintext files was less a rejection of Evernote, and more of a push to change up my way of organizing and working. To be clear: **My goal was not to replace Evernote but to evolve my systems**.

Migration is not an insignificant undertaking. Evernote makes your life easy for collecting, jotting ideas and then finding your old notes and documents later. If you have been a heavy user of Evernote, you likely have hundreds, if not thousands, of notes. Migrating to a new system is a time-consuming effort, and you still need to consider and adjust to your new way of working too. 

There are several ways to migrate off of Evernote and onto another tool. One of the easiest note-taking tools to import into is [Bear](https://bear.app), a Mac/iOS markdown notes app. Lifehacker has a decent, though somewhat dated, [post](https://lifehacker.com/how-to-jump-ship-from-evernote-and-take-your-data-with-1782841075) sharing several approaches for migrating to Microsoft's OneNote, Apple Notes, or Simple Notes. Unfotunately none of these approaches work for migrating off of Evernote and onto plain text files. Even the best script, [Ever2Simple](https://github.com/claytron/ever2simple), won't keep your images, tags and meta-data when migrating to txt files. Losing so much information from my notes was a non-starter for me and forced me to find a new approach. 

Fortunately, as I'll show in this write-up, with a couple of steps and a combination of tools and scripts, you can effectively export your entire collection of notes out of Evernote and into markdown plaintext files. Most importantly, you can also still preserve the essentials of your old notes like images, tags, and even metadata like date created. Yoou can also maintain your legacy Evernote links between notes. 

In this post, I'm going to show you how to migrate your notes out of Evernote and convert them into a collection of plaintext files in markdown. I'll provide be providing a step-by-step guide to exporting out of Evernote and and processing into a format that you can open on any markdown editor. Additionally we will be sure to keep the images, links and meta for your original notes. Along the way, I'll share some tips and my way of doing it too. At the end, I'll conclude by briefly sharing a bit more about why I left Evernote and a few aspects of my new plain text life. 

Let's get started migrating our Evernote Notes! 

<!--more-->

## Post-Evernote: Step-By-Step Migration Guide: 

### How to Migrate Your Evernote Notes, Images and Tags into Plain Text Markdown Files

First off, it's worth mentioning that for heavy users of Evernote migrating off of the platform can take some time. In my case, it took me about several sessions over about a week to accomplish it and a total of about 8 hours. 

This was partially due to figuring out the best way to migrate my notes, which I'll share with you, and a few false starts. I also spent some time developed a couple bash scripts to optimize my system after. Specifically I wrote a script to track my plain text notes daily in git and a script to create an index file of notes with a tag. 

Overall, I'd estimate that someone with about 4000-5000 notes in Evernote can complete the migration process in 2 or 3 hours with the majority of that time being spent waiting for the importing and exporting processes to complete. These numbers largely depend on how many notes and images you have and the processing speed of your computer. 

I recommend first experimenting with a sub-set of your notes, before attempting the full migration. For example, start out by exporting a single notebook or tag of notes. Go through the steps one by one to see how it works and confirm the end notes are in the format you need. Once you've done it once or twice, you should be ready to do a larger selection of notes. 

#### Getting Ready: Download Your Tools

{% img center /images/2018-resources/evernote-migration-tools.jpg %}

We will be doing the migration locally using the Desktop Version of Evernote on a Mac.  While we won't be using Bear to edit our notes after, we will use Bear as the primary helper in migrating off of Evernote. 

So, go ahead and download the following free tools:

- [Bear](https://bear.app)
- [Name Changer](https://mrrsoftware.com/namechanger/)
- [MassReplaceIt](http://www.hexmonkeysoftware.com/)

Additionally if you prefer and are a decent command line or bash scripter, much of the files cleanup process can be accomplished there. I chose these tools to provide more accessiblity to less technical users. 

#### Evernote Preparations: Cleanup Your Notes Library 

Before you start migrating, I recommend you spend a bit of time surveying your notes in Evernote. Try to see if there are some things you can delete and any necessary changes you might make organizationally too. 

While you can do many of the same changes and cleanup post-migration, it is probably easiest to do while your notes are still in Evernote. 

Personally, I spent 30 minutes deleting about 3000 legacy notes I no longer needed from when I used [Evernote as a GTD task manager](http://www.markwk.com/gtd-with-evernote.html).

#### Evernote Preparations: Tags Cleanup and Renaming

Tags are important in Evernote and will remain so post-migration. But since everything is just text, you'll want to ensure a few conventions are followed. 

The gist of it is that you want the tags in your files to have no spaces. Spaces in tags (and files for that matter) make search and references harder and more error-prone. While you can get around this limitation with some clever scripting, things will be simpler if your tags have no spaces and you avoid special characters like !$%^&. 

So, in the step, go to Evernote and into the tags section. There you should edit your existing tags to remove any spaces and crazy characters. Editing the tags there will universally change them on any previous content you tagged. 

In terms of how to tag with spaces, you can either switch to CamelCase tags or put in underscores. It's up to you. Both will be fine.  

{% img center /images/2018-resources/evernote-tag-updates.jpg %}

In my case, I had a lot of tags, so my tags cleanup took a bit over an hour to complete. 

#### Evernote Notes Export

While some people might have worried about data-lock-in with Evernote or even if it was possible to get your data out of Evernote, I've long respected how open Evernote was about letting you get your data. As one executive was reported to have said, you typically don't want to live in a country that doesn't let you leave, so you should use products that let you get your data out too. 

Evernote provides strong data accessiblity. You can get your notes data from either the API or using the desktop export. There are some limitations with the API method. 

On the desktop you can either export notes by selecting them in bulk and exporting the selected notes OR you can go into the notebooks section and export an entire notebook. 

On the desktop version, get some notes by exporting either an entire notebook or selecting some individuals notes. Once selected, right click and select the option for "Export Notes." 

{% img center /images/2018-resources/evernote-export-notes.jpg %}

For the format, select Evernote's XML .enex format and be sure to include tags. 

{% img center /images/2018-resources/evernote-export-format.jpg %}

While it's possible to export everything at once, in my case, I exported my notes in a few batches. I mostly did this to check my process and save processing time. But also by separating things, I could ensure I kept things properly organized and sorted in my new setup. For example, writing notes were separated from articles read. 

Depending on the number of notes you export, it might take several minutes to export your notes and attachments from Evernote. In the end, you should have a .enex file. 

#### Import Evernote Export into Bear

Using your Evernote export file, there are several options now. If you are switching to a new note taking app, there should be an Evernote importer tool you can use. In our case, we are going to use Bear to help us with the migration to plain text files. 

Bear is considered one of the best markdown editors for Mac and iOS. It also does an amazing job importing Evernote notes. So, while our ultimate goal is plain text files, we will use Bear to convert the text to markdown syntax, preserve images and generate tags too. 

Inside of Bear, go into FILE > IMPORT FROM > EVERNOTE. Then, select your previously exported evernote file. 

{% img center /images/2018-resources/bear-export-notes.jpg %}

Importing from Evernote into Bear might take some time, especially if you have a lot of notes, tags and images. For example, for my biggest import of around 8000 notes, it took 20~30 minutes to complete. 

#### Additional Tags and Cleanup of Notes in Bear

If you did a good job cleaning up your notes in Evernote, you can proceed to the next step. But you may want to apply a tag to your existing notes before exporting. Bear and your eventual plaintext files have a flat-structure and everything is basically organized through tags. So, you may want to add a notebook tag for whatever was the equivalent notebook in Evernote. 

To add a tag, select your notes and then drag them onto the target tag. This will then bulk add a tag to all of those selected notes. This can take a bit of time as well as Bear updates each file one by one. In one case where I updated 1000 files at once it took 10 minutes. It is probably best to update tags in small chunks. But either just be patient since while Bear might appear frozen, it mostly likely is still just processing the files. 

#### Export out of Bear into Plain Text

Now that we've exported our notes from Evernote and imported them into Bear, it's time to export them back out as plain text files. The main reason for using Bear is that unlike some existing scripts, Bear does a great job converting Evernote syntax into markdown, and it also preserves tags, creation date, and images too. 

Inside of Bear under FILE select the option for export notes. Select a new directory to export your notes to and make sure you select the Markdown option under "Export As" and tick the box for "Export attachments." 

Exporting from Bear is the most time consuming step. Depending on the number of notes, exporting from Bear to plaintext files can a few minutes or several hours. 

As a point of reference, for my final batch of about 8200 notes, the export out of Evernote and into Bear was not noticeable, maybe 30 minutes. But the exporting from Bear to files was VERY noticeable. 

According to my logs, it took over 8 hours to complete. Bear was exporting around 6 and  12 notes a minute. This might have been optimized through smaller batches but since I saw the process was not stalled and files were exporting every few seconds, I just let it run all night. 

If you have 1000 notes to export with images, it's a fair bet to guess this will  take between 1h and 1h20. You can extrapolate beyond that. 

#### Separate Out and Move Exported Images Directories

If you've completed the following steps, congrats! You now have exported your notes from Evernote and into plain text files. Now all we need to do is a bit of cleanup and organizational work. 

By default, Bear will export the text files and attachments into a single directory. I prefer to keep the text files and  images separate. So, while optional, I recommend moving all of the attached files and directories to a new location. 

Go ahead and drag and drop them to wherever you like and note the new location since we will using that to update image references inside of the notes later. 

#### NOTE about File Renaming and Processing

In the next couple steps, we are going to be cleaning up our exported files. The first part will be renaming the file titles and the second will be modify the contents. 

*One quick warning. If you plan to append the creation date, which I recommend, make sure you run this step BEFORE you bulk edit the contents. Most techniques to update file contents will result in a new file and thus you will lose the original creation date on the new file.* 

#### Process Files to Replace Spaces to Underscores and Remove Commas

Technically, while it is not necessary to rename your files, it's a recommended best practice. This is especially true if you'll be managing and processing your files to some extent on the command line. Basically, removing spaces in files will make your life easier. 

There are a few ways to rename files, including using the command line or some bash scripting. We are going to be using the Mac app, Name Changer, to quickly cleanup our files. 

So open up Name Changer and drag or add your files. Then select the option *Replace All Occurances with*. In the first field put a space and in the second add an underscore. 

{% img center /images/2018-resources/renaming-files-example.jpg %}

Then run the "Rename" command to bulk update the files. After that I advise you to **remove apostrophes, commands and semi-colons**. 

#### Process Files to Prepend with File's Creation Date

One of the cool things Bear does in exporting your notes is preserve the creation date. Since Bear assigns the creation date when you import Evernote notes, that means your final exported file will still have the  original date that note was created in Evernote. Glorious!  

In order to preserve this metadata going forward, I'm going to prepend this to the actual file. Using Name Changer, select the date option. Then use file creation and paste in the following Format: YYYYMMddHHmm. 

{% img center /images/2018-resources/renaming-files-by-date-example.jpg %}

After running the command, you will now have prepended the date and time the note was originally created. This date format will put the year, month, date, hour and minutes at the start of the file and effectively you'll have a unique identify for your notes going forward

#### Update File Contents with New Images Paths 

When you export your notes from Bear, it uses a local path for the images. This works ok, but, as I noted, I prefered to move my images into a special directory and update the paths to an absolute path on my computer. In order to do this, I used MassReplaceIt. MassReplaceIt is quite similar to Name Changer but with one key difference, you can edit the actual contents inside your files.

Inside of MassReplaceIt, create an action to Find ![]( and replace it with ![](/my-path on the computers/. Basically what we are doing is modifying the markdown syntax for image urls and assigning it to the new directory we placed all of the exported images in. 

Here is what I mean: 

{% img center /images/2018-resources/updating-image-paths-in-files-1.jpg %}

After that, be sure to configure your options so it searches contents of the entire file. 

{% img center /images/2018-resources/updating-image-paths-in-files-2.jpg %}

After you've reviewed it and maybe tested it on a single file, go ahead and run the command:

{% img center /images/2018-resources/updating-image-paths-in-files-3.jpg %}

The end result should be updates to all of your files with hopefully the image paths corrected. 

#### Check Sample Documents in a Markdown Editor

Now that you've cleaned up those files, it's time to check some of the files. Using your favorite markdown editor, open up a few of the exported and processed files to check that everything looks ok, including tags and image paths. 

Here are two of my sample note files: 

{% img center /images/2018-resources/evernote-to-plaintext-exported-files-example.jpg %}

As you can see it's included the title, embedded images and my original tags at the bottom too. Awesome sauce!

(FYI -- While honestly there are a ton of great markdown and text editor apps available today, two of my favorite markdown editors on Mac right now are [Typora](https://typora.io/) and [MacDown](https://macdown.uranusjr.com/). Both provide options for viewing inline images, which is great feature for me. I also use [The Archive](https://zettelkasten.de/the-archive/) to help me stay organized and search by tags inside of the text.)  

#### Move Markdown Files to Your Preferred Directory

{% img center /images/2018-resources/file-organization-post-migration.jpg %}

Now that we've got our files processed and ready, it's time to move them to their own directory. 

I recommend storing your files in a cloud-synced folder. Dropbox, Google Drive and iCloud all work great and will allow you to view and edit your files on the go. For a great markdown editor on iOS, I recommend [1Writer](1writerapp.com), which, besides being a solid editor and viewer of markdown files, has some nice bonus features like a tag viewer option.  

How you organize files going forward is up to you. But for an example, I elected to not put everything into a single directory but split my exported notes into three directories: 1. my knowledge notes and writing drafts, 2. project notes, (including notes on goals, actual projects, habits and study notes), and 3. an "everything else." This split allowed me to avoid mixing up my core working notes and a bunch of legacy stuff I still need to better sort and organize over time. 

#### Tips for Managing Your Evernote Migration Process

Congratulations! If you've gone through these steps and managed to get your notes into plaintext with working images and tags, you've already taken a HUGE step towards app-independent files and future-proofing your data. 

Here are a few additonal tips as you start or continue migrating your files and setting up your new systems:

1. **Use a new tag to track what you've exported from Evernote**: In my case, I was migrating a lot of notes. So I added a tag inside of Evernote to the notes after I had migrated them. This was a kind of sanity check and made it possible to log my progress. For example at one point, I had migrated 707 notes and 13,319 remained but about a week later, I had migrated 11,278. I was able to track this through post-migration tag in Evernote. 
2. **Create a checklist for your migration**: I recommend setting up a checklist for your migration process. Feel free to adapt from my steps above. Checklists are great since this makes it easier to be consistent during the migration and not miss something important (which I did once or twice and had to roll back). 
3. **Keep a List of What to Export and What's Completed**: My initial start was migrating my drafts into plaintext. As I embraced a complete plaintext setup, I eventually decide to export everything. It seemed pretty intimidating at first, so I made a list of the different note types, tags and directories I wanted to export. I worked through that list one by one over a week and ensured the new setup was well organized for each exported type. I'm obviously still tweaking the end result, but having a list of what was done and what was to do keep my eye on the ball. 
4. **Think of Your End Goals and Usages to Determine How to Organize Your Files**: While it is possible to export everything into a single directory and use tools like The Archive or nALT to stay organized after, it is beneficial to think about your end goals and intended usage before and during your migration process. In general, you probably should avoid too many separate directories for your files. At the same time, some organizational divisions can be great mentally and helpful long-term. Depending on your needs, take a moment to decide where stuff should go, some tags you might add during migration and what your goals are going forward.  

For my purposes, my primary goals were 1. to setup a better system for knowledge notes and for my writing drafts (a.k.a. my own Zettelkarten) and 2. to organize my notes in a way that made it possible to track my usage (writing vs. coding vs. project management). As such, I elected to store my files in a four different directories initially: 

- **Coding Notes** = ship's log of daily coding jobs and a collection of tool and programming notes. 
- **Project Notes** = Essentially everything is a project, and I use a note to keep track of stuff, make notes and draw connections. This includes notes on my goals, actual projects, studies, etc. 
- **Knowledge/Drafts** = These are initial writing drafts and my actual smart notes organized into an archive or Zettelkasten. 
- **"Everything else"** = For legacy purposes, this where my collection of random articles and notes ended up. A lot of will be deleted or folded into other places, but I still need to sort and clean it up first. 

Ultimately, migrating off of Evernote could be a huge decision. So, take your time. Initially experiment with one aspect of your note taking or writing using a new tool or approach. After awhile figure out what works and doesn't and then make adjustments. There might even still be situations where you'll continue to use Evernote, as do for collecting things. 

## Conclusion: Don't Replace Evernote, Evolve Your Process

As a long-time "power user" of Evernote, I've gone from imagining Evernote as my one and only "desert island" tool to watching what appears to be a sinking ship. 

I've used Evernote as my preferred tool for a whole range of functions, and I would have continued to do so. But recently, like many others, I became worrried by Evernote's lack of privacy, its corporate turn-over, and its lack of serious product development too. My personal experience of the product has soured somewhat as it had become slow and laggy on Desktop. Its on-going lack of support for markdown remained baffling too. These concerns eventually led me to explore alternative tools and consider how I might migrate my notes. 

In this post we looked at how to migrate your notes out of Evernote and into a collection of plaintext files in markdown. The essence of it could be summarized like this: Use Bear to process Evernote notes into Markdown files while preserving meta-data, links and images. Afer exporting out of Bear to plain text files, use Name Changer and MassReplaceIt (or command line scripts) to first update the filenames and second to fix image paths. Depending on the number of notes you have, the migration process might take several hours to complete.

**Whatever your reason for leaving Evernote, one thing I recommend keeping in mind is that you should avoid looking for an exact replacement for Evernote**. If you want an Evernote replacement with the same features, you are better served continuing to use Evernote and avoid torturing yourself with lesser products. Evernote is one of the most amazing software products ever developed, and it fulfills its stated mission to help you capture everything, including notes, photos, documents and more. 

In the end, it wasn't so much a cost, product or company issue with Evernote that convinced me to change; it was a re-thinking about my approach to note-taking and my on-going effort to "track everything" and make data useful. Let's conclude by looking at these two points one by one.  

Regarding note-taking, for the last several years I've become a bit of a digital horder. I love collecting and generating data. But as I shared in [The Power of Systematic Notes: A Book Review of How to Take Smart Notes](http://www.markwk.com/smart-notes.html), collecting stuff is an easy (and, in my case, rather addictive) behavior and just because you have a note or article doesn't mean you learned anything or created something useful for later. I've come to realize the importance of priorizing *creating over collecting* and *on learning and knowledge development over filling up notebooks with junk*. Basically, as learners and creatives, we should all aim to write more, take better notes, and to build a connected and usable system from those notes and drafts. Evernote made it a bit too easy to collect and by switching to plaintext files I was able to develop some better habit. 

Regarding my data and self-tracking, there are a lot of advanatages to using text files. They are flexible, simple, and future-proof. I can open and edit them anywhere, and, with cloud syncing, I can use text files on any platform too. As a blogger and writer, text files in markdown syntax allows me to quickly convert the text for web, a pdf or even an ebook. As as a [self-tracker](http://www.markwk.com/category/track-everything/), plaintext files now makes it possible to track my writing and project notes in a new way too. Using a [bash script and Git to track my notes](https://gist.github.com/markwk/c85a8a72bc8c03d0f510262bb5219a34), I can track how many words I type on different types of notes and whether I'm spending more time on project notes, coding notes or writing notes. This is useful data to optimize and get feedback on my productivity and creativity. 

Initially a few factors at Evernote itself led to me look for alternatives, but it was this desire to change how I took and organized my notes and to track my writings in a new dimension that convinced me that the best choice for me was not another note-taking app but plaintext files. 

As I explored in this post, migrating off of Evernote takes some time and work, but it can be empowering too. With plaintext files you no longer have to worry about compatibility and the future of your data. You can focus on creating rather than collecting, and hopefully if done thoughtfully you can create a system for your own creative, organized mind. 

<br/ >

Best of luck and happy migrating!

<br/ >

*PS -- How did migrating off of Evernote go for you? And how do you plan to manage your notes going forward? Send me a note or drop a comment below!* 





