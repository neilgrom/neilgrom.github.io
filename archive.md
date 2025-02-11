---
layout: page
title: Blog Archive
---

{% if site.tags %}
  {% assign sorted_tags = site.tags | sort %}
  {% for tag in sorted_tags %}
    <h3>{{ tag[0] }}</h3>
    <ul>
      {% for post in tag[1] %}
        <li><a href="{{ post.url }}">{{ post.date | date: "%B %d, %Y" }} - {{ post.title }}</a></li>
      {% endfor %}
    </ul>
  {% endfor %}
{% else %}
  <p>No posts found.</p>
{% endif %}
