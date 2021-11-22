---
title: "Migrating to Jekyll, Again: How to Migrate Your Octopress Blog to Standard Jekyll"
layout: post
categories:
  - Web Design
  - blogging
  - Migration
  - Jekyll
  - Writing
comments: true
published: true
date: 2021-02-26
featured_image_thumbnail:
featured_image: /images/2021-resources/markwk-blog-migration-2021.jpg 
---

This blog is written in markdown, generated using Jekyll and hosted in plain old HTML. It's all managed using Jekyll, a ruby-based static site generator, and it's *roughly* the same setup I've had for nearly 7 years. I love it. But after being such a mainstay of my life as a blogger, it was time to migrate this site from Jekyll to...well...Jekyll. 

After nearly 7 years hosting my blog on a flavor of Jekyll called Octopress, it was time to migrate my site from that setup on Jekyll to another one. 

In this blog post I want to share a few challenges I faced migrating my blog from Octopress Jekyll to "Standard" Jekyll. First I want to share what I love about Jekyll and Why I had to migrate / update my site. Second, I explain a few issues I dealt with them in keeping certain features with more standard Jekyll. Specifically, we will look at how to retain liquid image tags, the archive page, dedicated category pages, a RSS feed, SEO, and a few other components. Hopefully, by the end of this post, if you are someone migrating from Octopress to "Pure" Jekyll, you'll understand your migration and upgrading path. Let's dig in! 

### Why Jekyll (and a Plaintext Markdown Writing Life) Rocks

I'm a huge fan of the [Jekyll Blogging Setup](https://jekyllrb.com/) setup for a number of reasons:

- First, since it's hosted in HTML, there is no backend or database to manage. 
- Second, removing dynamic content and dedicated programming languages means it loads fast. 
- Third, Jekyll lets me write in markdown, a simple and clear plain text formatting syntax that only requires the basic text editor to manage. In fact, as I explain in one of my more popular posts, [The Plaintext Life](http://www.markwk.com/plain-text-life.html), I use markdown and plaintext files for nearly all of my work, including note-taking, writing and blogging. 

One of my first steps into the world of markdown and plaintext workflows was in 2013 when I elected to migrate my then Wordpress blog to Jekyll. 

As I explained in [Migrating from WordPress to Octopress / Jekyll](http://www.markwk.com/2013/04/wordpress-migrations-to-octopress-blog.html), [Jekyll](https://jekyllrb.com/) allows you to write files in markdown and then, using a few simple commands, generate a static, html site. The generated site can then be hosted on nearly any server, including Amazon S3 buckets as I do or using Github Pages. 

When I switched this blog to Jekyll in 2013, I used one of the most popular and trending approaches to blogging on Jekyll, Octopress. Octopress offered a number of improvements to blogging in Jekyll and, to be honest, I liked the slick default theme it came with. I've really enjoyed Octopress and honestly wouldn't mind continuing to use it today. 

Fast forward several years and unfortunately, like many open source projects, Octopress is no longer being developed, and its support has wained. If I was retired or had additional open source dev time to spare, I'd love to contribute to its maintenance and on-going support. Unfortunately, while I've managed to keep the Octopress scripts working through several updates on Mac OS, my recent upgrade to Big Sur meant it was going to increasingly challenging using the version of Ruby supported by Octopress. So, in view of the lack of maintenance support, I decided it was time to "migrate off" of Octopress Jekyll and use a more "standard" Jekyll setup going forward.  

Additionally, I wanted to keep as much as I could that I liked about Octopress, especially category pages and the main archive listing of blog posts. Like any web product I build and design for, a migration or upgrade was a good opportunity to sharpen the look, feel and usability of the product too. Even though the primary goal was migration and visual polish, it never hurts to improve usability too. 

### How to Migrate Your Octopress Blog to Standard Jekyll

In order to migrate to Jekyll from Octopress, I recommend starting with a vanilla default version of Jekyll. So, go to [jekyllrb.com](https://jekyllrb.com/), download and setup Jekyll locally. 

Once you have Jekyll running, you should be able to simply copy and past all of your pages, posts and assets into the new directory. There is a chance that your blog will work as is. 

If not, don't worry. It's highly likely at this stage that you are going to hit the first of a series of hiccups in migrating. For example, if you use a few core features of Octopress (like image liquid tags syntax, category pages, or the blog archive), you'll need to drop those features or find fixes. Let's look at a few key fixes I made to get my site working: 

### Fixing Broken Images: Enabling Liquid-like Image Tags

Unfortunately, one biggest gotcha leaving Octopress are liquid image tags, which was basically a simple syntax for embedding image ([Ref](http://octopress.org/docs/plugins/image-tag/)).

Unfortunately, though I didn't know this at the time when I started using Octopress, this syntax is break with standard markdown which embeds images in this syntax: `![](path-to-image-file.png)`

Since basically every single one of my posts has images embedded in this liquid tag syntax, I explored a few fixes. One option would be to parse and update all of my old posts to reflect standard markdown. 

The other option I found and one I used involved adding the [jekyll_picture_tag plugin](https://rbuchberger.github.io/jekyll_picture_tag/), which not only provided the same syntax but also provided image versions optimized for screen size and mobile. The only bulk change I needed to make was to replace img with picture.  

Though you may need to manually fix some posts, this plugin is a solid fix for migrating off of Octopress and keeping the same markup for images in your posts. 

(NOTE: The only issue I still face here involves positional tags like left, right, and center which normally adds css markdown for positioning images around text.) 

### Wow, Default Jekyll Looks Terrible: Finding a Starter Theme

While structurally default Jekyll is great, it doesn't really provide anything reasonably good looking out of the box. So one of the first things you'll want to do is get a new theme or design. 

One option is to create or adapt an HTML template. Since Jekyll is HTML centric, an HTML theme would be easy to adapt on a Jekyll blog. 

Another option and the route I took was using a template on [jekyllthemes.io](https://jekyllthemes.io/). There are a lot of decent free options and nice paid options too. Many are adapted for specific use cases too. If you are looking to support open source and designers and developers (and to save your time), buy a theme you'll love.  

Admittedly as a designer, I could have designed and created a custom look and theme. But frankly, my goal on this site is to focus on writing and providing good content to my readers. So I bought a theme and did my tweaks on that. I just wanted a theme that looked great on all screen sizes and created an enjoyable and aesthetically pleasing reading experience. I didn't want to spend days designing and developing when I could be writing and creating in other ways. 

Following a few more minor tweaks here and there and an hour or two of manual blog edits, I went ahead and relaunched the site with my latest blog posts. Warts and all. 

### Setting Up Dedicated Category Pages

Ok, now that we got our basic migration accomplished, we should have a functioning Jekyll blog and maybe even a decent theme too. Now what to do about some missing "Octopress" features on Jekyll? Can we fix those? 

For me, one of the biggest features missing from switching to pure Jekyll for this blog was dedicated category pages. With Octopress, I really liked the idea of providing a single link for all of the writings I've done on a topic. I regularly share out and reference two of my most popular series via the category page, namely [Tracking Everything](http://www.markwk.com/category/track-everything/) and the [science of goals](http://www.markwk.com/category/science-of-goals/). So I was sad when I migrated off of Octopress without dedicated category pages. 

Unfortunately, while a lot of documentation on Jekyll claims that it is easy to create such pages, setting up category pages turned into the biggest time suck of this conversion. I ran into a number of issues with code I found on GitHub and fixes I found on several blog posts regarding generating category pages with Jekyll. Frankly I don't know why I had so much trouble. For example, was it again a syntax issue or problems in the code I found. 

Anyways, after several attempts, I finally found a solution using a couple snippets of code, which I aggregated and shared in a Github Gist [here](https://gist.github.com/markwk/52d00f3f4e1ef1598fc2fb58f5b8ab7c). 

Here are the steps to make it happen:

1. Create a file named GenerateCategoryPages.rb, add it to the _plugins directory and copy and paste the snippet below.
2. Create a file named category_index.html, add it to the _layouts directory and copy and paste the snippet below.
3. Regenerate your website using `jekyll serve` or `bundle exec jekyll serve`.

For me getting my category pages working again was one of the highlights of this "challenge."

### Creating a Archive Page

While generating category pages required several attempts, fortunately generating a replacement archive page was easy. All you need to do is create a markdown file for a page can include the following code: 

{% picture center /images/2021-resources/archive-page-snippet-jekyll.jpg %}

This code is a loop that will generate a list of past blog posts. In my case, I'm keeping it as just the date of publication and the title, but you could easily update this to include tags or categories or even feature images too. 

### Providing an RSS Feed

I know that blog syndication via RSS or Atom feeds is what it used to be, but I still personally believe it's a feature I wanted to maintain. This is probably a topic for separate rant someday, but I personally think RSS subscriber approach to blog and article consumption makes a lot of sense. It allows you to get updates from blogs or podcasts you follow and read and display them as you like.  

Anyways, leaving aside my political opinions on decentralized content syndication, setting up an atom or rss is pretty simple with Jekyll. In my case I installed jekyll-feed plugin and tweaked the rss location so my long-time RSS subscriptions should continue to get updates. 

### BONUS: List of Links to Categories

Here is a little [snippet](https://gist.github.com/markwk/db151fc91eb8f08a2891fd0ac68a28a9) you can add to an html or markdown page to generate and list all of your categories as links. 

### Conclusions and Meta Thoughts on Blogging Going Forward

Hopefully this post provided some tips for dealing with common issues you might face migrating off of Octopress to more standard Jekyll. There are plenty of additional customizations and tweaks you might add to improve your blog. Jekyll is relatively easy to learn if you want to go deep on creating some pretty powerful content focused sites.  

I personally think a markdown blog is a powerful enabler of creatives today. It's easy to host it anywhere. You can even host it using Github pages for free. By using disqus, you get free comments too. While a Wordpress or Drupal site might be easier for blogging, they come with challenges too, especially around updates and databases. Jekyll removes many of these limitations and lets you focus on writing and publishing. 

A couple years ago, I migrated off of Evernote and now use [plaintext for my note-taking](http://www.markwk.com/plain-text-life.html) and my [knowledge management system](http://www.markwk.com/smart-notes.html). This means that nearly all of my research and note-taking as well as my final outputs and writings are all done in markdown files. This has enabled me to take on harder learning and writing challenges while also focusing on making writing and output of my writing as seamlessly as possible. 

For me as a blogger, 2020 was a difficult year to write and publish. I had just moved to Los Angeles, California, roughly 4 months before COVID-19 resulted in a near continuous state of lockdown that is now going on nearly a year straight. My initial gratitude at **not** being in China when coronavirus struck has slowly pivoted into a degree of acceptance of just how poorly the United States as a government and society has dealt with this pandemic. It's not been a great year anywhere and I'm glad to have had remote work and some positive impacts in my community. I'm still writing and creating, loving and living, especially around the intersection of tech and human betterment. I'm hopeful that things will change soon for the better, that we will all get vacinated, and that the United States and world will emerge stronger and more resilient. 

Selfishly, after enjoying more time to be in one place, I'm also excited to travel again one day soon. In the meantime, I'm happy to be blogging and writing in the open again. 

To borrow a phrase following my last blog migration 7 years ago that grew into a great sprout and period of blogging productivity: **Readers beware**. 