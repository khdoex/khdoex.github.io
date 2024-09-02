---
layout: home
title: Home
permalink: /home/
---

# Welcome to My Portfolio

I'm a Data Scientist passionate about working on interesting problems and building things.


## Featured Blog Posts

{% for post in site.posts limit:3 %}
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
{% endfor %}

[View all posts](/blogs)