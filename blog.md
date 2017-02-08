---
layout: page
title: Blog
permalink: /blog/
---
<section>
  {% for post in site.posts %}
		<time>{{ post.date | date:"%Y/%m/%d" }}</time> : <a href="{{ post.url }}">{{ post.title }}</a><br>
  {% endfor %}
</section>

