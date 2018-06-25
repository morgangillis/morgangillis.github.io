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
<h4><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></h4><span>{{ post.date | date_to_string }}</span>
{% endfor %}
