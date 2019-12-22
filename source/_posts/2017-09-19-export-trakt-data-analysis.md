---
title: "How to Export Your Trakt Watching History for Free (and Do Some Data Analysis)"
layout: post
categories:
  - Tracking
  - Quantified Self
  - Personal Data
  - Track Everything
  - Habits
  - Productivity
  - Self-Improvement
  - TV
  - Data Analysis
  - Data Visualization
comments: true
published: true
permalink: /export-trakt-watching-history.html
---

{% img center /images/2016-resources/tv-watcher-tracker.png %}

[Trakt.tv](www.trakt.tv) is a great, free service for tracking your TV and movie watching. You can manually log what you watch or use additional integrations and tools to automatically track everything on Netflix and other places. 

Whether your goal is  to decrease your TV addiction or mere curiosity at knowing which shows you watch and when, Trakt is one of the best ways to quantify your media consumption. I’ve written previously about [how track your TV and movie watching using Trakt](http://www.markwk.com/2016/10/tv-movie-tracking.html). Personally my main usage is seeing my weekly viewing time statistic, which I can employ in my [data-driven weekly review](http://www.markwk.com/data-driven-weekly-review.html) as a data point to better gauge how much tube time I spent and, if excessive, potentially take action. 

Let’s go one step beyond the actual tracking and start leveraging our data. But first things first is getting our data. 

Tracking services that don’t allow you to export your data should be avoided and honestly have a very bad data policy. Fortunately, Trakt provides a few options to export your data. One option is to become a VIP premium member and to download a CSV export directly from Trakt.tv. Alternatively, you can use a data aggregation service called Zenobase to pull your watching history directly from Trakt.

In this post, we will look at how to export your data from Trakt using Zenobase. First, we will look at how to integrate Trakt with Zenobase; second, at how to do basic data analysis around media time; and third, from there you can use Zenobase’s tools to explore the data, create visualizations and even download a full export of your TV and movie watching history on Trakt. 

<!--more-->

## Data Aggregation with Trakt and Zenobase

{% img center /images/2016-resources/trak-weekly-stats.jpg %}

I am a big fan of Trakt, and it is my preferred service for tracking my TV and movie watching. Each week I pull my weekly viewing time from my dashboard and compare it with the previous week. Along with my productivity score and time log, this stats helps me notice things like burnout, apathy and other potential issues. 

Beyond the tracking itself and this one data point, you’ll need to get access to your full viewing data in order to do anything with it. To get your data, you can either become a full VIP member on Trakt or alternatively you can integrate Trakt with a service called Zenobase. 

{% img right /images/2017-resources/zenobase-homepage.jpg %}

[Zenobase](https://zenobase.com/) is data platform with an emphasis on the quantified self and self-tracking. Zenobase integrates with over 30 tracking services, including some of the most popular like RescueTime, Fitbit, Last.fm, Apple Health, Google Fit, Runkeeper, Strava and several others. It also has an API and import options for add all kinds of other data. As their tagline says, Zenobase helps you “store, aggregate and visualize your data.” 

Zenobase is not quite as simple to use as other data aggregation services like Gyroscope or Exist.io, but it is also significantly more powerful and flexible since its main feature is allowing you view, compare, and correlate disparate data points. 

Adding data into Zenobase is quite straightforward. After creating an account, you create a “bucket,” which in Zenobase parlance is where you pull in and add data. Your bucket can be an empty data set and you’ll have to manually import your data or you can choose one of roughly 30 sources from which Zenobase will directly pull data. Once an external services is added, you’ll be required to confirm your credentials. For example, if you add either Strava or RunKeeper as a bucket, you’ll be asked to confirm this integration and your data is then automatically synced to Zenobase. 

With Trakt, it’s super simple to add on Zenobase. All you need to do is create a bucket and set “Trakt.tv” as the source. 

{% img center /images/2017-resources/zenobase-create-bucket-for-trakt.jpg %}

Once Zenobase finishes syncing your history, you’ll get a timeline graph like this: 

{% img center /images/2017-resources/zenobase-trakt-watching-history-chart.png %}

I’ve been tracking my TV and movie watch for a bit over a year and logged 348 shows so far. This graph is a week-by-week breakdown of how many hours I watched. 

Let’s look at some data analysis and visualizations of our media watching using Zenobase. 

## Data Analysis and Data Visualizations of Media Watching with Zenobase and Trakt

Now that we’ve been tracking our shows for awhile with Trakt and pulled our data into Zenobase, we can start to do some basic data analysis and data visualizations, two core aspects of data science. While the tracking itself has some benefits, it’s important to take some data to look at the data and gain some understanding from.  

All in all, Zenobase does a great job working with different types of data and, by default, provides several nice representations, including the timeline display. This displays the sum of duration of TV and movie watching each week. 

Another interesting one is the histogram display, which shows line chart count by duration of each movie or TV show. In my case, 205 out of 348 items are 30 minutes to one hour long. 

You also have a count by tag, which you use to represent which genres you watch most or even movies vs TV episodes. In my case, I’ve watched 292 episodes compared to 56 movies. I guess this makes me a TV show watcher! 

{% img center /images/2017-resources/zenobase-trakt-data-analysis.png %}

It’s quite easy on Zenobase to add filters. The simplest are filtering by time and tags. 

This allows us to do some simple data analysis. For example, when I filter by episodes, my most popular genre category by a wide margin is drama, but for the movie type, it’s quite equal distribution between adventure, action, thriller, and drama. It should be noted that films can fall into multiple genres and there is a high correlation between several genres. 

Finally, Zenobase as a data platform makes it possible to create your own displays. For example, in the above example I created my only monthly breakdown using the timeline “widget” display. I set the title, filters and data point I was aggregating (example, sum of durations). 

Here is a quick comparison I did between my watching TV (top) vs movie (bottom): 

{% img center /images/2017-resources/tv-vs-movie-watching-2016-2017.png %}

These timeline charts reveal an interesting recent trend away from TV series and towards movie watching. CONFESSION: I recently binge watched all 9 or 10 Star Trek movies over about two weeks. 

Now that we’ve looked at Zenobase and how we can use it to integrate Trakt data as well as some data analysis and visualizations we can create on the platform, let’s look at how to export our data. 

## Exporting Your Trakt.tv Full History for Free using Zenobase 

While Zenobase does a great job of empowering trackers to look more at their data and create beautiful visualizations, eventually you’ll want to get the raw data. 

If you are a self-tracker, I highly encourage you to take some time to ensure that the services you use to track allow you to export your data. In most cases, the preferred data format is a plain-text CSV. This allows you to manipulate the data in spreadsheets or in data science tools like Tableau or R Studio. Let’s look at how we can export our viewing history from Trakt.tv using Zenobase. 

Once you’ve integrated Trakt into Zenobase, there is also a hidden “trick” to downloading the underlying data. This is for both the chart data as well as the original raw data. 

To download your full data, click the icon on top right and click on “Export.” This will then open a dialogue popup to enable you download in either JSON or CSV format. 

{% img center /images/2017-resources/export-trakt-data-from-zenobase.png %}

NOTE: This raw export is filtered to your current view so to get all your data, make sure you remove any date or tag filtering you previously added. 

Here is a screenshot of the full export: 

{% img center /images/2017-resources/trakt-tv-raw-export-from-zenobase.png %}

As you can see, the data is quite clean and you should be able to easily clean it up for further analysis. 

To download the underlying data and calculated fields in your filtered visualizations in Zenobase, all you need to do is click document icon which is in between the filter icon and the camera icon. You’ll get a CSV with the various elements like this: 

{% img center /images/2017-resources/export-trakt-filtered-visualization-data.png %}

You’ll then be able to open this data in a spreadsheet with a format as week | sum_duration. For example, "2016-W31 5400000” and "2016-W32 16200000.” 

NOTE: Zenobase exports its duration fields as milliseconds. So to view this in a spreadsheet as a more “human readable” format, you’ll need to convert it to hours and minutes. 

## Conclusion: From Tracking to Analyzing Your Data

By adding Trakt as a data source in Zenobase, you suddenly have access to the data itself and have gone a step beyond just merely tracking. In our case, we used Zenobase to do all kinds of data analysis and visualizations, and we also managed to get a full export our raw data too. 

When it comes to tracking, I often find that we spend most of our time and efforts on the tracking aspects and spend much less on the data analysis. I believe there are two reasons why this happens. 

First, too many folks think tracking itself is the magic, and fail to realize that after tracking their steps or other data point for awhile, they need to engage with the data. Engagement with data can mean a number of things. It could mean pulling the data into a spreadsheet or program to look at it, create visualizations and explore it. It could mean noticing it, gamifying it or logging it week by week in a [data-driven weekly review](http://www.markwk.com/data-driven-weekly-review.html) like I do.  In any case, simply tracking does little unless you are using it as feedback and a measuring stick towards a certain behavior or improvement. 

The second reason why people focus on tracking aspect instead of the data side is that we often lack the skills to deal with data and statistics. While we might be able to balance our finances, we often make incredible cognitive mistakes when it comes to statistics and probability. This was made quite apparent in the wonderful book, “Thinking Fast, Slow,” which chronicles how our minds (even training statistics and psychologists!) fail to make the correct inferences from numbers and probability. Fortunately, we can improve our statistical thinking as well as our skills in working with data. There are tons of books, articles and online courses for those that want to get better with data and statistics. Personally I highly recommend starting with the [Intro to Data Science Course on Udemy](https://www.udemy.com/datascience/), which looks at several key aspects from visualizations and modeling to thinking and presenting as data scientists.  

If you are a tracker and you are using any of the most popular tools to track your time, I highly encourage you to try out Zenobase. It makes it easy to do some incredible data analysis on tons of tracking services. 

In my case, I was able to see a few interesting observations about my media watching. Using the timeline visualization of Movies vs. TV shows, I saw a clear trend towards watching more movies. I also noticed periods in time where my media consumption was particularly high, and without a doubt I’d be able to explore possible correlations with my physical activity levels and productivity from other data points. 

In conclusion, make sure the services you use provide access to your data. Ideally as a CSV. We were lucky that Trakt not only provides a premium way to get your data, but you can also use a “workaround” to get your data for free with Zenobase. 

If you are looking for more on media tracking, check on my posts on how I use [GoodReads to log my book reading](http://www.markwk.com/2016/11/book-reading-tracking.html) or [Evernote to store all the web content and articles I consume](http://www.markwk.com/2016/11/tracking-article-reading.html). I also employ Last.fm for tracking my music listening, and recently I’ve been building a [tool to track podcast listening](http://www.markwk.com/2017/03/podcast-tracker-app-update.html) too. 

What are you tracking? And how are you learning from the data?

Best of luck and happy tracking! 