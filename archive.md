---
layout: page
title: Blog Archive
---

<h1>Blog Archive</h1>

<ul>
  {% for post in site.posts %}
    <li><a href="{{ post.url }}">{{ post.date | date: "%B %d, %Y" }} - {{ post.title }}</a></li>
  {% endfor %}
</ul>
