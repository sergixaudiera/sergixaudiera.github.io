---
layout: page
title: Blog
description: Posts published by Sergi Xaudiera
permalink: /blog/
---
## All Blog articles

<ul>
{% for post in site.posts %}
	<li><a href="{{ post.url }}">{{ post.title }}</a> <small>{{ post.date | date:"%d %b %Y" }}</small></li>
	{% endfor %}
</ul>
