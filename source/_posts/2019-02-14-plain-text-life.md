---
title: "The Plain Text Life: Note Taking, Writing and Life Organization Using Plain Text Files"
layout: post
categories:
  - Writing
  - Writing Tools
  - Productivity
  - Knowledge Management
  - Networks
  - Plain Text
  - Markdown
  - Organization
  - Typora
  - The Archive
comments: true
published: true
date:   2019-02-14
permalink: /plain-text-life.html
---



{% img center /images/2019-resources/plain-text-life-cover.png %}

> "The power of the unaided mind is highly overrated. Without external aids, deep, sustained reasoning is difficult."
>
> Don Norman, professor and author of *The Design of Everyday Things*

External aids, especially writing, are the key to sustained learning and a creative life. The goal of your productivity, writing or note-taking systems should be to enable you to think clearly, stay organized, learn, and create. They should augment your ability to reason, to develop connections across knowledge, and produce a targeted output. 

There are a lot of tools that can help you in this pursuit. We live in a world of nearly endless options for productivity and writing software. Personally, I've tried many. But sometimes the best solution is one of the simplest and oldest.  For me, that solution was "downgrading" to plain text files as my primary means for note-taking, writing, knowledge management and life organization. 

Rather than a fully featured notes or writing tool, I now have a bunch of plain text files and a lot of them. The files themselves are simple, can be edited on any system, and are future-proof. I write in [markdown](http://daringfireball.net/projects/markdown/).  I use plain text files not only for my writings, study notes and note-taking but also for my goals, organizational, project notes. 

I call this method and approach a **plain text life**, by which I mean **a note-taking, organizational, and writing system based on plain text files**. 

The files and notes themselves have been intentionally designed to be "organized" as network of information. Practically-speaking this translates into notes stored in a few directories, tagged, and connected together using a links. The end result is a loosely-coupled web of notes. It's evolving, has emergent properties and is trackable too.  

**This setup helps me focus on what matters: writing and keeping my projects, ideas and thinking organized and interconnected.** 

In this post, I want to share my take on the "plain text life" and how using plain text files and combination of tools, best practices, and organizational principles can unlock a powerful and efficient framework for writing, thinking, note-taking, project management, goal tracking, or whatever you are working on. 

This post is divided into four sections with four questions:

- Why plain text files and what are the current limitations? 
- What tools can I use for writing and managing plain text files?
- How to stay organized? 
- What are my notes for and how to organize towards my creative, learning or organizational goals?  

At its core the plain text life is just a just a bunch of text files, but hopefully you too can assemble a powerful framework for staying organized, writing, learning and creating. 

Let's get started exploring a plain text life! 

<br />

**NOTE**: For a how-to post on migrating off of Evernote, check out [Post-Evernote: How to Migrate Your Notes, Images and Tag into Plain Text Markdown](http://www.markwk.com/migrate-evernote-plaintext.html).

<!--more-->

### The Why: Advantages and Disadvantages of Plaintext Files

> “Writing is thinking. To write well is to think clearly. That's why it's so hard."
>
> David McCullough 

Writing is arguably *the* critical ingredient to how we think and learn. If you can't write about something coherently and intelligibly, then your thinking on that topic or subject is vague and incomplete. 

Similarly, I'd argue writing is a key aspect to personal and professional organization too. Often through lists, note-taking, project management tools, or a process journal, we write out our plans, goals, intentions and other aspects that clarify what we want to accomplish. Writing allows us to express vague feelings and turn them into intentions and goals. 

Writing is also a way to keep track of things. It is argued that written language evolved largely as a mean to help us keep track of early business transactions. Writing is central factor in externalizing our memory. It also provides how we pass knowledge from generation to generation. 

Over the years, I've used a number of tools to help me write, learn, and stay organized. I recently [migrated off of Evernote](http://www.markwk.com/migrate-evernote-plaintext.html). I elected not to switch to another note-taking app and instead started using just plain text files. 

##### Key Advantages of Plain Text Files: 

Plain text will never require a subscription, lock away features, or go out of business. It's free and here forever. 

- **Flexibility: Open Them Anywhere**: Plain text files are the most flexible file format we have. They can be opened by hundreds, if not thousands, of applications. Since they are a basic component of computers, you can even open them on the computer command line.  
- **No New Tools**: We all get excited by new stuff, and for productivity junkies, we perk up with excitement to try out a new piece of software. Unfortunately tools come and go, and switching system can be wasteful and counterproductive. Switching to plain text means you never need to migrate to a new tool.
- **Portability**: By portability I mean that your files can be moved to and from different operating systems, platforms and devices and you can still open them. Whether you are on a Mac, Linux, Windows or some future tool, you'll be able to open and edit your plain text files there. 
- **Future-Proof**: A while back I discovered several writings I did in high school using Windows 95 and a version of Microsoft Word. While I was able to eventually open the files, the formatting had been lost. This revealed a potential danger in locking your words into a format that may not be around forever. Fortunately, while other file formats may come and go, plain text files will remain.
- **Trackable**: While self-tracking may not be a priority for everyone, if you are someone like me who [likes to track](http://www.markwk.com/category/track-everything/), plain text files provide the most trackable file format. As I'll share in detail in a separate post, plain text files allows you to leverage Git, a common code management system, to track your notes and writings. This lets you see your daily changes in topics and word counts as well as the evolution of your notes, projects and manuscripts. You can see a [git-based notes tracking script example](https://gist.github.com/markwk/c85a8a72bc8c03d0f510262bb5219a34) here. 

##### Notable Disadvantages of Plain Text Files: 

There are also notable concerns with using plain text files. Chief among them is the requirement for more personal discipline and personal organization. By not using someone else's designed setup, you have to make your own choices on how to stay organized. 

- **Less Unified, Weaker User Experience:** Unlike a complete note-taking or writing tool like Evernote, Ulysses, or Simple Note, editing and managing plain text files can feel more fragmented. Instead of a single app, you just have a bunch of files. This can make it feel less unified and provide a weaker user experience. Several tools, like The Archive and nvALT, provide organizational solutions on-top of plain text files. These include file and tag search. This brings much of the same feel and user experience as a complete note-taking tool, while keeping all of your files in plain text. 
- **Poorly Designed Tools for Writers and Note-Takers**: Historically plain text editors were developed for software engineers and coders. Most are (or were) free or open source. This focus on writing code and being open source has resulted in many plain text editors that are not very attractive or well-designed for writers. They can be a bit intimidating to use too. Fortunately, with the rise of markdown many new and beautiful editors have appeared. 
- **Search and Discoverability Challenges:** For me the key disadvantage since switching to plain text files has been search and discoverability. Since its indexing and search functionality was so strong, Evernote Search allowed you to get away with loose or poor note organization. You didn't need to be that organized since search could still find what you were looking for. Plain text files can also be searched but the results are not as strong as other tools. Personally, I've realized that search may not be the best solution for dealing with a complex and growing network of notes and writings. As such search is not as important for me. 
- **Requires More Personal Discipline and Organizational Habits**: Like a junk drawer or an unsorted inbox, things can get get pretty disorganized using plain text files. By default plain text files setup does force any kind of structure. You'll need to develop and follow your own process. 

While it might seem like there are a lot of disadvantages or at least challenges to a plain text file-based setup, they might all be boiled down a singular question: *How to stay organized with plain text files?* 

Let's at check out a few plain text file tools first before returning to this question. 

<br />

### The How: Great Tools for Editing and Managing Plain Text Files

The great thing about working with plain text files is you can open them up on almost any tool. This makes it quick and easy to edit a document in the command line, on your phone or on any number of text or code editors. 

While I listed "poorly designed" and "weak user experience" as one of the disadvantages to using plain text files and existing editors, this issue has started to change. In fact, due to the increased popularity of simple writing tool, there are a number of great plain text editors out there.

Here several I like: 

##### Typora: one of the best looking and best user experiences for markdown writing 

Along with The Archive, Typora is my primary plain text editor. 

![](http://www.markwk.com/images/2018-resources/evernote-to-plaintext-exported-files-example.jpg)

Typora provides both a great looking interface and smooth user experience. The layout and typography makes for a pleasurable appearance. Unlike most other editors, Typora hides the actual markdown as you write and shows you the preview of what you'll see in the output. It's much like a WYSIWYG ("What You See Is What You Get") editor. You'll need to get used to a few shortcuts to make the experience smooth, but once you get the hang of it, it really is a great way to write and edit plain text documents. 

One of my favorite features with Typora is its ability to embed images. This allows me to include local and external images that are displayed seamlessly, much like other full-featured note-taking tools. 

Typora is available for Mac, Windows and Linux and is under active development. 

##### The Archive: Connected, Plain Text Files Organizer and Management Tool

Keeping your notes organized and connected is one of the principal challenges to using plain text files. The Archive provides one of the best solutions so far. 

Basically, after opening a directory of files, The Archive feels much like a normal note-taking app but uses any directory of files. You can search and open notes by file name or find related notes by a tag. You can add sidebar shortcuts to tags or specific searches, much like you would in a tool like Evernote. It also provides a simple and clean interface for editing plain text files or option to open an external editor. 

{% img center /images/2019-resources/the-archive-writing-tool.jpg %}

The Archive is attempting to solve the problem of connecting together notes into a robust knowledge base using wiki-style links and tagging. So, if you've migrated your notes from a system with existing tags, then it should provide much of the same functionality you had before. 

Embracing the philosophy of plain text files and tool independence, The Archive's explicit focus is helping you build a [Zettelkasten or Connected Knowledge System](http://www.markwk.com/smart-notes.html) on top of your existing plain text files. We will explore several of these organizational aspects around plain text files below. 

The creators of The Archive also provide a good intro to [what is a Zettelkasten]( https://zettelkasten.de/posts/overview/) and a list of other [compatible tools for a connected notes system using plain text files](https://zettelkasten.de/tools/). Most notable are nvAlt and DevonThing. 

The Archive is currently only available on Mac and is under active development. 

##### 1Writer: My Preferred Plain Text Editor and Search for iOS

There are a lot of markdown editors for iOS. You can view [feature-by-feature breakdown of markdown apps here](http://brettterpstra.com/ios-text-editors/). I've tried several and found 1Writer to be the most complete solution. The editor itself is solid, and the preview option is great. But the real distinguishing feature is file search and tagging. 1Writer makes it easy to find files with a certain tag, view recently changed files or search. At present, I find the search function superior and faster on iOS to The Archive on Mac. 

##### Monospace: Solid Plain Text Editor for Android

I don't do much writing or permanent note-taking on Android. I mostly just jot notes into a standard note-taking app that I sync and process on the computer. That said, my preferred editor for Android right now is Monospace. It looks great and performs well. I also find Writer Plus to be another solid option. 

##### Plain Text Editors Abound

Considering how active the space around plain text and markdown editors is, I highly recommend you do your own research and testing on the best markdown and plain text editor for you. 

### A Few Key Practical Organizational Principles

In a previous section, we left a question on the table, *How to stay organized with plain text files?* This question might be shortened to just: *How to stay organized?*

Personally, I've invested a lot of thought, testing, and writings to personal organization, and it's been an important aspect of a productive and creative professional life. For me, the core of my productivity and note-taking systems have come from [Getting Things Done (GTD)](http://www.markwk.com/category/getting-things-done), The Organized Mind, Wikipedia and, most recently, the Zettelkasten Method, which I covered in [A Book Review of How To Take Smart Notes by Sönke Ahrens](http://www.markwk.com/smart-notes.html). 

{% img right /images/2019-resources/organizational-principles-infographic.png %}

A few practical principles have emerged:  

- **Outcome Thinking**: Think about what you want to accomplish. Every project, task or goal should clarify what you intend to accomplish.  
- **Establish Next Actions**: Figure out what is the next best action is on something and then do it. 
- **Leverage External Systems**: Our memories should not be the primary place where we store information or organize the things we need to do. Use a list, notebook, calendar or to-do list application to get stuff out of your head and into a system. In short, embrace tools that help you work best. 
- **Develop Processes**: Processes allow you to automate how you do something and remove the need to think too much. Much of what stresses us out about work are open threads and unprocessed items. We similarly struggle early on in a new job or facing a new type of task. In these situations, it's best to spend some time learning and experimenting with processes. Once you figure out processes and flows to deal with any challenge, then you start to remove the start and automate a best way of doing something. This apply to nearly everything, like inbox emails, requests, information and other stuff. Research how others are doing but be willing to use your processes too. 
- **Review and Reflect**: Taking a step back, cleaning up and reviewing are critical to a robust organizational system. For me the best single thing I do is a [Weekly Review](http://www.markwk.com/data-driven-weekly-review.html).  
- **Do the Work**: Assuming you have a system, tools and processes, then it should empower you to not be stressed out, find a zen-like state and focus on the work. 

These principles apply most directly to project and task management. The main tools I've used historically are [Evernote](http://www.markwk.com/gtd-with-evernote.html), Todoist, and a Calendar. I still use [Todoist as my GTD-inspired task manager](http://www.markwk.com/gtd-with-todoist.html) as well as a way to [track what I get done](http://www.markwk.com/task-tracking-with-todoist.html). In place of Evernote, I now use plain text files to accomplish many of the same roles, like outcome thinking, goal planning, clarifying next steps and periodic reviews. 

### The How: Best Practices for Naming, Tagging and Linking Files

**The core organizational idea behind my plain text files-based notes, organization or writing system is this: uniquely named plain text files; files connected together using manual tagging and links between files; and files grouped into a few targeted directories by either project or purpose.**  

The only requirements of my notes and writing system are: 1. notes must have a permanent and unique identifier, and 2. they must be capable of being connected to other notes. The unique id is generated by a date timestamp, which by the passage of time means it won't be repeated. Connections are provided through manual links between notes and by adding tags. 

<br />

##### File Naming Convention: Unique Creation Datetime and an optional keyword or short title

All files should have a unique file name. 

There are various opinions on how best to name your files. For our needs, setting your own title won't work, because you might change it one day. It might not be unique, especially if you occasional create similarly titled notes. 

It might not seem obvious why you want your file names to be unique. A unique identifier is responsible for keeping that note separate from other notes and allows for connections between files. With a unique and immutable identifier you can separate that piece of content from everything else and you can be sure links to it will go to the right place. 

So, the current best practice to use a unique name based on the datetime when you create that file. This results in files like 201902111136.md or 201603302120.txt. 

A program like The Archive or 1Writer can be configured such that new files default to this naming convention. Additionally, you can use a [bash script to automate creating unique plain text files](https://gist.github.com/markwk/86ad08822d7cfe47ed8533eb812a233d). 

While I recognize the need for unique filenames and believe that the file's creation datetime is the best starting point, I still find it useful to have an indicative name or keyword as well. Without a keyword in the filename, search because a challenge. 

Personally, the best file naming convention I've found includes a unique name based on the creation data with an optional keyword or short title after. This results in files that look like this: 201812182000_neurofeedback.md, 201602261908_My_Studies_Meta-Note.md, or 201901101453_model_of_habits.md. 

This ensures a unique identifier with the datetime so you can reference and link to the file elsewhere as well as making file lookups faster from memory.

##### Beyond Just Search: Creating Direct Links between Files

All notes should be linked to other pieces of information in your system. 

Search and discoverability have always seemed key features for me when looking for a note taking and knowledge setup. But I've come to realize the the ease of search has resulted in significant cognitive overload later and a somewhat muddled way of organizing things overall. 

With search we can often times can get to what we wanted, eventually. As [one of the writers on Zettelkasten notes](https://zettelkasten.de/posts/search-alone-is-not-enough/),  search is like a shotgun. Sometimes it hits but it's method is a wide blast and often times it's just getting you a broad selection you still need to process through to find something. What we want is a sniper's precision rather than a shotgun approach. Manual connections and proper tagging are the sniper and curator at its best. 

My objective is to create a latticework of notes, much like how our brains work. What I'm building is a curated network of linked information. As such, we need consciously built connections for this to work. 

There are a couple of practical ways to create connections between notes. If you are using a Zettelkasten tool like The Archive, you can use wiki-style links with double brackets. You can also use a full-qualified link to the file on your file system. Personally, I use both methods. In both cases I've literally connected pieces of information into a network that makes it easy to "dance" through referenced notes and related topics smoothly.

##### Tagging: Creating Shared, Flexible Groupings

I believe all tags must also include at least one tag. 

Tags are another form of organization. Unlike a folder or directory, tags are flat and non-hierarchical. Multiple notes will all reference a single tag. You can then do a search on a single or multiple tags to find all tagged content. Like a link, tags are a manual, curated process where you build out key connections in your network of notes. 

 Tags can be quite flexible, allowing you to build flexible groupings. Applying tags to certain notes allows you to reference a topic that may not even be mentioned in the note's text. 

While tagging can seem easy initially, as your system grows tagging can admittedly become rather huge and overwhelming, especially if you have dozens or hundreds of notes sharing the same tag. Tags remains one area where you likely should consider specialized tags based on the type of note. For example, a comprehensive summary note might be tagged #SummaryNote or a blog draft as #DraftWorking. 

<br />

### Notes for What?: How to Stay Organized with Plain Text Files

If you are a regular writer or note-taker, then it's likely you have lots and lots of files and notes. In my own case, [when I migrated off of Evernote](http://www.markwk.com/migrate-evernote-plaintext.html), I ended up with 11,278 note files. That's so many files that I couldn't even use certain basic search functions on the command line. And since I had many different types of notes from personal writings and project notes to collected articles, journal entries and random thoughts, it was not immediately obvious how to organize all of these files. 

Sure, everything was tagged, but where should everything go?  

We often conflate working on our productivity system with actually being productive and working. They are not the same thing. In fact, how you stay organized should serve the outcomes you want to achieve (and not the other way around). As such, we need to remember that **our file and notes system are for two purposes: organization and creation/learning**. 

This means we should develop and maintain a system that help us towards those two roles of planning and staying organizing and creating and learning stuff. 

### Fallacy of the Collector

One of the key things I realized early on when I switched to plain text was that a lot of my notes didn't serve either of these roles. Instead they just helped me collect stuff. 

As a self-tracker and documenting guy, I love collecting stuff and tracking different aspects of my life. For example, automation tools like IFTTT and Zapier can make it seamless for me to pull in links, articles and clippings from tools like Todoist or Instapaper. Evernote and most note-taking tools also make it a tad too easily to be used for miscellaneous collecting. Once all of my notes were into plain text, I discovered how much of it was just collected stuff. 

The key realization here is that your plain text files system should not just be another collection system. In fact, collecting and aggregating should be a minor aspect of what these systems should do. What our system should help us do is to learn, connect and create and to stay organized. 

### Note Types: Different Notes for Different Needs 

One helpful step in the direction of better organization was clarifying the type of notes I have and generate. At present I have six primary types of notes: 

1. **Impermanent, Fleeting Note**: These are the quick notes notes you capture while reading or learning.  You jot-down them in a physical notebook while reading a book or article or watching a video online. A thought may come on a walk or on a commute that I record in an audio file or my phone's notepad app. They are often just a rough concept you want to capture immediately. The intention isn't permanence since eventually you process and transfer these fleeting notes into something more permanent, like an insight note.  
2. **Permanent, Insight Note or Smart Note**: A smart note is a distilled, atomic idea you create in writing. They explain something in a concise and precise expression. You can't just copy someone else's way of putting it. You have to express in your own words and thoughts. The notes should be connected to other notes, tagged with key concepts, and include references to the related source material if possible. As I put it in [A Book Review of How To Take Smart Notes by Sönke Ahrens](http://www.markwk.com/smart-notes.html), "these permanent notes strive to be the stepping stone between our fleeting notes from what we read and our eventual creative production." These notes can be used as both a form of elaborative learning and to provide processed knowledge notes for on-going use in your thinking and creating. 
3. **Project Notes**: These are meta-level, organizational notes. They can used for both professional and personal projects, initiatives, goals, studies, etc. These notes often include lists, plans, to-do's, personal reflections, and references to follow up on. It might be a process journal for initial drafting, planning, and thinking through. They often serve as a way to reflect *about* the work. The work itself is covered in actual writings, insight notes or elsewhere. For me project notes have a list of next actions and links at the top and a journal of progress below. 
4. **Actual Writings (or Creation Notes)**: These are the actual things you create. This includes drafts, manuscripts, scripts, dialogues, published writings, or whatever you target output is. This is where you do the work. For me, these are blog drafts, chapters, and even markdown slides.
5. **Summary Notes (aka Structure Notes)**: Sometimes called Outlines, Index Files and Theme notes, these kinds of notes serve as an entry point into a specific topic or area. It might be an early draft or a way to conceptualize how different pieces of knowledge fit together. It could include a raw unsorted list of links to the various notes related to that topic or, as I prefer, a more sorted, organized format. In general, these structure notes service as a high-level organizational tool making it easy to build up knowledge over time and an intermediary step between insight notes and a manuscript or other creation. Depending on the project or topic, a summary note might also be be a nice complement a project note showing you what you have and gaps that you may want to work on. 
6. **Collection (or "Collector") Notes**: These are random assortments of links, highlights, clippings, and quotes from books, articles and online material. I find that they are best kept separate to avoid polluting these other notes with the unprocessed stuff. It is nice to have them available when you want to check a reference or find a specific quote from a book or article. Frankly, as a long-time collector of notes rather than a taker of a notes, these collected bits should not be the goal of your system. 

With these note types, I'm now better at staying organized and at using certain notes towards an intended purpose. This is better than what I previously had which was one mega note that mixed quotes, insights, reflections and collected study materials. 

For me the core distinction worth reiterating is between project notes and insight notes. Insight notes are atomic ideas distilled largely in your own words on a single topic or idea. Project notes are the meta-note about an area I'm working on. These could be goal, a field of study or some other largely unified area. 

For example, my reflection on the process for a goal or project is best separated from the work itself, like learning notes or writing on that project. This is actually how writers like John Steinbeck worked. They had the book they were writing and a separate meta or process journal as well as letters to friends describing the effort and challenges of that project. 

Similarly, it doesn't make sense to mix my actual study notes with the meta-level note on the goal-striving related to those studies. Their roles are separate so it makes sense to split up the notes. 

This realization has lead to the primary way of separating notes into directories.  

### The Where: Organizing Separate Directories and Grouping Your Files and Notes

Now that we've defined our core note types, we can then think about where those files should go and how to organize them. 

While we've set a few key requirements around filenames and organizational aspects and with tags and direct links, we haven't talked about how best to group and organize all of your notes. 

Some argue in favor of splitting notes into different projects and areas, while others believe it is best to keep everything in a single system, like a Luhmnan's Zettelkasten. In general it is best to not split your notes into too many subdirectories or sub-projects. this leads to notes getting buried and lost. 

In view of my goal of a networked system of notes, my notes work best all together, linked through flexible structures like tags and direct links. 

The one exception is your "collector notes," which I'd say are best kept entirely separate. These notes are other people's words, pollute search and distract from the importance of putting things in your own words. 

For the other notes, keep as many of the notes as you can together and use tagging as main way of staying organized. 

In terms of how many folders and directories to use, it depends on you, but I find that a balanced approach works best for me. At present, I have four folders or file directories:

- **My Archive**: This is where my writings, insight or smart notes, and summary notes go. This is where I do my work. Since writing involves using my insight notes, it makes sense to have them in a unified setup. 
- **My Project Notes**: This is where all of my notes on projects, initiatives, goals and progress logs are kept. I typically have a separate notes for each project, learning area, or goal. Inside I have a list of next actions and important links at the top, and at the bottom, I have a process journal recording my progress and reflections. 
- **The Collected Stuff Directory:** Beyond these core three, I also have a directory entitled **z_collected**. This is where clippings from articles and kindle readings go. It's also where I have stored my legacy notes, unsorted stuff, and past articles. For example, I use some python code to take Kindle clippings from each book I read and convert them into a separate note. I have another script that takes highlights from Instapaper articles I read too. These are nice things to have but best kept separate. 

Arguably I could go and either combine all of my notes into a single directory or further refine my notes into additional subdirectories. I find that the current separation works well for me. 

It separates out three key areas of my life and work. I have notes about my projects and goals, which serve meta-level organizational objectives; I have my writings and learning notes in a single knowledge and creation base, which allows for an organic and connective approach to learning and writing; and I have my coder notes to follow my technology work. Overall, this division is a good conceptual division too. It also makes it possible to track the evolution of each of these areas separately. 

There is a lot more that I could share related how I take and manage specific types of notes. For now, I'll have to leave these topics for future posts. 

My main advice here is to realize that notes and writing serve different purposes. You generally want all of your notes together and to use manual connections and flexible tagging to serve as your primarily organizational methods. When developing your own setup, define specific note types towards your creative and your organizational goals. 

### Conclusion: Building a Latticework of Notes

> My goal was not to replace Evernote but to evolve my system. My objective was to reconsider my organization, writing, and how I capture, process and use bits of information productively, creatively and meaningfully. 
>
> *[Post-Evernote: How to Migrate Your Notes, Images and Tag into Plain Text Markdown](http://www.markwk.com/migrate-evernote-plaintext.html)* 

When I migrated all of my notes off of Evernote and into plain text, I wasn't looking to repeat what I had done before: Create a convenient, grab-bag collection of notes, articles, writings and project ideas. Instead, I wanted to "evolve my system." The current working result is what I call *a plain text life*. 

At its core are simple plain text files that are future-proof and flexible. I write my files in markdown. These files can be opened up on any device and edited on any number of text editors. Currently my two favorites are Typora and The Archive. 

The real challenge has been and remains: How to stay organized? This isn't merely a question of information management and note-taking but of learning, memory and human creativity. 

So far, a few practical, organizational principles have emerged. 

First, all files need a unique name. My current preference is a combination of a unique datetime and an indicative keyword or title. This second feature enables easily file look-ups.  

Second, all files should be connected to other files through direct links as well as an evolving system of tags. While it's possible to have notes that aren't linked to others, what we are building should hint at the flaw in this. It would be like having a single neuron storing a single memory but not connected to anything else. The memory neuron would be useless since it wouldn't be connected or retrievable. It'd be a memory you could never get to. Notes should aim to be interconnected.  

Third, strive to keep all files together in as few directories as possible. This is both practical and conceptually. Practically, fewer directories forces you to develop an interconnected network, rather than sub-divided directories. Files come into contact and become more meaningful when interlinked. Conceptually, I define and divide things using a different note types and a few directories according to my primary use cases: learning/writing, organization/projects/goals and coder notes. This corresponds with how the plain text life applies to my work as such as a writer, engineer, and life-long learner. There are a lot of ways to organize information and knowledge and I encourage you to explore your own way. 

This final point leads me again to ponder the question of organization. It's a question that I suspect will continue to haunt me going forward too. To repose the question: **What is the best way to organize information, knowledge or our creative work, especially in view of our goal of creative output?**

In writing this post, I realize that at times I may have come off as a "comprehensive," "systematic" or all knowing. This was more about my trying to encompass and write about a range of topics, rather than some claim at the definitive answer. Learning and creativity are complex topics. Both are still being actively studied by researchers today and much still needs to be explored before we can claim a definitive understanding of how thinking works. 

That said, at least two key aspects from the research stand out to me when it comes to learning and creativity. Those are network and complexity. Basically our brains work through a network of connections. [As we learn](http://www.markwk.com/science-of-learning.html), we build connections between chunks of information. Complexity defines that fact that we can never reduce it to its individual aspects and instead properties and new aspects emerge from that complexity and network. In our brains, as a complex network of ideas emerge, these existing and emergent connections enable us to learn, think and create. We are the product of complex, internal neurological networks. 

In this same spirit, my notes system strives to emulate and evolve as a complex network of notes too. The organizational structure holds similar assumptions such that notes should be linked together and exist as part of a complex network of interconnections. 

This complex, connective approach to notes means we must largely move beyond any attempt at hierarchy. Notes will never fully or completely be ordered and organized. This includes knowledge and smart notes, written drafts and organizational project notes. We must accept them as a network since it's from this network where emergent, magical things happens, like thinking, learning and creativity. In our notes and writing systems, we must embrace the network and endeavor to write and create notes much like how our brains works: as a complex **latticework of connections**. 