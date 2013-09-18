---
layout: base
title: Home
slug: home
---
<ul class="block-list list">
{% for post in site.posts %}
<li>
<a href="{{ post.url }}" class="block-list__link link">
  <date class="date milli muted">{{ post.date | date_to_long_string }}</date>
  <span class="title">{{ post.title }}</span>
</a>
</li>
{% endfor %}
</ul>
