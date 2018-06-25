---
layout: default
title: Blog - Morgan Gillis
permalink: /blog/
---

{% for post in site.posts %}
<h4 style="display:inline;"><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></h4> <span style="display:inline;">{{ post.date | date_to_string }}</span>
{% endfor %}

{% for post in site.posts %}
<div style="display:flex; justify-content:space-between; align-items:baseline;">
  <h4><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></h4>
  <span>{{ post.date | date_to_string }}</span>
</div>
{% endfor %}
