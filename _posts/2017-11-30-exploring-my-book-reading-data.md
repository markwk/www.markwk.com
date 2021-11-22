---
title: "How Do I Read?: A Reading Data Exploration with GoodReads and Tableau"
layout: post
categories:
  - Tracking
  - Data Visualization
  - Reading
  - Track Everything
  - Media Tracking
  - Tableau
  - Data Analysis
comments: true
published: true
permalink: /reading-data-visualization.html
---

{% picture center /images/2016-resources/tracking-your-book-reading-guy.jpg %}

The facts: I read between 3 and 6 books per month. I finish more books on Weekends and Friday’s than during the work week. The number of books I’ve read stands at 831 (as of late Nov 2017). The average length of the books I finish is 352 pages. Currently I’m reading 58 pages per day. At my present reading pace (~3.438 books per month), I’m on track to complete [my 2000 book reading challenge](http://www.markwk.com/2016/06/2000-book-reading-challenge.html) by spring 2045.

**How did I get to these numbers? And what else do I know about my reading trends and behaviors?**

I currently use GoodReads to track my book reading. I can log when I start and finish a book. With an export of my reading history, I can use Tableau to explore that data. Tableau is a great and relatively user friendly tool for data visualization. The software allows you to pull in data from different sources and create charts and graphs of that data.

Quite simply when it came to my reading, the question was “How do I read?”

With these questions and tools in mind, let’s explore data visualization on my book reading with GoodReads and Tableau.

<!--more-->

## My Book Reading Trends Since 2013

By my count, I read 598 books prior to 2013. I only started using GoodReads regularly in 2013. Previously to that I had logged my book reading in a now defunct service. Luckily I was able to transfer the majority of my reading list into GoodReads.

Using Tableau, I filtered out non-read books and books before 2013 to create a simple breakdown of books and pages read per year since 2013 as well as my trending line (per month):

{% picture center /images/2017-resources/data-visualization-with-goodreads-02.png %}

Interestingly the top charts reveal how I’m clearly not reading books of the same length year on year, and in some cases like 2014 and 2017, I’m reading fewer books but books of longer length. This leads to a pretty consistent number of pages read, though you can clearly see a trend towards more reading in the last two years.

Depending on how you look at book reading, it’s important to remember that a pure count of books read may not be as revelatory when you consider whether you are reading longer or shorter books. As my brother confessed during last year’s reading challenge, it’s probably not "fair" to include graphic novels.

This bottom chart show my trends. While I generally use R for predictive modeling and certain visualization, Tableau makes a decent data science tool in certain scenarios too. In this situation, Tableau was able to look at my plotted data and create a linear prediction for the future. Based on the patterns in my past reads by month, I can show and predict a positive trend line towards reading and finishing more books in the future. For clarity, I’ve also noted my upper and lower confidence bounds, which are used to show the range of these predictions assuming I read less or more.

These charts only took a few minutes to create, and I was already able to plot some interesting discoveries.

## How I Track My Book Reading with GoodReads

I track a [number of areas](www.markwk.com/category/tracking-everything) in my life with a focus on health, time and productivity. I’ve become increasingly dedicated to media tracking, i.e. logging the books, [podcasts](http://www.markwk.com/how-to-track-podcast-listening-with-screenshots.html), music, [tv shows and movies](http://www.markwk.com/2016/10/tv-movie-tracking.html) I consume. Most are simple one-off manual tracking events that I can check-in from my phone or computer.

I’ve yet to pool all of this media tracking together or build anything, but I believe this media tracking will help me in the future. For example, I’m optimistic that I’ll be able to optimize and better filter my media consumption, and I hope to have my own AI someday that can be there to help me to find the things I want to read, watch, listen to and learn.

Most media tracking is part of a social network where we share what we consume and discover what our friends and family are consuming. This is especially true with GoodReads, the service I use to track my book reading.

GoodReads is first and foremost a social network for readers and writers with its main “currency” being sharing the books you read and review and finding future books to read on day.

As I examine in detail in [Tracking Your Book Reading, Data Points to the Soul](http://www.markwk.com/2016/11/book-reading-tracking.html), there are several ways to record what you read and when. From a physical journal to a spreadsheet to an online logging tool like GoodReads, there are pro’s and con’s to each choice. Tracking may not be a central feature of GoodReads, but it's a central function and works quite well. With GoodReads you manually log the books you read.

The social aspect of GoodReads as well as the yearly reading challenge create a decent incentive to track your reading and share your progress.

**One tip for better tracking your book reading is to make sure you log both when you start and when you finish a book.**

One mistake I made when I started the service was that I didn’t mark when I started reading a book. Simply logging when you finish can result in the appearance that you read some books in a single day. Going forward, I'll do my best to log when I started a book and when I finished.

In terms of statistics and charts, GoodReads provides two that you seem most useful: books read and number of pages read. Beyond that you might use custom bookshelves to track certain other things like types of books. The tracking angle isn’t GoodReads strength. It’s strength is the social interactions around reading and recommendations engine. Both of which do a good job of helping me find good things to read.

## My Reading Behavior: Days of the Week and Month-on-Month

Based on the export of data you get from GoodReads, it’s possible to visualize some of my reading behavior. For example, I can see my reading behavior by day of the week and even throughout the year by month.

**NOTE:** One caveat about this data and visualizations is that it’s based on “Date Read,” which is when you finished a book for GoodReads. This is not a great metric, especially by itself. It’s biased towards when you finish and doesn’t capture the trend or reading behavior across the reading period. Likely I should consider nuancing this data by averaging pages read from start date to finish date. Unfortunately your start date isn’t in the export.

That said, all things being equal, if I’m reading more on these periods, then the chance are that I’ll also be finishing more books as well.

Looking at these charts, not surprisingly I read more on the weekend and on Fridays. On Monday to Thursday I tend to read less (since I’m most likely working).

{% picture center /images/2017-resources/data-visualization-with-goodreads-01.png %}

Interestingly when I visualized and compared my reading behavior according to months of the year, it’s appeared that I had found a pattern as well: I read by far the most in August. I read the least in December. Both April and July were low reading months for me.

Overall, I plotted a trend line which, following a dip in winter, predicts an increase after January through summer and a decrease leading into winter, which is curious and somewhat counterintuitive. It would indicate that summer holidays is when I read more while winter’s I read less. I’d be interested to see if there is an offset somewhere in my other other time logs, like in winter, do I watch more TV and movies? play more sports? work or study more? These are questions to explore in other datasets.

## How to Export Your Data from GoodReads

Once that you’ve been logging your reading for awhile on GoodReads and you’ve seen a few examples of my data exploration and data visualization with Tableau, how do you get your own data?

It’s simple. GoodReads provides a simple way to get your export:

- Step 1: Log onto Goodreads.com
- Step 2: Go to My Books
- Step 3: Go to Import / Export (Also accessible directly using this link: https://www.goodreads.com/review/import)
- Step 4: Select "Export Your Books"

It might take a bit of time. After a few minutes, you can refresh the page to download a CSV your books and reviews that you can open in your preferred spreadsheet application.

## Questions and Patterns in My Reading Data

A few years of data makes it hard to be 100% sure about your predictions and trends. So, when you have doubts, it’s a good idea to add visualizations that better point out discrepancies.

Below is a chart showing my reading trends per month from 2014 to present (late 2017):

{% picture center /images/2017-resources/data-visualization-with-goodreads-03.png %}

As you can see the data isn’t quite as clear as the aggregate trend lines of months we looked at previously. Notably, there are a couple months that fall pretty far out of the average like August 2017 (10) and July 2016 (0).

This is part of the problem with using "Date Read” to look at my reading trends, since if I’m reading a particularly long book during that period, then I may not finish it during a single month. This can lead to a lagging score. You can see this in 2016 where in July I finished “zero” books, but, by contrast, I finished 8 in both August and September. Both those months show an some higher page counts too.

It’s important to note that I typically read between 4 and 10 books concurrently too. So it’s not uncommon that finish several books in succession.

This data would indicate that I may not be finishing as many books in July, but this might be because I’m reading longer books that require more time. In order to explore this question, I believe it will require more data analysis and potentially a different data point like parsing book updates from GoodReads to see how my progress correlates in certain months.

One starting point would be to calculate the average number of pages read per book in a month. Here’s a graph that attempts to explore these relationships:

{% picture center /images/2017-resources/data-visualization-with-goodreads-04.png %}

There is an awful lot going on in this chart, but this visualization starts to tease out something in my reading behavior. Namely, that I was actually reading longer books in 2014 than I was in 2015, 2016 or this current year of 2017.

Let’s add another chart to explore this:

{% picture center /images/2017-resources/data-visualization-with-goodreads-05.png %}

This chart clearly shows that I’m reading slightly shorter books in the last 3 years. While the number of books I’m completing has rising and total pages read has too, I shouldn't forget that I have read several epically long books in 2013 and 2014. This explains of the discrepancies and changes in my reading behavior.

## GoodReads Raw Data: Initial Data Exploration of the Exported Data

In this post, we’ve looked at several visualizations of my reading history using Tableau. It’s a great tool to explore all kinds of data for your business or life. Most of these visualizations depended on two fields: number of items read and date read.

I’d like to turn now to an exploration of the underlying data itself. GoodReads provides you with a CSV export of every single book in your collection. This includes both books you’ve read, books you plan to read, and books you are currently reading.

It’s a mix of your input, stats and some general info on those books. The file includes roughly 30 columns, including the book title, author and year published. It also show you where you store or categorize this book, i.e. your bookshelves.

Unfortunately it does not include the book’s official genre. GoodReads expects you to categorize using your own Bookshelves and Collections. Not having a genre makes it difficult to see patterns in the types of books you are reading from this data. If I wanted to get better about my trends, I’ll need to add my books to bookshelves.

Similarly the export does not include the start date when you begin a book. This is a particularly problematic situation if you want to go into more nuance on your reading behavior using this export. GoodReads does offer a number of RSS feeds and an API to access a lot additional info, so it should be possible to get more data around your reading tracking. But it’s not provided in the main export.

There are several services that can pull your GoodReads history, mash it up with other data, and present some interesting statistics on your reading. Two are worth noting:

- [GR Stats](https://victor.shinyapps.io/gr-stats/) is a simple web app links with your GoodReads profiles, pulls in your data, and display a few charts like breakdown of books per year and percentage of authors you read who are male vs female.
- [Bookworm Statistics](http://bookworm-stats.mveith.com/) pulls even more info to create additional charts about reading speed, top authors and even time period of books read.

Personally I found both of these services provided different results on books read in past years.

One additional issue I noticed in directly exploring the export was that exported book’s ISBN Numbers aren't accurate. I used a common ISBN look up service and got a lot of errors. This might be an approach issue, but it still makes it hard to tease out more about the books you read through lookup queries.

All in all, as I’ve shown in this post, there is enough data in the GoodReads export to do a significant amount of exploration around your book reading. Let’s look at one last stat.

## Final Stat: Increasing the Number of Pages I Read Per Day

There are a lot of reasons I read. Pizza Hut’s Pan pizza prizes helped, and I’ll admit that my mother partially “bribed” me. These factors among others that lead to a lifelong passion with read.

But over the last couple years, I’ve deepened and embrassed reading as one of my main hobbies too. I consciously decided to make time for reading and try and read more.

The data shows this:

{% picture center /images/2017-resources/data-visualization-with-goodreads-06.png %}

To put things in perspective I read about 27 pages per day in 2013, 47 in 2014, and 46 in 2015. In 2016, I reached 55 pages per day, and so far, I’ve been reading about 58 pages per day in 2017. It’s possible that I’m reading faster or reading easier books. But most likely I’m simply reading more.

## Conclusion: Observations from Tracking My Reading and Exploring the Data

In this post, we looked at my reading trends using tracking data from GoodReads and data visualization using Tableau. I was able to tease out several things from my reading data, like how many pages I’m reading and my trend towards more reading from 2013 to now.

While on the surface of it, this kind of data exploration might not appear to be all that meaningful. But for me, it’s a confirmation of an on-going effort to read more and read books. I believe firmly that reading is one of the greatest things I can do with my time, and reading helps me think wider and deeper. Having these tracking logs and exploring this data indicates that this habit and passion for reading still has room to grow!

What about the actual words and books I’m reading? Unfortunately, we didn’t have time to explore the actual content or highlights from what I'm reading. I do most of my reading on a Kindle. There are lot of advantages using an eReader, but for learning and self-trackers, one of the great features are highlights. In the books you read you can mark up different passages. These passages can be exported and saved for later. I hope to share more on that data in a future post.

I also have another data set that mashes up my books read with more data on the books themselves like genre, gender of author and publish data. I hope to try and tease out more trends on the kinds of books I’m reading and potentially see correlations on my review scores too.

Both of these avenues about the data of my reading highlights and about the books themselves presents some great source material for more data analysis and data visualization.

I hope you enjoyed this post. I sure did enjoy writing it. Best of luck and happy tracking!
