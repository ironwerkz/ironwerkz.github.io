---
title: / ironwerkz Blog
layout: home
permalink: /
---

{% comment %}
the homepage will display the most current article by date
{% endcomment %}

{% assign latest = site.posts.first %}

## Latest Article

### [{{ latest.title }}]({{ latest.url | relative_url }})
<span class="articles-meta">{{ latest.date | date: "%b %-d, %Y" }}</span>


[See all Articles →](/articles/)