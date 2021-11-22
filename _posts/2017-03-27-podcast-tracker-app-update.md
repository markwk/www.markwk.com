---
title: "Building a Podcast Tracker App: Dev Update and Other Podcast Listening News"
layout: post
categories:
  - Tracking
  - Quantified Self
  - Personal Data
  - Podcast
  - Podcast Tracking
  - PodcastTracker.com
comments: true
published: true
---

{% picture center /images/2017-resources/podcast-listen-example-03.jpg %}

I love me some podcasts. And this year I’ve been getting a healthy dose of podcast listening in. According to my count, I’ve already logged 2 days, 7 hours and 55 minutes of podcast listening so far in 2017.

To track and log this, I’m currently building my own podcast listening tracker.

It’s been almost 3 months since I first shared the [first version of my podcast listening tracker](http://www.markwk.com/2017/01/my-year-in-podcast-listening.html) and what I was up to. We’ve got some new features and more users. So it’s time to share a few updates.

In this post, first, I’ll share a bit about #trypod month and a few of my favorite new podcast listening discoveries. Second, I’ll provide an update on development and progress. And, finally I wanted to share a bit more about what’s next.

<!--more-->

## #TryPod: A Few Podcast Recommendations

First off, apparently March is the month to bring more ears to podcast listening. There is even a hashtag: [#trypod](https://twitter.com/hashtag/trypod?lang=en). As usual my monkish behaviors around social media means that I’m a bit late to join the #trypod hashtag party.

At the beginning of January, I shared a recap of my podcast tracking from 2016 under the auspicious title of ["My Year in Podcast Listening: 2016”](http://www.markwk.com/2017/01/my-year-in-podcast-listening.html). To summarize my favorite and most listened to podcasts in 2016 were: Presidential, Serial, Freakonomics, Planet Money and Revisionist History.

{% picture right /images/2017-resources/top-scoring-podcast-listened-to-2017.jpg %}

I still recommend all of these for first-time listeners. Unfortunately only two out of these top five (Planet Money and Freakonomics) have new episodes in 2017. Since release an episode on all the past American Presidents, I don’t expect Presidential will be releasing anything soon. After two amazing and suspenseful seasons, we will have to wait on Serial too, though word is out that they created a new partnership series called “S-Town.”

Planet Money and Freakonomics are both amazing podcast on the broader field of economics and subfield of behavior economics. For me the7 remain my most common listens with Freakonomics Radio at 6h45m in 11 episodes and Planet Money at 5h35m in 17 episodes.

For **Freakonomics** I’d recommend you start with “How to Get More Grit in Your Life,” which is about building passion over a lifetime, or try a recent episode called “Chuck E. Cheese’s: Where a Kid Can Learn Price Theory,” which delves into data and misperception around violence and kid’s entertainment.

For **Planet Money**, two episodes I enjoyed recently were "#753: Blockchain Gang,” which described the rise and fall of a blockchain entrepreneur and "#752: Eagles vs. Chickens,” which described the economic funniness of one of America’s most iconic and protected animals.

{% picture center /images/2017-resources/podcast-listen-example-01.jpg %}

Since my other top favorites are in hiatus, this has lead me to try out a lot of new podcasts since then.

Here are several of my favorite podcast listens with my stats and a favorite pick from so far in 2017:

- **50 Things That Made the Modern Economy** (1:57, 13 episodes): Short history lessons connected to the economy.
- **The Quantified Body** (2:59, 4 episodes): Checkout "10: Doug McGuff: Time-Efficient Workouts"
- **On Being with Krista Tippett** (2:33, 3 episodes): Long form discussions on science, religion and living. Checkout recent episode: Margaret Wertheim — The Grandeur and Limits of Science
- **Note to Self** (3:07, 9 episodes): Privacy Paradox Series on tech’s obsession with following our lives for profits
- **Radiolab** (2:53, 5 episodes): High quality and thought provoking pieces on science and society. Checkout: "Bringing Gamma Back” on recent advances in curing memory loss associated aging and disease
- **Horizon Line** (2:12, 4 episodes): Episodes about great adventurers from the past and present. Start with "Ep. 1 The Arctic Balloonist"

I also got into the series "Missing Richard Simmons" (3:20, 6 episodes), which looks at the life and “disappearance” of Richard Simmons from the public sphere. It was enjoyable but ultimately a bit pitiful since my takeaway was that Richard Simmons merely wants more space rather than some macabre problem. Podcaster: get a life.

And my 2017 podcast listening total so far:

{% picture center /images/2017-resources/podcast-listen-stats-q1-2017.jpg %}

## Podcast Tracker: Development Updates (March 2017)

Let’s take a look at developments in podcast tracking tech. I still haven’t heard of any podcast listening apps that provide an export of your history or statistics, so the super short story is that I’m building one.

To summarize, in late December 2016, I decided to build a tool to track podcast listening for listeners. Few if any podcast listening apps give you any historical data on your listens or even aggregate data on your listening time. Any application I use needs to give me my usage data or at the most basic some statistics.

{% picture right /images/2017-resources/recent-podcast-listens.jpg %}

This lack of options for podcast tracking pushed me. Inspired by the likes of Last.fm (music listening tracker), Trak.TV (TV and move watching tracker) and GoodReads (book reading tracker), I built the first version on top of Drupal, a PHP framework I’m specialized in. This become my DIY Tracker for Podcast Listeners:

> Here’s version 1.0: Since podcasts are distributed via RSS feeds, I was able to pull in all of the past content from my favorite podcast channels, and once I had them in a database structure, I added a simple feature to manually log my listens. With the podcasts episodes added automatically and a simple way to log when I listened to them, I had a working version 1.0.

This basic service then allowed me to create simple reports and statistics. As a slightly obsessive podcast listener, I then become able to know a lot more about my podcast listening:

> In 2016, I consumed roughly 191 episodes from 23 different podcast channels, and in total, I listened to 4 days, 23 hours and 2 minutes of podcasts . That’s equivalent to 15 eight-hour workdays or 15 full nights of sleep. Or in most earthly terms, 1.36% of my time in 2016 (it’s a leap year!) was listening to podcasts.

Since launching the alpha version of my podcast tracker in early 2017, I’ve slowly added a some early users (if you are interested, send me an email at markwoester@gmail.com. I’d love to have you try it!). Right now the service aggregates a huge host of podcasts and episodes and allows you to manually mark what you listen to. Overall, it’s great to have some people (including myself) using such a simple initial service.

{% picture center /images/2017-resources/podcast-listening-stats-by-podcast.jpg %}

Besides listening to a few additional days worth of podcasts, in January, February and March, I spent the majority of my extra dev time on two backend features:

- 1: optimizing the podcast aggregator
- 2: scraping and adding all of the podcasts from Apple’s podcast directory.

Unfortunately one of my early realizations was that there are really a ton of podcasts out there, even more than I thought. This means a lot of syncing to check for new updates.

As such, effort was needed to create an efficient backed service to pull and aggregate new episodes from the RSS feeds. We had to tweak the code to first sync subscribed podcasts and then a periodic sync of all other podcasts in the system. This means our users get their podcasts updated first and at the same time we continue to check on the latest episodes for other odd-ball podcasts. We’ve made some good improvements here, but I suspect long-term we will need a completely new feeds backend.

I’ve come to see that Apple and iTunes remain the central hub for podcasts, though likes of Stitcher gets a lot of attention too. While Apple’s default podcast player is far from perfect, it is the defacto standard podcast listening app. If you have an iPhone, then you can listen to podcasts without downloading anything new. Similarly, its directory is also the largest for aggregating and tracking the most popular podcasts on the web. This size made it the obvious choice for finding and discovering podcast channels.

Fortunately iTunes podcast directory is structurally straightforward, and we had no issues with spiders pulling data from the site. On the flip side there were nearly a hundred thousand podcast channels, so our python scraper took several days to go through the whole service, pull info from iTunes on every podcast and then match it to a public RSS feed.

The end result was 100,000 more podcast channels were pulled in. We then imported and integrated into the tracker. Our directory continues to grow. There were several lessons learned in scraping a site of this size, but that’s info for another day.

Once we added all these new podcast channels, several scaling problems hit us and meant we needed to tweak several of our database queries so some of the basic pages remained usable. Similarly we had to tweak several aspects of our code that update podcast artwork and basic info too. All told this means we know have better coverage of podcasts available for the tracker and solid information architecture to build from.

A couple smaller feature additions were:

- OPML Importer so you can import your podcast channels from Overcast, Pocket Casts and others
- Exporter of Your Podcast Listening Stats by Podcast
- Dozens of minor and bigger changes

{% picture center /images/2017-resources/export-of-podcast-listening-stats.jpg %}

So, let’s call what we have version 1.1: Our DIY podcast tracker now has a database of over 196,158 podcast channels (but who’s counting) and over 111,942 episodes too (and that will continue to grow as we spider the web). As a user, we’ve added an OPML importer. So, if you use Overcast, Pocket Casts or another service that lets you export your podcast subscriptions, you can now quickly sync your podcast subscriptions. As a service we check and pull the latest episodes regularly and allow podcast tracker to manually log when they listen to an episode. We’ve add a simple feed of the latest episodes, a history page with an export and statistics page to show how many hours you’ve listened to.

That’s it for Version 1.1. It’s live and we are still looking for early testers and users. The product is stable and we continue to develop it. If you are interested in joining, drop me an email at markwkoester@gmail.com.

What’s next? After much consideration, I’ve come to realize that it’s time to build for mobile.

{% picture center /images/2017-resources/podcast-listen-example-02.jpg %}

## Build Me an App: What’s Next? Some Thoughts

So, I’ll admit that I still haven’t come up with a name for this service. So that’s something to think about. The name question seems secondary to building a better podcast listening application. At a certain point I stick a name on this thing and start promoting more. For now, I’m building this for myself, for my friends and for my fellow trackers.

I’m currently quite happy with the prototype we’ve built, but the main limit is that it doesn’t track as you listen. There are a few options here. Namely we could start to work out a web version where you can listen and track, but I find that since podcast listening happens mostly in mobile, it’s time to think about building an app.

At present the current web version is mobile friendly and it isn’t any harder to log your episodes and listening on a mobile browser. But there is something different about the experience on an app. With touches and swipes, logging becomes a lot more enjoyable. In terms of UI and User Experience this makes sense to build a version that puts the logging together. So first step would be a simple list app with taps and swipes to log your episodes.

This, of course, will sync to the web version. This means turning the web version into more of a backend and API too.

I also think part of the point of tracking is pulling that data together to see yourself and share it back, so like tracking your runs and sharing a photo or map, I want to track podcast listening an share a portrait of it for social media. The quantified self movement contains a lot of elements, but we are just now beginning to see the benefit beyond capturing data points. In fact, I’d argue that real value comes in knowing your data and taking into something else via a story, a collection of data or a goal to work towards.

This leads me to the next big next for my podcast tracker: an app for podcast listening and tracking. Currently my building process has been focused on the backend and simple manual tracking. But to make this all work we need an application that lets us pull in the podcasts we love and listen to them, and then through listening to them, we collect a record and track our usage. It’s just that simple.

Over the last month, I’ve been polishing off my mobile development skills and started work on building a React-Native podcast listening app. It’s far from ready, but I’m making progress. The first version will likely focus on just logging your listens in a mobile friendly way and connect to the main backend. There are some challenges in audio and file management in react-native that I need to sort out before going into downloading episodes and mobile listening. Definitely going to happen though, and super excited to build it.

Here’s to more tech for tracking your podcast listening. Send me your thoughts and feedback in the comments or via email.
