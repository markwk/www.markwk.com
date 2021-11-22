---
title: "A Year in Writing and Creating: 2019"
layout: post
categories:
  - Writing
  - Creativity
  - Writing Tracker
  - Tracking
  - Data Visualization
  - Quantified Self
  - Personal Data Analysis
  - Track Everything
  - Year-in-Review
  - Year-in-Data
comments: true
published: true
date:   2020-02-06
permalink: /2019-year-in-writing-creating.html

---

{% img center /images/2020-resources/year-in-data-2019-writing-creating.jpg %}

This data was tracked and logged with a combination of tools (more on this below). The short of it is that *my number of creative words typed* was tracked with Wordcounter for Mac and *my project and smart notes* with my [open source, Git-based files writing tracker](http://www.markwk.com/track-writings.html). Data collection and visualization powered by [QS Ledger](https://github.com/markwk/qs_ledger). This post is part of my [*2019 Year in Data* project](http://www.markwk.com/category/year-in-data/). 

Below I'll share how I track these metrics, walkthrough areas I want to improve in the tracking, data analysis and visualization and some lessons learned. 

<!--more-->

### Challenge of Tracking Creativity

Tracking your creativity is challenging. Even just tracking your creative output in words typed, blog posts published or code commits isn't easy. 

Oftentimes we try to relegate creativity to some subset of productivity and time management. As if understanding the time we put in can tell us something about the quality of creative output that comes from it.  Admittedly organizational skills and an "organized mind" are just as important to an artist as they are to a management consultant. Steven King in his wonderful book, On Writing, talks a lot about how important it is to show and write and that there is a degree of craftsmanship to the so-called work of the muses. I agree that creativity does largely depend on the time we put into it. But besides tracking our time, can we track other aspects of our creativity?

For me, who has managed to track and visualize everything from my health, fitness and time to my reading and tasks completed, I'll admit that I have struggled to find a way to capture what I create. Creativity is hard to summarize outside of the final outcomes. 

The same chalenge hold trues for quantifying my learning and studies, As a life-long learner, my studies in a year may span history and science to technology and advanced algorithms and dozens of topics in-between. But how can we track what we learn, have learned or learning? 

In the in the last year or so, as I've documented in [The Plain Text Life](http://www.markwk.com/plain-text-life.html) and [Tracking Your Writings and Note-Taking](http://www.markwk.com/track-writings.html), I dramatically shifted how I write and create. The core creative principle stem from a book I read and reviewed called [How To Take Smart Notes by Sönke Ahrens](http://www.markwk.com/smart-notes.html). The key steps are: 

1. as I read books, articles and academic papers I take rough notes, 
2. I then write out these notes in my own words into "smart notes" which include
3. references to the source of that idea and quotes.
4. Finally when it's time to create something, I gather those smart notes and then transform into the final work, which in my case is a piece of writing, a presentation or a software product. 

This note-taking system has changed how I work and aided me in tackling more complicated topics. I no longer start with some outline that I expect to bend to my will. Instead, I read things that interest me, I collect passages and quotes, and I create smart notes. 

This system gives me something quantifiable to my learning and creating: my smart notes. This is one number I'm following. Similarly I create clusters of ideas with tags and summary notes. In these clusters of smart notes and interconnections between notes, I believe kernals of creativity lie. 

It's stil too early to say if and how this system will work for me. But I can say that I'm now able to engage on "heady" topics I'll study over the years ahead and I've noticed how my mind can emerge with new insights and ideas worth talking and writing about from the intersection of ideas and my notes. 

### How I Track My Creativity, Creative Output and Studies

The short of my writing and learning tracking is that I have plain text files where all of my knowledge notes, project notes and drafts are stored. This system of taking notes and writing enables me to now track most of my creative output too. I have a record of the first notes I take on a topic to the final product I produce, like an article, presentation or blog post. This setup also let's me track much of creative process too! 

Here are the tools I use to track my creative output and studies:

- **Wordcounter for Mac**: This method lets me track how many my words I type. Built by the same team behind The Archive, one of my favorite [note taking apps](http://www.markwk.com/writing-tools-2.html), [Word Counter for Mac](https://wordcounterapp.com/) is a configurable tool that keeps a record of how many words I type in each program per hour. To augment this tool, I created an [Alfred Workflow integration](https://www.packal.org/workflow/word-counter-app) to make it easier to see your stats as well as wrote [data analysis code in QS Ledger](https://github.com/markwk/qs_ledger/tree/master/wordcounter) for collecting and visualizing your stats over time. While my creative typing statistics doesn't tell me anything about what I'm writing, it does like my time tracking reveal patterns of my creative routines.  
- **IFTTT Recipe for Blog Posts Published**: I use a spreadsheet to track my blog publications. This is a bit of a hack using the automation tool IFTTT's RSS feature. I created a simple [IFTTT](https://ifttt.com/feed) recipe that detects new blog posts from my RSS feed and then adds a record into a Google Spreadsheet. After coping over legacy content, I have a dynamic way to see my publications over time. 
- **Git-based Writings Files Tracker**: When I [migrated off of Evernote](http://www.markwk.com/migrate-evernote-plaintext.html), one of my favorite productivity tools, and onto a [plaintext file-based note-taking system](http://www.markwk.com/migrate-evernote-plaintext.html), one of the motivations was the potential to track my notes in more detail. The fruit of this labor is Writings Tracker, which I wrote about [here](http://www.markwk.com/track-writings.html) and whose code is at [github.com/markwk/writing-tracker](https://github.com/markwk/writing-tracker). The script runs daily and looks at a directory of files to see if and what changed. The changes (like files modified and number of words added) get calculated and stored into a CSV, and a complete record of what changed is version controlled into a Git repo. This provides a complete record of any and all changes I made as well as summary statistics. I was only able to use the summary statistics in this current data analysis. 
- **What I Studied**:  While not high tech nor automated, in my monthly logging I keep a list of what I studied. 
- **How Many Smart Notes**: I also write down monthly how many smart notes I took. 

While far from perfect, I believe I have established a good starting point for tracking my creative output (both in terms of my study notes and my blog posts and presentations). What I'm tracking, especially the git repo of notes, is in need of more data analysis work to glean more. 

For example, I'd love to get a word cloud on my most used words or most written on topics. It would be fascinating to see which words, tags or topics appear throughout the year and clustered during certain time periods. Unfortunately I didn't have time to do that type of analysis yet, but hopefully next year! 

### Creative Output Highlights: 

I'm fortunate to lead a creative life. As a public speaker, [writer](http://www.markwk.com/), and [product creator and developer](http://int3c.com/), my work can be divided into presentations, articles published and products built (or at least worked on). 

Here are some highlights from my creative output in 2019:   

##### Presentations

- **How to Be Creative: An Ideation and Innovation Workshop for Companies, Startups and Communities**: I had the good fortune of sharing my thoughts on what is creativity, especially from the perspective of brain sciences, as well as doing a day-long hands-on workshop for finding and generating new ideas and then refining and strategizing them into products and solutions. 
- **[Self Across Time: On Time Series Data Analysis](https://markwk.github.io/ts4health/slides/slides.html)**: How does our health change over time? Can we account for it? Using Python's Data Science and Machine Learning tools, I explored how we can apply techniques traditionally used in financial models to looking at health data, like our steps, sleep and heart rate. This topic was one of the hardest technical areas I worked through last year, and, while the results were somewhat unspectatular (due to lack of temporal patterns in my data set), I now have code snippets to apply this in future health data analysis. I'm especially excited to use it in my continous blood glucose study. Thanks to Pycon Malaysia for being a wonderful host! 
- [**A Year in Data: Self-Tracking and Personal Data Analysis with Python**](https://rawgit.com/markwk/python4selftrackers/master/year-in-data-with-python/slides.html#/title-slide): "I’ve used self-tracking and personal data analysis to change my life. And I believe technology and personal data can help others." Building on previous presentations at various meetups and Pycons, I shortened and focused this talk as an intro to the [quantified self and self tracking](http://www.markwk.com/quantified-self-mind-map.html), [Python code for personal data analysis](https://github.com/markwk/qs_ledger) and actionable steps to using tracking for changing your life. In short, this is my dive into the how to lead a data-driven life and how to use tracking tech and Python to do it!

##### Blogs Published

I wrote [18 posts](http://www.markwk.com/) last year, and it's hard to pick my favorites. But a few stand out in my mind: 

- [The Plain Text Life: Note Taking, Writing and Life Organization Using Plain Text Files](http://www.markwk.com/plain-text-life.html): My magnum opus for how to track notes. 
- [Can Meditation Improve Your Attention? Self-Experiment into Mindfulness and Cognitive Testing](http://www.markwk.com/meditation-effect-on-cognition-experiment.html): I tested and tracked the effect of meditation on various psychological, cognitive tests of attention and reaction time. 
- [Quantified Self and Self-Tracking Mind Map: Conceptualizing Tracking and Other Data-Driven Tech](http://www.markwk.com/quantified-self-mind-map.html): Conceptual map of all of the tracking tech out there. 
- [Scoring Your Weekly Goals](http://www.markwk.com/goal-scoreing.html): Simple productivity "hack" to showcase weekly objectives and track if I acheive them. 
- [Instapaper: Empowering How I Read Articles with Highlights and Tracking](http://www.markwk.com/article-tracking-with-instapaper.html): This post is for anyone who reads a lot of online articles but wants to keep better track of what you read. 
- [No YouTube: 30-Day Challenge](http://www.markwk.com/youtube-30-day-challenge.html): YouTube is my biggest entertainment time suck on my phone and tablet. Here's my attempt at giving it up. 
- [Data-Driven Health Trackers: An Actionable List](http://www.markwk.com/health-trackers.html): A breakdown of technologies and techniques for tracking various dimensions of our health. A follow-up to [Are you tracking a health indicator or healthy habit?](http://www.markwk.com/tracking-health-or-habits.html)
- [What am I meditating for? In Pursuit of A Definition of Meditation](http://www.markwk.com/what-is-meditation.html): For such a popular behavior, we seem to struggle at how to define it historically and scientifically. One academic paper in particular helped me find a way to define this ancient yet modern practice.

- [Paper to Paperless: A Guide to Digitalizing Your Journals with a Scanner App](http://www.markwk.com/digitalize-paper-journals.html): I have a lot of analog notebooks. My attempt to bring paper journals into a digital notes system.  
- [Gordon Bell and The Epic Quest to Digitalize Everything](http://www.markwk.com/most-digitalized-life-ever.html): So you want to track everything? Here's an early innovator, err guinea pig, in pursuit of tracking a life down to the last pixel. 
- [Science of Goals: Goals as a Multi-Stage Pursuit](http://www.markwk.com/multistage-goal-pursuits.html): Another dive into the science of goals, specifically from the perspective of action stages. 
- [Goal Tracker for AirTable: A Flexible Tool for Goal Pursuit Tracking and Management](http://www.markwk.com/goal-tracking-with-airtable.html): My write-up on building a goal setting and tracker with AirTable. 
- [Tracking Your Writings and Note-Taking](http://www.markwk.com/track-writings.html): Here's one way to track all of your notes and writings using Git! 

##### Products, Coding and Things I Built (or Updated)

Besides several client projects where I built apps and websites, I worked on a number of my own [products](http://www.markwk.com/products/), including: 

**[DataDrivenYou.com (Web)](http://www.datadrivenyou.com)**: Data-Driven You is the new web portal I built for content and community around self-tracking and data-driven goals. I'm working on a new podcast video series, a directory of tracking tech, and an online course. I'm also hoping to finally build a data dashboard tool for self-tracking and understanding if and how life changes affect us. Basically a data portal for running your own n=1 experiments!  

[**Awesome Biomarkers (Database) + Biomarker Tracker (Google Sheets**)](https://github.com/markwk/awesome-biomarkers): Two years ago I created and open sourced a list of blood biomarkers (See: [What is a biomarker?](http://www.markwk.com/what-are-biomarkers.html)). While I still want to pursue building a [biomarker tracker app](http://www.biomarkertracker.com/), last year I used my open source biomarker list to create a way to track your biomakers with a Google Sheet. As a biohacker and health tracker, this tool makes it easy to track health metrics over time and clearly highlight at-risk areas.    

**[QS Ledger (Open Source, Python)](https://github.com/markwk/qs_ledger)**: This is an open source project for aggregating various self-tracking data and visualizing it. Since starting and coding most of the heavy lifting two year ago, this last year I added a few more data sources and made it more automated using commandline shortcuts.  

[**AttentiveAI App**](https://github.com/markwk/attn-tracker): At AT&T 5G Hackathon in LA, our team built an AI-enabled attention tracking app in React Native. The app detects faces and provides an attentive score. I created a custom model to detect and count hand raising using IBM Watson's backend. Our original intention was to empower teachers with technology to understand and better management classroom behavior. The code is open source and we walked away with the prize for best usage of IBM Watson. 

[**Manifest - an Adaptive Journaling App**](http://manifestjournaling.com/) - This is my latest venture focused on extracting meaningful data and insights from journaling. Using natural language processing, we enable journals to record with their voice or text and then present them with a sentiment analysis and additional feedback. The original version called [Mindset Journaling](https://github.com/markwk/mindset_journaling_app) was created in one weekend by me at hackathon with AI LA and Cedar-Sinai Accelerator. Following customer interviews and market research, we are currently developing our first version and expect to launch in early 2020! 

### What I Learned from the Data: 

{% img center /images/2020-resources/writing-tools-tracking-numbers.png %}

By far my favorite two writing apps on Mac are Typora and The Archive. As I share in [How I Write: My Favorite Tools and Apps for Writing](http://www.markwk.com/writing-tools-2.html), both are markdown writing tools. This chart (along with the others) show a marked spike in writing in summer and decrease into the fall and winter. 

Unlike 2018 when I published 25 posts, I only published 18 blog posts in www.markwk.com in 2019. This was below my intended goal. 

Looking at my writings data, two things stand out:

- **More Creative Typed Words**: My total typed creative word count was 491,927 in 2019 compared to 650,939. In short, I typed more creative words in 2019 than 2018! 
- **Less "Writing" Project Time**: According to my [time tracking](http://www.markwk.com/2019-year-in-time.html), I logged 70 hours less time writing in 2019 (300.3 hours) compared to 2018 (370.9 hours). Compared to the previous year's totals, this adds up to less than an hour a day.  

If I was looking for one reason why I published less in 2019 (besides the major life change in Q4!), one culprit would be that I spent less time writing! 

As I explain more below, this is likely do to the higher amount of time I spent on going deep and researching certain topics I have yet to write or publish on. For example, I did a month of studies on Tea, Qingchengshan and Daoism, but I haven't published anything on the topic. Similarly I only did a presentation on the topic of creativity but didn't publish a blog post on the topic yet. 

Unfortunately my current tracking doesn't tell me the length of blog posts compared year to year, so I can't be sure if I actually published significantly less words or not. 

Looking at my smart notes count, which is how I quantify how I learn inside my study method, we see another sign behind why my creative output dropped somewhat in 2019. Along with less blog posts I was taking less smart notes too. For me this decrease in digital note-taking is the strongest indicator for why my writings output dropped too. Basically, if I want to have complete ideas to publish on, I need to have already written and created good smart notes to start from, since most of the time writing is about transformation (rather than ex-nihilio inspirational moment). 

### What I Learned This Year: 

As part of my [monthly reviews](http://www.markwk.com/data-driven-weekly-review.html) and a general log I keep on what I'm learning, I record the topics I study each month. This isn't a very sophisticated form of tracking (at least compared to some of the data here or in my [year in reading](http://www.markwk.com/2019-year-in-reading.html)), but it does give me a month-by-month breakdown of what I learned in the past year:

- January: Book: War on Art, Habits, Marine Biology (esp Cephalopods), Flow
- February: Javascript, Flow, Tea, Self-Tracking, Qingchengshan
- March: Goals: Model of Action Phases, Implementation Intentions, Daoism, China History, Qingchengshan, Quantified Self Background, Feminism
- April: Feminism, Masculinity, COURSE: Flask API, Economics
- May: Economics, New Orleans History, Alexander Hamilton  
- June: Bitcoin, Jet Lag, Brain and Neurology Studies (ex. Nootropics, Cognitive Testing, Modafinil, L-Theanine)
- July: Health Studies, Brain and Neurology Studies (inc. Neurotransmitters and Cognitive Testing), Data Science Studies (Data Viz, Time Data Visualization, Crossover and N=1 Experimental Design, Statistics), Health Numbers, Experience Sampling, Creativity
- August: Health Studies, Time Series Data Visualization and Analysis, GRE Studies (especially Math Review), Experience Sampling, Time Series Modeling
- September: Skin Fluorescence, GraphQL, Behavioral Economics
- October: Classroom Management, Attention Tracking, React Native, Information Economics (Information Assymetry and Signalling), Product Management, Caffeine, Mental Health (like Flourishing and Positive Psychology) 
- November: GRE Studies (especially Math Review), React Native, Positive Psychology and Flourishing
- December: Javascript, React.js and Gatsby, UX Strategy, Phenomenology via World Beyond Your Head, AWS Amplify for Mobile Backends, Natural Language Processing

### Looking Ahead: 

My two writing goals in 2019 were 1.) to write longer, well-researched articles and 2.) to publish 24 blog posts. 

I definitely completed several long and deeply researched articles this year, like [What is Meditation?](http://www.markwk.com/what-is-meditation.html), [Goals as a Multi-Stage Pursuit](http://www.markwk.com/multistage-goal-pursuits.html) and [Gordon Bell, the Most Digitalized Life Ever]( http://www.markwk.com/most-digitalized-life-ever.html). I also created a few posts that required a good deal of data analysis (like [Does Meditation Affect My Cognition?](http://www.markwk.com/meditation-effect-on-cognition-experiment.html)), coding (like [Writings Tracker](http://www.markwk.com/track-writings.html)) or other product work (like [Goal Tracker for AirTable](http://www.markwk.com/goal-tracking-with-airtable.html). 

Like my current [series on a year in data](http://www.markwk.com/category/year-in-data/), I find these types of long, deep dives richly rewardly and fulfilling. But the effort is not insignificant. Unlike some past posts that merely introduced how to track something, I'm increasingly interested in the science behind whatever we are trying to quantify as well as what we can learn from these numbers. Combining the science of behavior with technologies that help us track and modify it is central to much of my product and social work today. 

While on the surface these two writing goals seem complementary, I now realize that these goals (write longer vs. publish a certain quantify) are somewhat discordant or in conflict. It's hard to research and write in depth and still expect to have the same numerical output. Push come to shove, I'm glad I went with depth over some arbitrary number. 

That said, the numbers don't lie. I didn't spend as much time on my writing as I did in 2018. I'd like to get this writing time number closer to where I was, meaning about 1 or 2 hours a day dedicated to writing. Similarly, while I had a great start and solid summer creating "smart notes," this lagged later in the year. I still [read a ton](http://www.markwk.com/2019-year-in-reading.html) but I need to get back in the habit of processing what I read into notes on key takeways and insights. 

Overall, I'm super excited about the year ahead. I have a solid list of things I want to write, create and learning. Now that I'm in the US more long-term, I'm especially keen to present more and focus more on creativing data-driven, tracking tools in line with my big vision. Additionally, I can't wait to see what I can glean from a deep data dive into tracking my creative output more too! 

<br />

[Check out other posts, data visualizations and infographics from my year in data!](http://www.markwk.com/category/year-in-data/)