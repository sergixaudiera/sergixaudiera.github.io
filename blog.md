---
layout: page
title: Blog
description: Recent posts by Sergi Xaudiera
permalink: /blog/
---
<aside>Things I’ve written, papers and thoughts</aside>

<ul>
  {% for post in site.categories.pro %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> <date>({{ post.date | date:"%B %Y" }})</date>
    </li>
  {% endfor %}
</ul>
