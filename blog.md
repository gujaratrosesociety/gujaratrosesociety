---
layout: default
title: Blog
---

# Blog

Explore our journey, discoveries, and innovations in rose cultivation.

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
      <div class="date">{{ post.date | date: "%B %d, %Y" }}</div>
      <div class="entry">
        {{ post.excerpt }}
      </div>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
