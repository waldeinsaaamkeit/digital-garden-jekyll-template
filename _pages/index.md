---
layout: page
title: Home
id: home
permalink: /
---




<div class="grid-element">
      <h2>Blog posts</h2>
      {% assign post_limit = 7 %}
      {% for post in site.posts limit: post_limit %}
      <div class="list-entry">
        <div><a class="internal-link" href="{{ post.url }}">{{ post.title }}</a> <span class="faded">({{ post.date | date: "%Y-%m-%d" }})</span></div>
        <div>{{ post.excerpt }}</div>
      </div>
      {% endfor %}
      <p>
        <a class="internal-link" href="/blog">I wrote {{ site.posts.size | post_limit }} more posts</a>.
      </p>
    </div>
<div class="grid-element">
      <h2>Digital Garden</h2>
- [[Cărți]]
- [[Filme]]
- [[Writing]]
- [[Fotografie]]
    </div>
<style>
  .wrapper {
    max-width: 46em;
  }
</style>
