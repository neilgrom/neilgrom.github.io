---
layout: page
title: Blog Archive
---

<h1>Blog Archive</h1>
<p>Sort by tag</p>

{% assign sorted_tags = site.tags | sort %}

{% for tag in sorted_tags %}
  <h2>{{ tag[0] }}</h2>  <!-- Displays the tag name -->
  <ul>
    {% for post in tag[1] %}
      <li>
        <a href="{{ post.url }}">{{ post.date | date: "%b %Y" }} - {{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
{% endfor %}

<h2>Debugging</h2>
<p>Total tags found: {{ site.tags | size }}</p>
{% for tag in site.tags %}
  <p>Tag: {{ tag[0] }} has {{ tag[1] | size }} posts.</p>
{% endfor %}
