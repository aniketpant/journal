---
layout: base
title: Home
slug: home
---
### Recent writings

<ul class="list">
{% for post in site.posts %}
<li>
<a href="{{ post.url }}">{{ post.title }}</a>
</li>
{% endfor %}
</ul>