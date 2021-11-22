---
title: Blog Categories
layout: page
permalink: /categories-list
---

<ul>
{% for category in site.categories %}
<li><a href="{{ site.url }}/category/{{ category | first | slugify }}/index.html">{{ category | first }}</a></li>
{% endfor %}
</ul>


