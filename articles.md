---
layout: page
title: / Articles
permalink: /articles/
---

{% comment %}
Repository of past Articles

for personal reference
https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one
^using this plugin for markdown articles
{% endcomment %}

<ul class="articles-list">
{% for post in site.posts %}
  <li>
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  </li>
{% endfor %}
</ul>