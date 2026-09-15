---
layout: page
title: / Articles
permalink: /articles/
---

{% comment %}
Repository of past Articles
{% endcomment %}

<ul class="articles-list">
{% for posts in site.posts %}
  <li>
    <span class="articles-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
    <h3><a href="{{ posts.url | relative_url }}">{{ post.title }}</a></h3>
  </li>
{% endfor %}
</ul>