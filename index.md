---
layout: default
title: Home
---

## 文章列表

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small>（{{ post.date | date: "%Y-%m-%d" }}）</small>
  </li>
{% endfor %}
</ul>
