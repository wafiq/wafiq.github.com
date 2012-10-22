---
layout: page
title: Code-block
header: Learning to Code
---

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &mdash; <a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

