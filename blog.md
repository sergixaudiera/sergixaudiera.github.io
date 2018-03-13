---
layout: page
title: Blog
description: Posts published by Sergi Xaudiera
permalink: /blog/
---
<section class="posts">
  {% for post in site.posts %}
		<p><a href="{{ post.url }}">{{ post.title }}</a><time>{{ post.date | date:"%b %d %Y" }}</time></p>
  {% endfor %}
</section>

