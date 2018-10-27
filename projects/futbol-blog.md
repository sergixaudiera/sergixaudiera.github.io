---
layout: page
title: Futbol Blog
description: Futbol Blog Archive
permalink: /blog/futbol/
---
<aside>futbol blog (2012 - 2013)</aside>
Experimento inspirado en el libro de Eduardo Galeano *Fútbol a Sol y sombra*.
<ul>
  {% for post in site.categories.futbol %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> <date>({{ post.date | date:"%B %Y" }})</date>
    </li>
  {% endfor %}
</ul>