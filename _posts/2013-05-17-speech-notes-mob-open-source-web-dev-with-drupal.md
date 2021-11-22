---
title: "My Story Learning Drupal: How I Got Empowered by Drupal's Site Builder CMS"
author: Mark Koester
layout: post
categories:
  - Learning
  - Drupal
  - Speech
  - Technology
comments: true
published: true
---

I consider myself extremely fortunate to have landed on Drupal so early in my web development learning journey. Drupal was a technology I was able to start using very early without any programming skills and still was able to create real, working websites for myself and others. It's still a technology I encourage generally tech-phobic people to try since it can be extremely empowering to build and customize your own site, instead being forced to hire out the entire web application build process to an external company or programmer.

![](http://farm8.staticflickr.com/7283/8744276103_a1f762559f.jpg)

A few days ago, I gave a presentation on _[Introduction to Open Source, Web Development with Drupal](https://speakerdeck.com/markwk/intro-to-open-source-web-development-with-drupal)_, which I embedded the full presentation below and will hopefully post the video soon.

The presentation itself covered quite a few general introduction points (what is a CMS, Drupal vs. WordPress, and Drupal as a "Site Builder CMS"), but mainly I wanted to show the attendees that you can actually build stuff without knowing how to code, so I did a live demo creating a members directory for the co-working space where the event was hosted. Live demos are tough sometimes, but this one went quite well. I was able to cover what I consider the two keys to using Drupal: adding fields and managing data display by using Views.

While I mentioned it during the presentation, one of the points I don't think I covered fully enough was how I went from basically knowing very little about programming and web development to running [my own Drupal web shop](http://int3c.com). Just a few years ago, I was basically a novice to Drupal and web technologies in general, but through curiosity and a few "failed" projects, I was able to learn an amazing amount about Drupal, site building, information architecture, project management and slow-but-surely php module development.

When someone asked during the question and answer part at the end, "How do you recommend learning Drupal?," my answer gave two suggestions: First, I suggested that the best way to learn is to have a project or something you want to build and then try to build it with Drupal. This advice is valid for any new technology you want to learn. It's tough to learn something without having a clear situation where you'll use it. Second, I provided a few decent resources for learning Drupal, including Lynda.com's Drupal 7 video series, Drupalize.me and the book "Understanding Drupal." I also praised how helpful and kind the Drupal community can be towards newbies.

In this post about Drupal (which I normally blog about [here](http://int3c.com/blog)), I'd like to discuss how I came to become a web developer and site builder. It's the tale of a couple "failed" businesses and my effort, in spite the setbacks, to "build it myself" using open source technologies. Finally it's a bit of a "love story" in how I came to embrase Drupal and develop a business around this open source, site builders CMS.

<!--more-->

## My First Web Application That Was Never Built: DIY-Abroad.com

{% picture right /images/2013-resources/diyabroad-logo.png %}

In 2009/2010, I was living in Chengdu, China. Full of ambition and pure naiveté, I wanted to start my own business. I proposed and developed various ideas and projects, including a newspaper, a language school and an overseas education agency. It was pretty tough process and there were a lot of failures and constant setbacks. Those business failures and the lessons learned are perhaps worth writing about in another post someday. What I want to talk about is how these "failures" lead me to learning Drupal.

During that time, I was also handling the presentational websites for each of these projects. Like almost everybody that doesn't know better, I figured I needed a website to do business (which is not necessarily true but I thought so at the time). Originally I built these sites with HTML, then shifted to WordPress since it was easier.

As my hunger and plans grew in scale, I eventually decided on building a much more complicated web application. I wanted to build a website / app to help Chinese students better understand their study abroad choices. It was called it _DIY-Abroad.com_. There was a lot of false information going around in Chinese about the quality of universities abroad, so there was a lot of unhappy students that ended up at overpriced universities. So, I wanted to build a site about universities and their facts as well as provide a search functionality to better match up schools and students.

WordPress, which was the only web technology (besides some basic HTML/CSS) I could use at that time, didn't seem like the best choice on this new project. My needs had shifted from a simple blogging, presentational site to creating a web application, meaning I needed to build something with a lot more interactive back-and-forth. I figured I couldn't do it with WordPress, and unfortunately my web toolkit was quite limited, so I figured I'd just hire a local programmer. It's China, it'll be cheap, and at least I'll get something half-working at worst.

To be honest, I didn't even know enough _about_ technology to guide my choices. I tossed around a lot of words like PHP, java, and python like these magical words, which I didn't know the meaning of, would be enough to guide me to finding someone to help. I found someone to help who turned out to not be very helpful.

On my first real web project, I hired the wrong company. There were a number of problems with them, including many communication problems about deliverables, but frankly, in came down to them not having the skill level I needed and they didn't tell me upfront. It was also didn't help that were also terribly unaware of most open source technologies.

As I waited for them to "build" the first version, I started experimenting with a number of technologies like Ruby on Rails, Django, Joomla and Drupal. Never underestimate the power of knowing about technologies to eventually direct you towards the technology that will work best to solve your problem. Also never underestimate having a desire and enough time to learn and build towards it.

I watched videos and read articles and books, but mostly I just kept tweaking and trying stuff out. Building and rebuilding. Eventually I was able to build a very rough version of what I wanted with Drupal. It wasn't pretty but functionally, like a lot of Drupal stuff, it did the essential parts. I could create the dozens of fields needed to record school info.

But by that point, I was no longer interested in finishing building DIY-Abroad for various reasons, including a spin out with a Chinese business partner (ironically I would get my chance to work on a similar college database and search project a few years later!). Fortunately I was young, hungry, and already had a new project, a project that would get me to speak, think and even dream in Drupal: [language-corner.org](http://language-corner.org).

## Language-Corner.org: You Gotta Build to Learn

[{% picture right /images/2013-resources/language-corner-screenshot-01-thumb.jpg %}](/images/2013-resources/language-corner-screenshot-01-large.jpg)

As I told one of the hopeful Drupal learners at my speech, you really need some kind of project in order learn a web technology. In my opinion, studying a web technology without a clear personal use is a pretty good way to forget what you learned. It's essential that you plan to use or are already using that technologies when you learn something new.

For me personally, learning Drupal is closely connected to building and developing Language Corner.

As I recount in _[Open Source Education](http://www.markwk.com/2011/03/open-source-education-thoughts.html)_, I started building the initial version of Language Corner to experiment with ways to force collaborative writing between shy students. The project itself was called WikiWriteRight, and I basically used MediaWiki with a few tweaks to allow groups of students to work on writing a story together. While there were various setbacks, overall the project was a huge success and the final results was better than they could have achieved individually.

After that first semester experiment, I wanted more than just a wiki system for writing. I wanted to create a mashup of activity spaces for collaborative learning and also wanted better control and separation of different classes. At the time, one of the most significant and important Drupal distributions was [OpenAtrium](http://openatrium.com), literally an open source intranet-in-a-box. This distribution provided collaborative workspaces for project management, discussions and wiki-revision notebooks. It was extremely powerful, well-organized and beautiful.

At that time, I was looking for the next technology that I could best adapt to my needs in creating a collaborative workspace for students and teachers. I found my solution in EduGlu, which had embraced OpenAtrium's architecture in order to create a space for student learning. EduGlu provided a slightly rebranded discussion and writing space from OpenAtrium as well as some tweaks to the group or class activity dashboard.

From that setup, I created and adapted various existing Drupal contrib modules in order to work in a group space, like Quizes and a simple vocabulary sharing area. I also experimented with OpenTok to create a browser-based video chat area. All of these were interesting additions to the learning space.

Most importantly though I keep sharing back my questions, ideas and code with the Drupal community. Through this effort of using and sharing back, I was able to form relationships with several developers working in the educational space, especially with [@btopro](http://twitter.com/btopro) at Penn State and his [ELMS project](http://drupal.org/project/elms). Even though our needs differed, we were able to collaborate in mutually beneficial ways as well as validate many of architectural choices as a system.

## Building My First Modules

During the summer of 2010, I was still working on a few business projects, but mostly I had dedicated my time to refining Language-Corner.org. When the main developer behind EduGlu decided to no longer pursue the EduGlu project, I decided to use OpenAtrium and add my learning tools there. Fortunately, since the setup and underlying structure was the same, this was a pretty straightforward conversion process. I also started to share back my tentative feature code and modules to the drupal community.

During that summer, I was worked on building several new features and modules, including some of my first modules. None of these modules would win any awards or spark any developer revolutions, but they enabled me to learn by doing, which was key.

If you look at [my commit history on Drupal.org](http://drupal.org/user/1094790/track/code), you can see that my earliest commits were for several Chinese video integrations with Drupal. At the time, I simply ripped off code from a couple existing media modules and add a few key changes so they worked to embed video from these Chinese video sites. I also adapted the google plus one module to create a Weibo Sharebutton module, which even if initially was extremely rough, provided a way to create a way to share via China's homegrown Twitter.

In August, after a couple failed attempts to build my own vocabulary and dictionary system, I decided to create a module to integrate with Quizlet.com's flashcard database. It was a wise and huge timesaving change. At the time, I was trying to create an easy way to share flashcards inside of groups. For me the key was to share and view vocabulary and learning pages inside of groups. Importantly though, I first built a general purpose Quizlet for Drupal module and a secondary module for the OpenAtrium integration. This effectively made the module useable for other Drupal websites. This module also interestingly also lead to one my longest ongoing projects, [Course-Notes.org](http://www.course-notes.org).

By this point, people around me and on the internet started to notice me. I couldn't claim to be some super star programmer but effectively I had grown to the point where I could help other people in their Drupal problems. It's also when I took on some of my first clients.

## My First Clients from Friends and Family

In 2011, Language Corner started to get more attention from various teachers and students at my university and also from a few teachers outside, including teachers in the US, France and Sweden. It was an interesting time and exciting to see my site provide something useful to both students and teachers. There were still a lot of problems, most especially in usaability and in the business model.

Even though I was doing the majority of the web development and site building myself, I just didn't have enough time or skills to handle everything. So at several points during the site development, I hired outside developers to help me, especially on developing particularly ambitious areas of my site like live chat, video conferencing and ecommerce integration.

As I tell people, you should never hesitate to hire someone when you need something done relatively quickly and you don't have the skills nor time to learn how to do it, because even if you can't build it the first time, watching someone else build it for you will teach you alot that you can use the next time. Through this experience, I was able to learn quite a few new skills and develop several new features for the site.

Unfortunately, in the fall of 2011, I was starting to get low on funds for Language Corner and, while these new features would be great, they were complicated and took a lot of time to get working. They also weren't features that would save the business side of things. I still didn't really have any plan for revenue and frankly the product itself wasn't fully ready yet, though perhaps that was just an excuse to avoid getting more realistic users. Looking back, I had several notes and lists where I rationalize what was worth building, how I'd be able to afford it, and why it was necessary. I was extremely naive yet hopefully that more features would make the project "ready".

So, even as my main project, Language Corner, started to gain user traction, I was effectively lost in terms of what it could do as a business and didn't really have enough money to keep pouring money into a project without any revenue.

In spite of all the business and usabiity problems, though working on Language Corner I had been able to build a very technically demanding project. I'd also taken on several smaller "free" projects for friends and family, which had helped to expand my skillset and build different kinds of sites. While in Taiwan, a late night brainstorm turned into a two day building sprint to create an initial prototype. Through a Chengdu friend, I built a real estate site in Chinese for selling houses in Spain. One of my older brothers pushed me to take over two of my father's sites and convert them to Drupal. I also ended up building a boutique-type ecommerce site for another friend who was attempting to sell her handmade jewelry online. None of these projects made me a ton of a money but they helped build up my confidence and understanding of how to effectively use Drupal.

## Turning Free Code and a Drupal Blog into a Full-Time Business

My DIY-Abroad.com project may have failed, but during the delays, I was lucky enough to try enough technologies and finally find Drupal during such an early stage of my learning journey. I continued to learn more Drupal as I took on new challenges and built more complicated projects.

Drupal is a different kind of open source tehcnology. While it's used by big sites like Whitehouse.gov and big companies, Drupal in my opinion still aims to be a site builder's CMS. What I mean is that it is flexible about how we add data (everything is fieldable!) and relatively friendly in how we can pull the data out and display it (Views module empowering us to create dynamic SQL queries!).

Since Drupal is open source, I was able to "look under the hood" at the code and learn how things worked. I was able to take existing modules, then clone and adapt them to my needs. Moreover, Drupal's hook system presents a way for me to write code that augments how Drupal works without hacking the underlying system.

Also since Drupal uses some of the most common web components (mySQL, php and a web server), I was able to start hosting these sites on very cheap, shared hosting plans. In turn, I was able to build my own server via Linode and learn about Linux server management. Finally when self-hosting turned into a time suck and as my projects matured to need more stability, I was able to transition towards Drupal-dedicated hosting via the lovely folks at [Omega8.cc](http://omega8.cc).

In spite of its commercial failure, Language Corner was how I "cut my teeth" on Drupal development. I struggled through problems, bugs and new features. I learned and grew. It was a complicated project with a ton of a moving parts and yet the power of the underlying modules made it extremely stable (it still works today!).

Like pretty much every developer in Drupal, I ended up building my first real module to scratch my own itch and figured I'd share it back to see if it would help others. Even though those first modules I built were pretty rough, they got better and people use them on their own sites for free. I eventually built better and more significant modules. I also blogged about what I learned and created case studies. More suprisingly people eventually contacted me about these modules I had built requesting my expert help.

As my Language Corner came to a halt, I transitioned from building for that site to getting paid to build for others. [I still do](http://int3c.com/contact). I originally planned it as a break, but it slowly turned into a large part of my professional life.

Through each new project, I learn more and my skills improve. Importantly I continue learning and trying new technologies and Drupal modules. I still do my best to give back as much code as I have time for via [drupal.org](http://drupal.org/user/1094790/) and [github](github.com/markwk).

Ironically, while I couldn't have predicted it a few years ago, I have gone from a simple user of Drupal (a site builder!) to a Drupal developer. I still don't consider myself a true expert but I can now custom code Drupal modules and debug other people's code. Even today though, most of my work is still the same as my early work with Language Corner: adapting existing Drupal modules and tweaking them to my specific use case.

_So, don't be afraid, jump in and try Drupal. It's free, the people are nice, and you may just manage to build what you thought you need to pay a huge team to build for you._

Drupal and the Drupal community, I love you. **Thanks so much for empowering me.**

<script async class="speakerdeck-embed" data-id="66892be09f280130a1272e07bed0c63d" data-ratio="1.33333333333333" src="//speakerdeck.com/assets/embed.js"></script>
