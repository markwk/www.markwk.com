---
title: Off of WordPress, EmPowered by Jekyll
author: Mark Koester
layout: post
permalink: 
blr_date:
  - 2013-04-21
categories:
  - Geek Talk
  - WordPress
  - Migration
  - Jekyll
  - Writing
  - Octopress
  - Technology
published: true
comments: true
---
# 
{% img center /images/2013-resources/octopress-logo.png %}
**This Blog is Now Powered by Octopress, a Member of the Jekyll family.**

I've been itching to get my personal blog off of WordPress for sometime. I considered migrating it to Drupal. Since I mostly work with Drupal, this kind of made sense and, in the process of figuring out how to do it, I even wrote a blog post called *[Drupal vs WordPress](http://int3c.com/blog/2012/11/why-migrate-wordpress-drupal-drupal-vs-wordpress)*. It's actually one of my post popular Drupal articles.

Even though I pay my bills building and fixing sites built with Drupal, I didn't really want another site on Drupal. Drupal provides awesome interactive sites and is really powerful for ecommerce and other community-type projects. But for my blog it's a bit of an overkill. It's mostly just static text. Databases be damned! CMS enough! 

So, with a couple hours to kill, I decided to get to the heart of blogging geekiness with a Jekyll-powered blog using [Octopress](http://octopress.org). 

Here's the what's, why's, and how's in moving my WordPress blog onto a Jekyll/Octopress setup, a ruby-power generator for creating static HTML websites. 

<!--more-->

## A Site in HTML? No Way!

So, normally when you hear about people with their site in HTML, you get worried. No, worse yet scared. For me, it's visions of former clients and their favorite html editor (I mean you Dreamweaver!) and blotted content mixed with design markup. Generally, as a web developer these are the "migration" projects you spend copy-and-pasting. 

In today's world of modern web design, we expect our sites to be dynamic and powered by the latest and greatest programming languages and database servers. In many use cases, a full-blown CMS or web application makes sense. For a largely static blog, it's not needed. 

Jekyll is Github.com site creation engine that converts static text files and combines them with a layout system to build full html site export. It removes the need for anything more than a webserver to deliver static content. 

Say goodbye to databases, web programming languages and various performance enhancements. Say hello to Octopress. 

## The Why's? 

There are a lot of good articles out there about the benefits of this type of blogging setup: performance, simplicy, freedom, cost, etc. 
But for me, the main reason I like Jekyll/Octopress and ended up migrating my personal blog (which wasn't particularly fast or easy)  came down to this one reason: the zen simplicity and usability of writing in **markdown**. 

I know there is a place in this world for text rich editors, but for me, WordPress is not a very clean way for me to write. Too many distractions. Too many stylistic obstructions. 

I really enjoy writing in less cluttered text format. Screw Word. WYSIWYG editors be damned. Give me [markdown](daringfireball.net/projects/markdown/) or [textile](http://www.movabletype.org/documentation/author/textile-2-syntax.html) and a text editor like [Sublime Text 2](#) or Textmate. 

Recently, I've been heavily using the [online writing platform Draft](http://draftin.com), which takes the zen state of writing in markdown several steps forward with live save and easy sharing. And it keeps getting better. 

Anyways, that all said, I consider my blogger even though I don't blog as often as I used to and I wanted to get back to a blogging setup that lets me keep me focus on writing easy and provides a solid solution to getting my writing online to be shared. 

## The What: 

#### Jekyll + Octopress = A blogging framework for hackers.

I think [Jekyll](https://github.com/mojombo/jekyll) provides this clean writing and html generation-publication workflow and Octopress takes it a few steps forward with various improvements and generally nice looking design.

So what is Jekyll? What is Ocotopress? How does it all work?

To quote for the [docs](https://github.com/mojombo/jekyll/wiki/Usage#basic-structure), "Jekyll at its core is a text transformation engine." This means the system takes your clean documents written in your favorite markup language like Mardown and it combines it with a layout structure to make it into a website with various links and page structures. 

There are various technologies involved, but mostly it's a series of ruby scripts that pulls the pieces together into a standard, html website. 

Octopress takes this a few steps forward since Jekyll is a bit rough beyond the simple generation of html. To quote:

{% blockquote http://octopress.org/blog/2011/07/23/octopress-20-surfaces/ %}
Octopress is a framework designed by Brandon Mathis for Jekyll, the blog aware static site generator powering Github Pages. To start blogging with Jekyll, you have to write your own HTML templates, CSS, Javascripts and set up your configuration. But with Octopress All of that is already taken care of. Simply clone or fork Octopress, install dependencies and the theme, and you’re set.{% endblockquote %}

To sum it all up, Jekyll + Octopress are a nifty batch of scripts that take your text files and convert into a full out site. The underlying code is pretty straightforward, such that with enough time and patience you can crawl through it make most of the common changes you'll ever need. 

The system is built with a lot of best practices, so you'll learn plenty along the way too. 

## The How: Migrating from WordPress to Octopress

Ok, with all that amazingness out of the way, let's get to the less enjoable part: migrating your current site to Octopress. 

Migrating any site from one system to another can be one of the least enjoyable developer tasks out there. As a Drupal developer, I also get to enjoy the migration process between major Drupal versions, which can take a lot of tiem depending on the complexity of the web application. 

For converting a WordPress site to Octopress, there are a ton of articles and resources out there, especially relevant is this wiki page on [migrating your blog to Jekyll](https://github.com/mojombo/jekyll/wiki/Blog-Migrations). It provided various options. The main thing to keep in mind is that you are looking to convert in a way that you keep what you had before like tags, titles and pathes, but converted now into static text pages that you'll manage outside of a database. 

I tried some of the scripts, but in the end, I used this [WordPress plugin to Export the site to Jekyll](https://github.com/benbalter/wordpress-to-jekyll-exporter). It did a really great job getting all the current blog posts and pages converted to markdown. While there were admittedly a few issues that I had to fix manually, the most important thing was that it was a great starting position. 

My blog isn't particularly huge, so I was able to manually go through and fix any issues. It also gave me a great way to re-read, edit and stylistically improve various posts. I added and fixed some of the links and images. While I am sure there are still some issues I'll come across, I'm pretty happy with the migration. 

Finally, while there are various options for [deploying your octopress site](http://octopress.org/docs/deploying/), I decided to host my site via AWS S3, since I could initially just setup a bucket and upload the files I needed. [This post from Jerome Bernard](http://www.jerome-bernard.com/blog/2011/08/20/quick-tip-for-easily-deploying-octopress-blog-on-amazon-s3/) was helpful on get the deployment process more automated.

## Conclusion: A few hours into a couple days

While I didn't report the full process in this conversion, in the end it took almost two days of work to get the site converted from WordPress to Octopress. I worked on it in my "geek-out" downtime and did quite a few things manually, because I wanted to do it that way to understand the system. Like a lot of things, I'm guessing the next time (if it ever happens) will be a lot faster and easier. 

Conclusion: This conversion to Octopress came after a nice break in Morocco. So watch out: Now that my blog site is in the "markdown/html/deployment" wonderland that is Octopress, no more excuses for not writing and writing more often. **Readers beware**.
