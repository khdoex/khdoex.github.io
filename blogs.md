---
layout: page
title: Blogs
permalink: /blogs/
---

# My Blog Posts

{% for post in site.posts %}
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%B %d, %Y" }}</p>
  <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
{% endfor %}