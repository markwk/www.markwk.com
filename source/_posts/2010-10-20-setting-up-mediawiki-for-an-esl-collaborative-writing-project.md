---
title: Setting Up MediaWiki for an ESL Collaborative Writing Project
author: Mark Koester
layout: post
permalink: /2010/10/setting-up-mediawiki-for-an-esl-collaborative-writing-project.html
blr_date:
  - 2013-04-18
categories:
  - China
  - ESL
  - Teaching
  - Technology
  - Web Development
comments: true
---
# 

{% img center /images/wp-img/wwr-logo-large.png "WikiWriteRight logo for ESL wiki on collabrative writing together in Chengdu, China" %} 
 
As I mentioned a couple days ago, I've been [thinking about how to use technology in my classroom teaching](http://www.markwk.com/2010/10/using-technology-in-teaching.html). Over the last couple days, I setup my first wiki project: [WikiWriteRight](http://markwk.com/teaching/wwr/). It's a wiki for my students to be able to draft and revise their stories collectively.

I have used PHP-based web application for about a year now. I understand the basics of setting up my own CMS (Content Management System) as well as using systems like WordPress, Drupal and Joomla. This current blog is run on WordPress, which is a very easy and adaptable system for blogs. As a blogging and content management system, these all have their place, but they are not wiki, though they are adaptable for some wiki-like functions.

A wiki, if you didn't already know, is web page that can be edited and created by anyone. The biggest and most famous example of this technology in action is [Wikipedia](http://www.wikipedia.org), which currently boasts, as of August 2010, 3,400,000 articles in English alone. Excluding a few paid positions, which go with any large project, Wikipedia has been amazingly almost entirely created, edited and managed by volunteers. Since reading The Wikipedia Revolution a couple months ago, I came to understand the power and potential of this kind of technology adapted to a collective goal managed and run through individual actions. It is almost unbelievable that this project succeeded as it has. Since then, I have been wondering how I might put wiki technology to use in my life and in my projects.

## The Situation: Getting Students to Write and Edit Together

I currently teach *English Writing* to Chinese Business students at a well-known university in Chengdu. Like most young people, my students are keen on technology, and, unlike my previous teaching at a different university, these students are quite motivated to study and learn. The students are interested in practicing their English, and they do, indeed, enjoy giving me their homework to look over. But there is one major problem: they don't like revising and editing their homework. In fact, I think they hardly even re-read their homework before turning it in.

While I have no difficulty correctly their errors, it pains me to see those errors repeated. The cycle tends to go like this: 1.) They do their homework and give it to me. 2.) I correct and return their homework to them. 3.) They look at what I wrote and corrected. Unfortunately, what happens next is the hard part. When I assign them a new exercise they tend to repeat the same mistakes: they don't check that verb tenses match; they misuse the same terminology; etc. En bref, they don't learn from their mistakes. One of the reasons they don't learn from their mistakes is the failure to re-read and revise their homework.

Revision is a key component in writing and learning to write. Ideally, I would have students work together to revise each other's homework, but in a Chinese context, this is a somewhat culturally delicate affair since friends don't want to seem critical or disapproving of their friends. It's a delicate balance.

To summarize the situation: My students need a way to write and revise together, and as their teacher, I need a way to provide corrections and track their changes and corrections over time.

## The Solution: "WikiWriteRight," a wiki for collaborative writing and editing for ESL students.  
 
In order to meet this situation, I decided to try my hand at using Wiki technology and created [WikiWriteRight](#). I tried a couple wiki systems before settling on MediaWiki, which is the open source software that runs Wikipedia. MediaWiki has been perfected and worked on by a large group of people, and it has successful run on of the largest internet projects in history. Unlike other PHP-based CMSs, MediaWiki isn't trying to satisfying everything and, in the end, do nothing particularly well. MediaWiki is an extremely powerful wiki platform. It keeps track of changes and additions to pages. It provides a discussion page for debates between writers and editors about what to change. And it is relatively intuitive to use. There are some strange editing features like creating headlines and links, but more or less, it is a "what you see is what you get" system.

To test and setup MediaWiki for this project, WikiWriteRight, I setup a MySQL database and installed MediaWiki locally on my computer. I setup of three user accounts: a systems administrator or, in Wiki-talk, a "bureaucrat" account (WikiSyops) with all privileges, a simple administrator account (TeacherMark) and a simple user account (SampleStudent). I then began write and setting up textual elements of my wiki.

One of the first difficulties I ran into was understanding how to write and format my text in the editor so it would look and act like I wanted. While it should be clear from the above that I consider MediaWiki to be a very capable and robust system for creating and managing wikis, it's editing system is a little bit confusing initially. Once you get an idea how it works, it is extremely simple and not particularly difficult to use or understand.

One of my worries when I begin implementing this system with my students in the coming weeks is their ability to understand the somewhat confusing editing of a wiki page. Hopefully, if during the first classes I am able to successfully explain what is a wiki and how to use one, then the rest of the project should be fine. In order to ease the use and implementation of this project, I have written numerous instructional pages (as well as links to Chinese versions on other sites) and created a sample project for them to use as a reference to know what they should do. I hypothesize that most of my students will have little difficult getting used to this system and might even take some pleasure in the technical side of it all.

I think one of the more powerful features of wikis is the history page. When we use and read entries on wikipedia, we are almost never aware of the process that went into building these pages, but once you open up the history page, it becomes clear all the hands, eyes and brains that went into a single entry. As a teacher, I think the history page will hopefully provide me and my students a better way to track and follow their progress in this collaborative writing process.

Along with the core setup and initial pages, from a technical perspective, I also added a couple changes and extensions to my wiki in order to improve the use for my students:

1.  I created a logo and added it the basic layout.
2.  I activated the upload function.
3.  I added a more organized forum-like extension to the discussion page to make it easier to use and more understandable.
4.  I added the Google Analytics code in order to track and follow user stats.
5.  I added a voting system, which will allow my students to vote on which stories they think are the best.

** Initial Conclusions: Using Wiki Technology in an ESL Context for Collaborative Writing**

For someone who is reasonably computer savvy, setting up a wiki using MediaWiki is pretty easy. There are a few quirks to improving the use of a wiki including adding some useful extensions, but I think overall it is fairly intuitive and well-built system.

From my personal perspective as a teacher and web designer and developer, I think this technology has a lot of strengths for a teaching environment. A teacher can setup the basic pages by themselves and, after some initial explanations, students should be able to self-manage their projects. Once the project has started, a teacher can easily follow the progress of their students work by reviewing the history pages, and a teacher can either suggest directly make changes on the page itself or suggest changes on talk/discussion page. From a pedagogical perspective, I think the system encourages participation and will hopefully solve some of the difficulties in getting students to revise and perfect their work.

The major problem and difficulty I have this using MediaWiki in a teaching context is that it slightly too complicated for a teaching environment. I suppose if I had more time or were to do this project again, I could revise the template pages to remove certain information and links and to change the complexity of the layout. The main difficulty I think is that the page presents too much information and too many choices without directing students to which activities that should do and use. One change I am considering adding would be adding a way to associate students with certain pages. Once they are attached to a certain page or project, a sidebar box could be built that indicates activities that they can and should do.

Overall, I look forward to putting this project into action, and I will provide updates soon on how it goes. I'm interested to hear your ideas and comments.