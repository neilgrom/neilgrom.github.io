---
layout: page
title: Blog Archive
---

<h1>Blog Archive</h1>
<p>Sort by tag</p>

{% assign all_tags = "" %}

{% for post in site.posts %}
  {% for tag in post.tags %}
    {% unless all_tags contains tag %}
      {% assign all_tags = all_tags | append: "," | append: tag %}
    {% endunless %}
  {% endfor %}
{% endfor %}

{% assign tag_list = all_tags | split: "," | uniq | sort %}

{% for tag in tag_list %}
  {% if tag != "" %}
    <h2>{{ tag }}</h2>
    <ul>
      {% for post in site.posts %}
        {% if post.tags contains tag %}
          <li><a href="{{ post.url }}">{{ post.date | date: "%b %d, %Y" }} - {{ post.title }}</a></li>
        {% endif %}
      {% endfor %}
    </ul>
  {% endif %}
{% endfor %}
