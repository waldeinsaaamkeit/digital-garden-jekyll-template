---
layout: default
title: Blog archives
permalink: /blog
---

<div>
  <div class="post-heading">
    <h1 class="post-title">Toate articolele</h1>
  </div>
  {% for post in site.posts limit: post_limit %}
  <div class="list-entry">
    <div><a class="internal-link" href="{{ post.url }}">{{ post.title }}</a> <span class="faded">({{ post.date | date: "%Y-%m-%d" }})</span></div>
    <div>{{ post.excerpt }}</div>
  </div>
  {% endfor %}
  <br>
</div>
