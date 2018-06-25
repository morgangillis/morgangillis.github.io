---
layout: default
title: Blog - Morgan Gillis
permalink: /blog/
---

{% for post in site.posts %}
<h4><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></h4><p style="display:inline"><span>{{ post.date | date_to_string }}</span></p>
{% endfor %}
