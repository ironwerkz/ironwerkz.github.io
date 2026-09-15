---
layout: page
title: / Articles
permalink: /articles/
---

<ul class="articles-list">
{% for post in site.posts %}
  <li>
    <span class="articles-meta">{{ articles.date | date: "%b %-d, %Y" }}</span>
    <h3><a href="{{ articles.url | relative_url }}">{{ articles.title }}</a></h3>
  </li>
{% endfor %}
</ul>