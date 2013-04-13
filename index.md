---
layout: base
title: Home
slug: home
---
<section class="grid__item one-whole" markdown="1">
### Recent writings

<ul class="block-list recent-posts">
{% for post in site.posts %}
<li>
<a href="{{ post.url }}" class="block-list__link">
  <span class="highlight gamma">{{ post.title }}</span><br/>
  <span class="muted">Written on <date class="date">{{ post.date | date:"%d %B" }}</date></span>
</a>
</li>
{% endfor %}
</ul>
</section>