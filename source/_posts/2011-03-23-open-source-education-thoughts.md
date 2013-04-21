---
title: 'Open Source Education: Thoughts'
author: Mark Koester
layout: post
permalink: /2011/03/open-source-education-thoughts.html
blr_date:
  - 2013-04-14
categories:
  - Drupal
  - Education
  - Language
  - Learning
  - Technology
  - Web Development
comments: true
---
# 

Since early at the beginning of this semester (2010-2011), I started thinking about how to use more and better technology in my classes. I have taught for a number of years, but I was not longer satisfied with merely providing a classroom setting for learning. **As a teacher, I wanted to make sharing information easier and collect assignments more efficiently. For a students I want to create a more interactive way to communicate and learn and perhaps build something to improve learning in general beyond the classroom setting.** With these goals in mind, I started teaching myself internet technologies and implementing different solutions.

Ironically, my own work developing online resources for my students and my study of internet technologies reflects I think a broader and older transitions in open education education: from static to interactive, for closed to shared and open, for localized to distributed and global.

I have blogged and written online for a number of years. A year after coming to China, my blog moved from blogspot (since Google blogs got blocked in China) to my own hosting using wordpress. So, since I had my own hosting space, I could start experimenting. I started by adding a simple html site/space for me to post articles and resources from class. I played with ideas of creating a better and more useful display of information via javascript. I even imagined being to stop using powerpoints and create slides via a jquery transitions setup.

This initial efforts with **static html **were difficult to manage and required me to ftp files and changes. It wasn't particularly attractive, nor interactive. Students could indeed access resources but not much else.

[![Teacher Mark's Teaching Site, Version 1][2]][2]
Teacher Mark's Teaching Site, Version 1

Since Chinese students have little experience nor training working groups, I wanted to find a way for groups to work together well. My next step was a Wiki project using MediaWiki. After reading *The Wikipedia Revolution*, I was inspired by the idea that disparate individuals could contribute and edit in a way that could be beneficial as a community or group. So began ***WikiWriteRight*, a collective ESL writing wiki. **

 []: http://www.markwk.com/wp-content/uploads/2011/03/Screen-shot-2011-03-23-at-4.08.54-PM.png

** **[![WikiWriteRight, a collective ESL writing wiki][3]][3]**
WikiWriteRight, a collective ESL writing wiki

After explaining briefly the nature of a wiki and dividing students into groups, we worked on writing stories together. [As I recorded elsewhere][3], there were positive and negative points in the project itself, in my shepherding of the student groups and in the technology itself, but the main achievement was getting students to work better together. The main lesson I learned as a teacher and educational technologist was that there was a strong interest amongst a large percentage of Chinese students learning English to use technology for learning, in particular social media focused tools.

In my mind a new goal emerged that I would later learn the name for: **a social learning environment**. The purpose of a social learning environment is to provide an interactive and collaborative space for students and teachers. This kind of space encompasses the need to engage modern needs of students in today's world driven by internet information in general but social media in particular.

I toyed with building the project myself from scratch using PHP, but with various open source software and tools available today, starting any project with a single line of code is absurd and stupid. I looked at the various platforms available including Moodle, WordPress and Drupal. While Moodle has a number of great features, it is too focused on a specific educational use case. WordPress also failed to meet my needs, because it is a blog site and not as easily adaptable. Drupal with its healthy community of modules (addable function units) proved to be great starting point.

Drupal is relatively easy to get up and going but it isn't the easiest system to get your head around quickly in some its more complicated development aspects like Views. Fortunately, Drupal has tons of documentation and reading and video resources. I worked on a couple, non-education sites so I came realize some the power and potential with Drupal. After I started looking at various distributions (specific installation configurations of Drupal and modules and themes) that give you a specific use case situation.

I looked at Aquia's *Drupal Commons*, Development Seed's *Open Atrium* and eventually *EduGlu* and Penn States's *ELMS*. While Drupal Commons and Open Atrium are sophisticated, multi-developer projects for large institutions, they are open source so their code is completely available for changing and learning. These Drupal distributions keyed me into some the important modules, development setups and general "architecture" for working effectively with Drupal (specifically, organic groups (og), context, spaces and features).

*EduGlu* and *ELMS *are two educational distributions looking to answers some of the same questions I have been looking for technological solutions. Namely, both use Drupal to create a powerful sharing and learning space. I have for the last few months been working on top of or within EduGlu, a discussion focused distro. While EduGlu is extremely powerful discussions and information sharing, it feels still immature in its concern for more traditional teacher needs (like organizing classes, collecting assignments and a gradebook). It is also somewhat lacking in providing an individual social space for students. These are two areas I have been working to extend EduGlu through my own features.

The result: [**Language-Corner.org**][4]:

![Language-Corner.org Welcome Page][5]
Language-Corner.org Welcome Page

While there are numerous changes I want to make, it is clear that this is a strong basis from which to construct an innovative learning space for foreign language learners, teachers and groups. The site is based on the simple idea that classes and groups need their own customizable space. From there, groups add the features they need to make learning more effective. So, while some classes might function as a simple exchange point of information, other groups like my own classes are more focused a richer experience of interaction including discussions, exchanging photos and videos and even class polls.

Here is screenshot of my group and the features that are configured:

[![Teacher Mark's Teaching Site, Version 2.0][7]][7]
Teacher Mark's Teaching Site, Version 2.0

One specific feature I added to my site is called **"Words." **This simple addition allows group members to add new vocabulary (including an image, a definition and a translation) and then students votes on the results. While I'd like to extend it into a more engaging and effective learning experience (perhaps through something like flashcard interactive display), this simple feature has proven to be incredibly engaging and effective in a communally, student-driven way. Since adding it a couple weeks ago, students have add several dozen words already:

[![Words added by students for English Writing 102][8]][8]
Words added by students for English Writing 102

As so well noted in [this post by ELMS's "one man show" developer][8], one of the things technology created for education situations often misses is that **it's all about and for the students**. In developing information and educational technology for the web, we need to keep this main objective in mind. Also we need to continually ask two questions

1.  **How will this improve education and the educational experience for students?**
2.  **In relation to what we've made and developed, does it work? How can we make it better?**

I hope to continue to develop my educational site, Language Corner, for students as well as participate in the broader work of building and improving educational software for Drupal around the world. By building and improving on things in our own way but in a shared context, everyone benefits.

 []: http://www.markwk.com/wp-content/uploads/2011/03/Screen-shot-2011-03-23-at-4.09.19-PM.png
 [3]: http://www.markwk.com/2010/11/working-together-wiki-esl-writing-project-update.html
 [4]: http://language-corner.org/
 [5]: http://www.markwk.com/wp-content/uploads/2011/03/Screen-shot-2011-03-23-at-5.36.51-PM-300x160.png "Language-Corner.org Welcome Page"
 []: http://www.markwk.com/wp-content/uploads/2011/03/Screen-shot-2011-03-23-at-5.35.23-PM.png
 []: http://www.markwk.com/wp-content/uploads/2011/03/Screen-shot-2011-03-23-at-5.53.38-PM.png
 [8]: http://btopro.wordpress.com/2010/03/16/open-source-learning-environments-theyre-about-students-dumby/