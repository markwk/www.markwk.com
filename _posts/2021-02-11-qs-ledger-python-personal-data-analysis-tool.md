---
title: "Give Me My Data, Tell Me a Story: Introducing Quantified Self Ledger"
layout: post
categories:
  - Tracking
  - Data Visualization
  - Quantified Self
  - Personal Data Analysis
  - Track Everything
  - Year-in-Review
  - Year-in-Data
  - Python
comments: true
published: true
date: 2021-02-11
permalink: /qs-ledger-intro.html
featured_image_thumbnail:
featured_image: images/2021-resources/qs_ledger_promo_image.gif 
featured: true
---

Several years ago I was exploring various self-tracking technologies and how I might integrate personal data into my own life. One of the first things I discovered was just how many ways you might [track a life](http://www.markwk.com/category/track-everything/) using wearables, apps and other technologies. The second lesson I learned was just how hard it was to bring all of this data together and start engaging with it, even as a developer and fledgling data scientist.

While it is easier than ever to track a life, bringing all of your data together to visualize and compare it remains a real challenge. Personal data aggregation and data visualization was and has been the main motivation by my open source python data science project, [Quantified Self Ledger](https://github.com/markwk/qs_ledger).

When I started the project a couple of years ago, I was simply trying to share my own journey into improving my python and data science skills as well as make my code available to others too.

### A Personal Data Collector and Data Visualization for a Quantified Self and a Data-Driven Life

Initially QS Ledger was an assortment of python scripts to download and aggregate personal tracking data. I later added some additional notebooks to share examples of data analysis and data visualization. My primary goal was to use python to pull together a bunch of different streams of data and see if I could create something interesting with that data.

Much of my initial work was came out of a couple of [data visualization and machine learning speeches](https://github.com/markwk/python4selftrackers) I gave at Python conferences and data science events, including [A Year In Data with Python](https://rawgit.com/markwk/python4selftrackers/master/year-in-data-with-python/slides.html). Having built a few tools in the quantified self and self-tracking space over the last couple years, including a [podcast listening tracker web service](http://www.podcasttracker.com/) and [PhotoStats.io](http://www.photostats.io/), a private, mobile app for counting and tracking the photos you take on your phone, I was part of a huge initiative amongst developer to create various tracking services. Broadly speaking I've witnessed a rise in [health tracking tools](http://www.markwk.com/health-trackers.html) as well as various methods to quantify our productivity, [time usage](http://www.markwk.com/time-tracking-tools.html) and even [creativity](http://www.markwk.com/track-writings.html).

As I document in my [QS Mind Map](http://www.markwk.com/quantified-self-mind-map.html), if there is something you want to track, quantify or collect data on, then there is probably already a tool, app or service that can help you do it. But what to do if you want to look at, compare and use multiple personal data sources in one place?

Unfortunately the number of options for data aggregation and visualization are much more limited. Additionally, there are privacy concerns about many of these services too.

If data is more than something you want to collect, then QS Ledger might be a tool for you.

So what is QS Ledger?

<!--more-->

### Introducing Quantified Self Ledger: An Open Source Python Data Science Project for the Data Enthusiast

[QS Ledger](https://github.com/markwk/qs_ledger) is open source python data science project that aggregates and visualizes your personal data.

The project has two primary goals:

1. **download all of your personal data** from various tracking services (see below for list of integration services) and store locally.
2. provide the starting point for **personal data analysis, data visualization and a personal data dashboard**

At present, the main objective is to provide working data downloaders and simple data analysis for each of the integrated services. What that means is that it can help you collect your data and offers examples on how to visualize your data.

If you just want to know more about the data you track, then QS Ledger can help you get your data and help you on the journey to exploring it.

If you are interested in creating year in review data infographics like I have in my [year in data series](http://www.markwk.com/category/year-in-data/), then QS Ledger can provide a great starting point.

If you are interested in Machine Learning and Artificial Intelligence on personal data, including health and wellness, then QS Ledger can help you bring together different data streams for predictive analytics and forecasting. I've even used this code to show correlations and make machine learning predictions about [my own behavior over time](https://rawgit.com/markwk/python4selftrackers/master/slides/index.html) too.

Also, if you want to integrate data into a "Getting Things Done"-style [data-driven weekly review](http://www.markwk.com/data-driven-weekly-review.html), QS Ledger can help you create automated scripts for generating reports on your time, health or anything else you track.

### Current Integrations:

QS Ledger currently integrations over a dozen data sources, including:

- [Apple Health](https://github.com/markwk/qs_ledger/tree/master/apple_health): fitness and health tracking, data analysis and dashboard from iPhone or Apple Watch (includes example of Elastic Search integration and Kibana Health Dashboard).
- [AutoSleep](https://github.com/markwk/qs_ledger/tree/master/autosleep/autosleep_data_analysis.ipynb): iOS sleep tracking data analysis of sleep per night and rolling averages.
- [Fitbit](https://github.com/markwk/qs_ledger/tree/master/fitbit): fitness and health tracking and analysis of Steps, Sleep, and Heart Rate from a Fitbit wearable.
- [GoodReads](https://github.com/markwk/qs_ledger/tree/master/goodreads): book reading tracking and data analysis for GoodReads.
- [Google Calendar](https://github.com/markwk/qs_ledger/tree/master/google_calendar/): past events, meetings and times for Google Calendar.
- [Google Sheets](https://github.com/markwk/qs_ledger/tree/master/google_sheets/): get data from any Google Sheet which can be useful for pulling data from IFTTT integrations that add data.
- [Habitica](https://github.com/markwk/qs_ledger/tree/master/habitica/habitica_downloader.ipynb): habit and task tracking with Habitica's gamified approach to task management.
- [Instapaper](https://github.com/markwk/qs_ledger/tree/master/instapaper/instapaper_downloader.ipynb): articles read and highlighted passages from Instapaper.
- [Kindle Highlights](https://github.com/markwk/qs_ledger/tree/master/kindle/kindle_clippings_parser.ipynb): Parser and Highlight Extract from Kindle clippings, along with a sample data analysis and tool to export highlights to separate markdown files.
- [Last.fm](https://github.com/markwk/qs_ledger/tree/master/last_fm): music tracking and analysis of music listening history from Last.fm.
- [Oura](https://github.com/markwk/qs_ledger/tree/master/oura): oura ring activity, sleep and wellness data.
- [RescueTime](https://github.com/markwk/qs_ledger/tree/master/rescuetime): track computer usage and analysis of computer activities and time with RescueTime.
- [Pocket](https://github.com/markwk/qs_ledger/tree/master/pocket/pocket_downloader.ipynb): articles read and read count from Pocket.
- [Strava](https://github.com/markwk/qs_ledger/tree/master/strava): activities downloader (runs, cycling, swimming, etc.) and analysis from Strava.
- [Todoist](https://github.com/markwk/qs_ledger/tree/master/todoist): task tracking and analysis of todo's and tasks completed history from Todoist app.
- [Toggl](https://github.com/markwk/qs_ledger/tree/master/toggl): time tracking and analysis of manual timelog entries from Toggl.
- [WordCounter](https://github.com/markwk/qs_ledger/tree/master/wordcounter): extract wordcounter app history and visualize recent periods of word counts.

Have an area you are tracking or tool you are using that isn't include? Post a request in the [issue queue](https://github.com/markwk/qs_ledger/issues) or add your own integration to the project.

### Who is the project for? What do I need to get started?

While the project is generally for technically competent individuals, QS Ledger is intended as a beginner friendly data analysis and data science project. All you need is some basic knowledge of Python and a working installation of the Python Data Science stack. One good starting point is the [Anaconda Distribution](https://www.anaconda.com/download/#macos), which is cross-platform and will give you nearly all of the code you'll need to start using QS Ledger.

In terms of key highlights:

- The code is written in Python 3.
- Shared and distributed via Jupyter Notebooks.
- Most services depend on Pandas and NumPy for data manipulation and Matplot and Seaborn for data analysis and visualization.

### How to Install and Get Started

Until we provide a working version for Google's Collab or other online jupyter notebook setups, we recommend to get started by downloading and using the [Anaconda Distribution](https://www.anaconda.com/download/), which is free and open source. This will give you a local working version of Numpy, Pandas, Jupyter Notebook and other Python Data Science tools.

After installation, we recommend create and activating a virtual environment using [Anaconda](https://www.geeksforgeeks.org/set-up-virtual-environment-for-python-using-anaconda/) or manually:

`python3 -m venv ~/.virtualenvs/qs_ledger`

`source ~/.virtualenvs/qs_ledger/bin/activate`

Then clone the current github repo:

`git clone https://github.com/markwk/qs_ledger.git`

Using your activate virtual environment, install dependencies:

`pip install -r requirements.txt`

Then navigate into your directory and launch an individual notebook or the full project with jupyter notebook or jupyter lab:

`jupyter lab`

After that, you can navigate to any number of data directories to continue your configuration and setup for the relevant service. For a deeper dive into one example with Apple Health, checkout my past post on [How to Export, Parse and Explore Your Apple Health Data With Python](http://www.markwk.com/data-analysis-for-apple-health.html).

### Conclusion: Tips for New Python Data Scientists

On a surface, QS Ledger might look like a tool for experienced developers and technical folks, but speaking from my own journey to learning data science and machine learning, this is the kind of project and code for newbies too. In fact, one of my missions for this project is bring greater accessibility to personal data analysis and data science with Python. I highly recommend giving the project a try if you are new to python data science and you are looking for a way to work with new data sources.

Here are a couple tips for anyone getting started:

- **Completely new to python and data science?** Check out [Python for Data Analysis: Data Wrangling with Pandas, NumPy, and IPython](https://www.amazon.com/Python-Data-Analysis-Wrangling-IPython/dp/1491957662/) by Wes McKinney as well as the tons of example jupyter notebooks you can find at Github.
- **New to Personal Data Analysis? Start with a single data source**: While it can be tempting both personally and as a developer to want to work with lots of different data points, I have found a ton of value focusing just one data source and personal data question at a time.
- **Link your personal health goal with self-tracking and personal data analysis**: One of the best ways I've found to reach my goals and change my behavior is through self-tracking. Even better when you pursue a goal is to link it with other projects you are working on. Considering getting more exercise or sleeping more, start tracking with Strava, Oura, Fitbit or Apple Health. Then using QS Ledger to create your own data visualizations.
- **Focus on Project-Based Learning**: While online courses and books can be a great start to your learning, there is no replacing working on projects. QS Ledger might be a great way to get started but you can only get so far with copy and paste code. Eventually you need "cut your teeth" by creating something on your own, ideally something no one else has done.
- **Not sure what project to work?** Reach out or post to the issue queue. I'm always looking for collaborators and happy to help anyone learning python data science too.
- **Blog or Contribute to Open Source**: As you learn and grow as a data scientist and technical person, be sure to write about in a blog or even better contribute to open source software. Nothing sets apart a candidate for a job better than open source code or a launched product.
- **Stuck? Take a break and try again later**. Good things come through working on hard projects and challenge. Also don't be afraid to google or ask around for help.

Good luck on your personal data journey. Please like and share QS Ledger with your friends. And if you are in need of a data-centric product person, contact me [here](http://www.markwk.com/contact).
