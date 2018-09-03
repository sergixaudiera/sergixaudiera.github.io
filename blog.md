---
layout: page
title: Blog
description: Recent posts by Sergi Xaudiera
permalink: /blog/
---

{% for post in site.posts %}
[{{ post.title }} ]({{ post.url }})  <span style="color: #6b737b">{{ post.date | date:"%Y/%m/%d" }}</span>   
{% endfor %}
