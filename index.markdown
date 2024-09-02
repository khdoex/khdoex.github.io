---
layout: home
title: Home
---

# Welcome to Kaan Hacıhaliloğlu's Portfolio

I'm a Data Scientist based in Istanbul, passionate about machine learning, data analysis, and deep learning. With a background in Physics.


## Recent Blog Posts

{% for post in site.posts limit:3 %}
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
{% endfor %}

[View all posts](/blogs)