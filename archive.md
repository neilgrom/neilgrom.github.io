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
    <h2 style="margin-top: 30px; font-size: 24px; font-weight: bold;">{{ tag }}</h2>

    <ul style="margin-bottom: 20px; padding-left: 20px;">
      {% for post in site.posts %}
        {% if post.tags contains tag %}
          <li style="margin-bottom: 10px;">
            <a href="{{ post.url | relative_url }}" style="font-size: 18px; text-decoration: none; color: #007bff;">
              {{ post.date | date: "%b %d, %Y" }} - {{ post.title }}
            </a>
          </li>
        {% endif %}
      {% endfor %}
    </ul>
  {% endif %}
{% endfor %}
