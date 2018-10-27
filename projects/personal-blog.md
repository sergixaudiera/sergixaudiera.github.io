---
layout: page
title: Personal Blog
description: Personal Blog Archive
permalink: /blog/personal/
---
<aside>personal blog (2007 - now)</aside>
I started blogging on 2007 about life and thoughts, studies, work and hobbies.

<ul>
  {% for post in site.categories.personal %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> <date>({{ post.date | date:"%B %Y" }})</date>
    </li>
  {% endfor %}
</ul>