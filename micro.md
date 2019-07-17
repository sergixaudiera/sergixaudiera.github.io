---
layout: page
title: Micro
description: Micro
permalink: /micro/
---
<aside>micro</aside>
<ul>
  {% for post in site.categories.micro %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> <date>({{ post.date | date:"%B %Y" }})</date>
    </li>
  {% endfor %}
</ul>