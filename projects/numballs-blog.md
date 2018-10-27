---
layout: page
title: Numballs Blog
description: Numballs Blog Archive
permalink: /blog/numballs/
---
<aside>numballs blog (2012 - 2018)</aside>
We published a mixed of company related, social media sports and data analysis posts.

<ul>
  {% for post in site.categories.numballs %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> <date>({{ post.date | date:"%B %Y" }})</date>
    </li>
  {% endfor %}
</ul>