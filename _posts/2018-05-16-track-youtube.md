---
title: "How to Track Your YouTube Watching (And Understand It)"
layout: post
categories:
  - Tracking
  - Track Everything
  - YouTube
  - Online Video Consumption
  - Media Tracking
  - Quantified Self
  - Self-Tracking
  - Python
date: 2018-05-16
comments: true
published: true
permalink: /youtube-tracking.html
---

{% picture center /images/2018-resources/how-to-track-youtube-watching-cover.png %}

**How much time do you think you spend watching online videos like Youtube each day?**

Be honest and take a guess.

While you probably have a pretty good sense of the type of content you are watching on YouTube, do you know how much time you spend watching?

You are likely underestimating the amount of time you spend watching online videos. According various studies, the average adult watches videos and TV for an hour longer than they estimate.

**In short, we think we watch less TV and online videos than we actually do.**

Personally, there have been nights where I’ll guiltily realize at 2am or later that I’ve just spent several hours streaming dozens of entertaining videos but wish I hadn’t. I’ll tell myself again and again “just one more video” as the dawn nears. I have oscillating feelings about YouTube, since it's a free medium to watch amazing content, entertainment and educational.

If you have ever wondered what and how many videos you are watching online, you are in luck because you can transform Google's YouTube Watch History into tracking statistics that tell you what you are watching and how much. Unlike other forms of tracking, it doesn't require you to set anything up to access this tracking data.

The reality is that people spend a lot more time on YouTube: about an hour or more per day, according to Google. In comparison to my own tracking data, which I’ll go into detail on how you can get these stats too, I have watched well over 45 days worth of videos on YouTube in my life, and in the past two months, I’ve spent over a day and half each month watching YouTube videos or about 73 minutes per day.

While a lot of blogs and people online talk about protecting your privacy and about deleting your history on this or that service, I highly encourage you to **collect your data before you delete it**. Google and YouTube data is particularly interesting, since it can tell you a lot about your online behavior. You can see trends in what you watched during different times of your life. Collecting your Youtube watch history is also a great way to save as well as [extend and augment your digital memory](http://www.markwk.com/2016/11/tracking-article-reading.html).

Our relation with technologies like smartphones, social media, apps, etc. is not always as simple as accept or reject. Instead, there can be a nuanced understanding and a conscious engagement. **By tracking and analyzing our usage of certain technologies, we can better understand our engagement and make conscious choices about how and how much we we want use a technology like YouTube.**

In this post, I want to share some ways to track and quantify your Youtube watching as well as a few steps you can try change and improve your Youtube usage. We will look at four different techniques for tracking your Youtube video watching. The first way is provided by YouTube app and requires zero setup, but it does require you to note your watching once a week. The next two ways are quite simple and require minimal setup but provide only a limited view of your Youtube History. The fourth way will require some Python Code and Data Analysis in order to gain the most complete data on your Youtube History.

Hopefully this techniques can help you not only understand how much and what you watch YouTube, but change it too.

<br />

PS -- Check out my [30-day No YouTube Challenge](http://www.markwk.com/youtube-30-day-challenge.html) for what happened when a took a break from online video watching.

<!--more-->

### YouTube: Love it or Hate, But First Track It

YouTube is a double-edged sword for me: lots of a positive but equally problematic technology too. With YouTube, I can find great videos that educational and informative and improve how I think about my work, my studies and any number of topics. With Youtube, I can also end up in a dangerous time whirlpool of time-suck.

YouTube is massive, and its place in our digital lives is staggering. A total of 1 billion hours of videos are watched on YouTube each day. About a third of all internet users are on YouTube. Over 1.5 billion active users per month to be exact. On mobile, it has been reported that logged-in users are spending more than one hour per day watching videos on YouTube, and the average mobile viewing session lasts over 40 minutes.

Our digital and technological lives are complicated. There have been some recent backlashes against services like Facebook, especially around digital privacy but also addiction and the idea of “time well-spent." There is the on-going struggles and debates about digital addiction, gaming, constant email, and our "always on, always available" internet and smartphone lifestyles. Mindfulness and digital detox come from the reality that we still haven’t figured out how best to live with these technologies as a society and as individuals.

Like a lot of digital technologies today like smart phones, apps, social media, online entertainment, and communication tools, it’s not quite so simple as leaving a service or deleting an app when we have some misgivings. These tools are part of the fabric of living in a digital economy and society. We can’t really leave the entire internet, though we can better fit these technologies into the type of lives we strive to lead.

If you are anything like me, then there is a good chance you watch a few videos or more per day on Youtube, and some days a lot more. But how to quantify one's usage? How to better understand the time and information we watch on the streaming video platform? How to understand my Youtube life?

Fortunately, it’s not that hard to track and quantify your Youtube usage, and in my opinion, everyone should take the opportunity. You should look at and consider how you spend your time on sites like Youtube.

So, can we know how much and what we are watching on a service like Youtube? Yes, we can.

### How to Track Your Youtube Time with the YouTube App and a Manual Log

_Did you know there is a way to check your watch time in the YouTube app?_

The first and easiest way to get to know how much you use YouTube is by checking the mobile app on your phone. Go into your account and then go to Time Watched and viola your watch time from the last week!

{% picture right /images/2019-resources/find-youtube-watching-history-in-app.jpg %}

Unfortunately you can only view how much time from last week and it appears to only be a feature available on the mobile phone app. It doesn't appear in the iPad app, which is where I use YouTube most of the time.

Personally, while the next several methods are more robust and detailed, this method is the one I use most. During my [weekly review](http://www.markwk.com/data-driven-weekly-review.html), I use a Google Form to quickly log a few different data points from various apps, website and life. These all then get aggregated into a Google Sheet. From there it is super simple to create charts. Here is an example of my Weekly YouTube usage compared with iPad time where I almost exclusive watch YouTube videos on.

{% picture right /images/2019-resources/youtube-ipad-usage-trrends.png %}

If you are looking from some initial numbers on your YouTube time, check the app! Even better if your trying to modify your usage, keep a weekly log and see how it varies over time.

### How to Track Your Youtube "Liked Videos" with IFTTT

When it comes to tracking your Youtube watching, the easiest way to start is by logging the videos you like with IFTTT. [IFTTT (“If This, Then That”)](https://ifttt.com) is an automation service that allows you to integrate or “glue” certain services together. For example, if you post on Twitter, you can save it to a Google Sheet, or if you post a photo on Instagram, you can save it to Dropbox. IFTTT and its alternative Zapier combine dozens of services together, allowing you to create nearly recipes.

To create a recipe in IFTTT, first pick the service and event trigger (i.e. Twitter and Post a Tweet) and then the action to take (i.e. share twitter on Facebook).

For any interested in the quantified self or self-tracking, IFTTT is a great way to aggregate and store events and activities from one service like Youtube into another. For my own tracking, I use IFTTT to store into Google Sheets things like the weather multiple, the articles I read in Pocket, the [tasks I complete in Todoist](http://www.markwk.com/task-tracking-with-todoist.html), and even my running stats from Strava and Runkeeper. Additionally, I use a Google Form, a Spreadsheet and Zapier to create my own [data-driven weekly review](http://www.markwk.com/data-driven-weekly-review.html).

IFTTT provides several integrations and services with Youtube with most of them geared towards Youtube creators. For self-trackers, there is also an event you can use for liked videos. When you like a video, you can trigger any number of events. If you want to keep a log, then when you like a video, you can store it in an spreadsheet like Google Sheets or AirTable or append to a note in Evernote.

This allows you to have a clear record of videos you liked and when:

{% picture center /images/2018-resources/youtube-likes-log-spreadsheet.png %}

You can create simple pivot table and charts too:

{% picture center /images/2018-resources/youtube-likes-log-by-month.png %}

Additionally, using an integration with Telegram, I’ve also created a special chat channel where I post my liked videos too.

One of the reasons I track my life is to extend and augment my memory. With tools like Evernote and various tracking methods for my Music, Read Articles, TV Watched and Youtube history, I’m able to look up any and everything I’ve consumed since I started. I have a complete history I can access and leverage in my projects.

In an ideal world, you’d have an option in IFTTT to trigger an event when you finish watching a video in Youtube, but fortunately this “liked video” trigger provides a great initial way to keep a log of your favorite Youtube views. For many, a record of your favorite Youtube videos might just be what you need.

### Tracking Your Youtube Computer Time with RescueTime

If most of your Youtube watching is done on the computer, then a great way to track it is with RescueTime, a well-known service for computer usage tracking and time tracking. RescueTime is a favorite productivity tool among anyone interested in productivity and quantified self enthusiasts, and it is probably the easiest tool to measure your computer time.

As I write about in detail in [How much time did that take? Time Tracking Tools for Self and Freelancing](http://www.markwk.com/time-tracking-tools.html), RescueTime is an application you install in the background on your computer, which logs which applications and websites you use and for how long. There are then a number of settings you can adjust to determine if that service is productive, distracting or neutral for you as well as the category it falls into it. Setup is simple, tracking is done passively, and, in only a few days of logging, you can quickly get a portrait of your time usage. RescueTime can also be great service for continuous lifelogging too, allowing you to know where your time was spent any day in the past.

When it comes to Youtube, RescueTime can tell you how much time you spend watching Youtube Videos. It will also note the name of videos too. Here is an example day from a year ago:

{% picture center /images/2018-resources/youtube-tracking-rescuetime.png %}

Fortunately or unfortunately, I’ve nearly completely stopped watching Youtube on my computer As you can see, over the last quarters I’ve reduced how much time quite significantly:

{% picture center /images/2018-resources/youtube-watching-by-quarter-rescuetime.png %}

I’m still watching Youtube, but I’ve intentionally decided that Youtube usage should fall outside of my work day and not be done on my computer. In a quest to do more focused work, avoid distraction, and eliminate shallow work, I deem Youtube as a non-work thing. Instead Youtube is for breaks, evenings and specifically not on the computer anymore.

Before going into how to your full Youtube Watch History, let’s look at some of the ways and techniques I’ve used to modify my Youtube Watching behavior.

### My Computer YouTube Watching: Reducing, Then Eliminating

While Youtube is great in some ways (more on this later), it can be a big time suck and distraction too. One of the reasons I decided to first reduce my Youtube Time on the computer and eventually nearly eliminate it was that Youtube watching wasn’t an impactful or meaningful way to spend my work time.

Watching Youtube videos is mostly a distraction, and, although you can find some good education content, it doesn’t generally contribute to reaching my goals and getting important things done. So I decided to reduce my usage.

In order to reduce (or block) my Youtube, Facebook and general distraction time, I’ve used a number of tools and techniques. Let’s look at two options.

##### Using Browser Extensions to Reduce and Block Youtube Usage

{% picture center /images/2018-resources/youtube-blocker-chrome-extension.png %}

Since most of your computer Youtube time is likely spent via a browser, then one of the best ways to make you more conscious or change your behavior is by using one of several productivity browser extensions. These extensions for Chrome, Firefox or Safari allow you to set limits on certain sites or even block them entirely.

My two favorite are [Stay Focused](https://chrome.google.com/webstore/detail/stayfocusd/laankejkbhbdhmipfmgcngdelahlfoji?hl=en) and [Go Fucking Work](https://chrome.google.com/webstore/detail/go-fucking-work/hibmkkpfegfiinilnlabbfnjcopdiiig?hl=en). Stay Focused provides a number of settings to control which sites and your specific limits. It’s goal is more about limiting the amount. By contrast, Go Fucking Work is more about completely blocking certain sites during certain hours of the day.

Personally my experimentation in limiting my time on Youtube and Facebook started with Stay Focused, and the goal of limiting my time to under 10 minutes day. It was hard at first, and it was tempting to disable the extension or use a workaround to check these sites. But over time, my habits changed, and checking youtube or facebook completely disappeared from my mind.

I recently switched to "Go Fucking Work.” It provides many of the same features, but in view of the fact that my goal changed to completely eliminating Youtube and Facebook during certain days and hours, this service made a bit more sense.

In my experience, if you are looking to reduce or change your Youtube usage, then extensions like these are a great help.

##### How RescueTime Can Support Reducing Your YouTube Time

If you decide you want to reduce or change your Youtube watching behavior, RescueTime can also be a be a great support in making this happen. Not only does it have your time logs, but you can create goals to limit how much time you want to spend on Youtube or any other tool. For example, after setting up a goal, RescueTime will give you a notification if you reach your limit. You can even program RescueTime to schedule periods of the day for “focus time” or block these sites when you go over your target limit.

In my attempt to limit my Youtube time on the computer a year ago, I set up a Goal in RescueTime. Here is a report from my last several days:

{% picture center /images/2018-resources/youtube-usage-rescuetime-goal-tracker.png %}

While my original goal was less than 2.5 hours a week, it’s clear that my mind doesn’t even think about using Youtube on the computer anymore, and my usage is trending to less than a minute a week!

Overall, with RescueTime, I’ve been able to decrease the amount of time I spend on my computer while staying productive maintaining consistent and productive creative output. One of the ways I’ve been able to do this is by reducing and then eliminating distracting sites like Youtube, Facebook and Twitter. Additionally I’ve been trying my best to reduce administrative time like email, chat, etc. These are so-called “shallow work.” These are areas I’m still working on, but I think in general, I’ve decided that I’d rather spend time on high value, deep work like writing, coding and thinking, over shallow work or distracting sites.

While completely eliminating Youtube from your computer usage might not be appropriate for you, I highly encourage you to consider finding ways to only use it in your non-work time. This kind of habit change can lead to both a huge productivity improvement and a better mood.

Now that we’ve looked at two simple ways to track your Youtube usage and some ways I’ve used to decrease using Youtube on the computer, let’s look at how to extract and do some data analysis on your full Youtube Watching History.

### How to Track and Extract Your Entire Youtube Watching History with Python

In this section, I’d like to share how to extract and analyze your Youtube Watching History with Python. This section is a quick step-by-step guide on how to get your youtube watch history and then how to extract and export it to CSV or Excel Spreadsheet format. With this export you can start to track, keep a log, and do data analysis on your youtube watching.

Unfortunately, at the time of writing, Google does not provide any way to view your aggregate stats on what and how much time you spend watching videos on Youtube. Personally, I’d love to see inside Youtube some simple charts like you do with Audible or some podcast apps. Fortunately, Google does provide a web listing with your complete youtube history that can be scraped and parsed.

**NOTE**: This section requires some basic technical skills. You don’t need to be a Python or coding expert, but you do need to know how to edit and run Python script. In order to follow this tutorial, you’ll need Python 2 installed and working on your computer. I'm specifically on Mac OS X, but an adaptation of this should work on Windows or Linux.

#### Extract Your Youtube Watching History with Python

{% picture right /images/2018-resources/youtube-python-scraper.png %}

##### Step 1: Install Python and Check Version

For this to work, you'll need version 2.x of Python. It’s installed by default on Mac OS X.

##### Step 2: Download/Clone Code:

Download or Clone code from this Github project: https://github.com/zvodd/Youtube-Watch-History-Scraper.

##### Step 3: Install Dependencies

pip install scrapy lxml sqlalchemy

##### Step 4: Copy Your Youtube Cookie

- Install a browser extension like [EditThisCookie](http://www.editthiscookie.com/)
- Go to Youtube.com and ensure you logged in.
- Click the "editThisCookie” icon or button, then click export. The cookies are now on you clipboard.

{% picture center /images/2018-resources/cookie-copy.png %}

Alternatively, Open chrome / chromium. Make sure your logged into youtube.com. Open the inspector (F12). Open the network tab, check the "Preserve History” box. Visit https://youtube.com/feed/history. Click the request for "/feed/history" in the network tab. Copy the section "Request Headers", below the title "Request Headers"

##### Step 4: Add Cookie to Your Scraper Script

In the directory for Youtube-Watch-History-Scraper, create the file “youtube_cookies.json.” Open that file with a text editor and paste in your Youtube Cookie info. Save the file.

##### Step 5: Run Command to Scrape Your Youtube History

Now open your command line tool like Terminal or iTerm and navigate to the directory for Youtube-Watch-History-Scraper. Inside that directory run the following command:

`scrapy crawl yth_spider`

This process might take several minutes depending on the spend of your internet and how extensive your Youtube History is. Once completed you should see in your directory the follow file: youtube_history.db.

#### Optional Step: Explore Data with SQLite DB Browser

If you prefer to explore the raw SQLite Database, checkout SQLite DB Browser, a program that will allow you to open up this file and explore it that way.

#### Step 6: Convert SQLite DB to CSV

If you want to explore your Youtube History in a spreadsheet or other data analysis tool, then you should convert it to a CSV. Assuming you have the dependencies installed, the following command should work:

`sqlite3 -header -csv youtube_history.db "select * from videoshistory;" > out.csv`

The end result will be a CSV file with several columns:

- vid - raw video id and url
- author_id - channel or creator url
- title
- description
- time - length of video in seconds

#### Caveats and Improving Youtube History Scraper

Overall, this python scraper is a great way to extract your youtube history. There are a few caveats worth mentioning.

First off, this method will scrape everything in your history, including videos you just watched for a few seconds and switched to another. So, if you decide to use this method and want a more accurate record, then you’ll need to delete videos from your history that you don’t watch entirely. It’s not hard, but you need to make it a habit.

Second, the current scraper doesn’t tell you when you watched a video. This is just the nature of the data on the history page, since it doesn’t include a watch date. One adjustment I might make to the code would be to note when the scrape was done and not re-import videos after they are scrapped. This will allow you to re-run the script, to know roughly before what date the video was watched, and, in turn, to improve later data analysis.

Third, right now this is a one-off script. One obvious improvement would be to automate this script to run a few times a day. Additionally it could post the data to a CSV in Dropbox or even into a Google Sheets log.

Currently, I’m using this script to scrape my Youtube History once or twice a month. I then edit the data, import it into Google Sheets, note the scrape date and month, and do my basic time and usage analysis.

#### Initial Data Exploration of YouTube Watch History

Now that we have a full export of your youtube watch history, it should be easy to explore your watch history data in your preferred method, like Tableau, Google Sheets or your favorite spreadsheet application. A full data analysis and data visualization is outside the scope of this post, but let’s do an initial exploration with Google Sheets to see what we can learn and manage this tracking data.

As a starting point, here is an example of my cleaned up data:

{% picture center /images/2018-resources/youtube-watch-history-tracking-log.png %}

As you can see, I’ve gone ahead and converted seconds to minutes, added a column for when I scrapped the data and tagged the month watched too. In the case of videos before I started tracking, I added a generic pre-XXX date. This allows me to keep some aggregate stats going forward.

I then created a simple pivot table showing me my aggregate stats by channel:

{% picture center /images/2018-resources/youtube-tracker-top-channels.png %}

These stats aren’t entirely surprising since I watch a few videos per day about the NBA, a few Comedy videos and occassionally some news. Recently I’ve been changing my habits to subscribe and watch more educational channels like Crash Course and SciShow.

Unfortunately not all the channels have obvious names, so I’ll need to do some more work to improve either the scraper or add their names manually. Additionally I’m interested in knowing the genre of my top channels (or of the videos themselves). Broadly I want to know whether these are entertainment or educational channels. These simple changes shouldn’t be too hard to add and, much like RescueTime, it would give me a better sense of how my Youtube Watch History reflects whether my watching was more productive and educational or distraction and mindless entertainment. Furthermore, I can then see how my transition to more positive and educational content looks in terms of the tracking numbers.

By my mental estimate, I suspected that I spent under an hour per day watching Youtube. Using the month tag, I was able to determine how much time I actually spent watching Youtube over the last two months:

{% picture center /images/2018-resources/youtube-tracker-monthly-watch-statistics.png %}

The grand total: 70,079 minutes of total youtube watching. Broken down over the last two months of more accurate tracking, I watched about 37 hours or 1.5 days worth of Youtube videos per month.

To be honest, these numbers surprised me somewhat, since while I have eliminated Youtube from my computer usage, I’m still watching a bit over 1 hour per day on either my iPad or phone each of the last two months.

In comparison, I watched on average 19.28 hours per month of TV and Movies over the last three months (April 18.75 hours, March 16.6 hours, Feb 22.5). So, all combined I'm watching on average 56 hours per month on videos, TV and movies, or about an hour and 51 minutes per day.

That’s nearly 8% of my total time per day. When you look at it in aggregate, this number appears bigger than I would have guessed, but it isn’t nearly as high as the estimates for many people today. According to a [summary in New York Times of video watching on different platforms](https://www.nytimes.com/2016/07/01/business/media/nielsen-survey-media-viewing.html), the average American adult watches per day: five hours and four minutes of television and thirty-one minutes on their tablet and one hour and thirty-nine minutes on their phone consuming media.As the writer puts it, we are “wired all the time” spending 10 hours and 39 minutes per day consuming media.

So in contrast, I spend a lot less than the average American in terms of my TV and online video watching. Considering how much time I read, the positive creative work I’m doing, and my language and technical studies, I’m not that concerned about the amount of my video watching time. It’s definitely an area I could reduce, but due to the current schedule and obligations I have, it’s probably an acceptable situation. Like everyone, I need breaks and relaxation, and watching videos isn’t that bad an option. If my work situation changes or I need to remove one time element to put my time in another, then video and TV time would be high my list to change.

Personally I don’t think watching Youtube (or TV and Movies) is a bad way to spend my time, especially since it’s outside my work day and a form of relaxation. Additionally, if you tailor your Youtube subscriptions and settings, Youtube can be highly educational and informative too. Over the last couple months, I’ve transformed my Youtube watching into educational time.

Let’s conclude this post by looking at some ways I’ve been tailoring my Youtube Feed to bias towards educational content.

#### Conclusion: My YouTube Time and Training the Learning Machines

YouTube is one of the most used services on the internet. With a total of 1 billion hours of videos watched on YouTube every day and average user spending over an hour on the platform daily, it’s worth thinking about it and how you use it.

If you are anything like me, then Youtube is another digital service or technology you both love and hate. It may not lead to the negativity like Facebook, but it doesn’t come without a certain degree of what I like to call "internal technological usage conflict.” You love Youtube since it’s an endless source of entertainment and educational content. You can study and learn anything through various educational and technological channels. You hate it because it can be distracting and a time suck. It’s an addictive yet educational and empowering. It’s democratic, open, free, and essentially endless.

In this post, we looked at a few different methods to understand and track your Youtube usage. We looked at using the the basic stats we can get in the app, the automation service IFTTT to keep a record of liked videos, and at RescueTime as a way to track computer time on Youtube. There are pro's and con's to each. We then looked at some custom Python code you can use to scrape and aggregate your entire Youtube Watch History. By modifying your watching habits slightly, regularly collecting your data and some simple data cleanup, you can track and keep an accurate record of your Youtube Watching.

These techniques provide a way to help you break down how and what you use Youtube for. Like a lot of technologies today, your usage isn’t a simple binary Yes or No. Instead, you need to think about what the technology is for, should you use it and how. Email is one of the earliest online communication methods, and yet we still struggle to use it well. Similarly Youtube presents both great aspects and negatives. Tracking and collecting your Youtube usage data can make you aware of how you use it, and, in turn, it provides the chance to change or modify your behaviors.

Personally, by tracking my Youtube time, I’ve realized that I don’t want to spend my computer time on Youtube, Facebook, and a few other services. I’ve implemented blockers and habit changes that means it’s an effort to access these services. Initially my brain habitually wanted to check a video or check a status update on these sites. But over time with the help of browser extension, I’ve completely lost interest in using these services during the day and rarely use them at all in some cases.

Youtube isn’t a service I want to leave entirely. I’m not a luddite, and its usage isn’t a pure situation of acceptance or rejection. Between mindless entertainment of cat videos and gossip new and high quality educational lessons on any subject lies the endless chasm of video content. Well over 5 billion videos have been shared as of early 2017, and content creators effectively upload and share 300 hours of video content every minute. The amount of content available to you on Youtube is staggering. I want access to this content, but I’ve had to adjust my habits to use it in the right place and time; namely, outside of my work time and for relaxation and learning.

Fortunately, you can even improve and modify your Youtube Watching Life. Specifically by subscribing to certain channels and liking targeted videos, you can train Youtube's recommendation engine to orient your feeds away from some things and towards certain other content.

Youtube is a system built to give you more or less what you tell it you want. Using machine learning, Youtube learns from your subscriptions, watch history and likes to recommend what it thinks you’ll enjoy next. Using a combination of factors, it tailors the videos it recommends to the top of your feeds.

In my case, over the last several months, I’ve subscribed to more and more channels related to science, technology, history, machine learning, programming, etc.; I’ve unsubscribed to channels that don’t fit me; and slowly but purely my Youtube Feed are biased towards great educational, awe-inspiring and informative content. By tracking and getting to know your Youtube watching history and modifying your behavior, Youtube can become what you want it to be.

Good luck and happy tracking!

<br />

<br />

_NOTE: Post was updated on 8/1/19 to include additional tracking method via app._
