---
layout: default
---
<header>
	<h1>Hi, my name is <a href="/">Sergi Xaudiera</a>.</h1>
	<aside>I'm a PhD candidate interested in internet</aside>
</header>

~

**What I do**  
I do Computational Social Science research in the context of internet, especially on social media and how they can make a positive impact for society.

~

**Get in touch**  
If you want to get in touch easily just [send me an e-mail](mailto:sergi@xaudiera.xyz). You cana also [follow me on Twitter](http://twitter.com/SergiXaudiera){:rel="nofollow"}, recieve my reads [on Telegram](https://t.me/readingx){:rel="nofollow"} and subscribe to my loved [rss feed](https://sergi.xaudiera.xyz/feed.xml).

~

**Things I’ve written:**
<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> 
    </li>
  {% endfor %}
</ul>