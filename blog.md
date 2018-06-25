---
layout: default
title: Blog - Morgan Gillis
permalink: /blog/
---

<ul class="posts">

  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

{% for post in site.posts %}
<h3><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a><span>{{ post.date | date_to_string }}</span></h3>
{% endfor %}
