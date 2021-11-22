---
title: Blog Categories
layout: page
permalink: /category/
---

I've written across a number of topics. Select the category below to view some articles on the topic.

Click here to view my [complete blog archive](/blog/archives/).

<h2>List of Categories</h2>

<ul>
{% for category in site.categories %}
<li><a href="{{ site.url }}/category/{{ category | first | slugify }}">{{ category | first }}</a></li>
{% endfor %}
</ul>

