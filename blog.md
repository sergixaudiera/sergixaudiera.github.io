---
layout: page
title: Blog
description: Recent posts by Sergi Xaudiera
permalink: /blog/
---
## Recent posts

<ul>
{% for post in site.posts %}
	<li><a href="{{ post.url }}">{{ post.title }}</a> <small>{{ post.date | date:"%d %b %Y" }}</small></li>
	{% endfor %}
</ul>
