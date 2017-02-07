---
layout: page
title: Blog
permalink: /blog/
---
<section>
    {% for post in site.categories.pro %}
    {% unless post.next %}
    	 <h2>{{ post.date | date: '%Y' }}</h2>
    {% else %}
      {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
      {% capture nyear %}{{ post.next.date | date: '%Y' }}{% endcapture %}
      {% if year != nyear %}
        <h2>{{ post.date | date: '%Y' }}</h2>
      {% endif %}
    {% endunless %}
		<time>{{ post.date | date:"%Y/%m/%d" }}</time> : <a href="{{ post.url }}">{{ post.title }}</a><br>
  {% endfor %}
</section>

