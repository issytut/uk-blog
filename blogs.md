---
layout: page
title: Blogs
permalink: /blogs/
---

Welcome to my blog posts!

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="meta">{{ post.date | date_to_string }}</p>
    {{ post.excerpt }}
  </article>
{% endfor %}
