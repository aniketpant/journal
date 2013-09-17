---
layout: base
title: Home
slug: home
---
<ul class="nav nav--stacked list">
{% for post in site.posts %}
{% if forloop.index == 1 or forloop.index == 2 or forloop.index == 3 %}
<li>
<a href="{{ post.url }}" class="link highlite">
  <date class="date milli">{{ post.date | date_to_long_string }}</date>
  <span class="title">{{ post.title }}</span>
  <div class="excerpt">{{ post.content }}</div>
</a>
</li>
{% else %}
<li>
<a href="{{ post.url }}" class="link">
  <date class="date milli">{{ post.date | date_to_long_string }}</date>
  <span class="title">{{ post.title }}</span>
</a>
</li>
{% endif %}
{% endfor %}
</ul>
