---
layout: base
title: Home
slug: home
---
<ul class="nav nav--stacked list">
{% for post in site.posts %}
<li>
<a href="{{ post.url }}">
  <date class="date milli">{{ post.date | date_to_long_string }}</date>
  <span class="title">{{ post.title }}</span>
</a>
</li>
{% endfor %}
</ul>