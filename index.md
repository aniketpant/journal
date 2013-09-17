---
layout: base
title: Home
slug: home
---
<ul class="nav nav--stacked list">
{% for post in site.posts %}
<li>
<a href="{{ post.url }}" class="link {% if forloop.index == 1 %}highlite{% endif %}">
  <date class="date milli muted">{{ post.date | date_to_long_string }}</date>
  <span class="title">{{ post.title }}</span>
</a>
</li>
{% endfor %}
</ul>
