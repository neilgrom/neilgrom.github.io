---
layout: page
---

<h1>Blog Archive</h1>

{% if site.posts %}
  <ul>
    {% for post in site.posts %}
      <li><a href="{{ post.url }}">{{ post.date | date: "%B %d, %Y" }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% else %}
  <p>No posts found.</p>
{% endif %}
