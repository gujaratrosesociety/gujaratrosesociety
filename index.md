---
layout: default
title: Gujarat Rose Society
---

# Gujarat Rose Society

A community of rose enthusiasts sharing knowledge, tools, and insights for rose cultivation in Gujarat.

---

## Articles & Insights

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
      <div class="date">{{ post.date | date: "%B %d, %Y" }}</div>
      <div class="entry">
        {{ post.excerpt }}
      </div>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More →</a>
    </article>
    <hr>
  {% endfor %}
</div>

---

## About Us

The Gujarat Rose Society is a dedicated community of rose enthusiasts, gardeners, and horticulturists who share a passion for cultivating beautiful roses in Gujarat's unique climate. We develop innovative tools, share best practices, and support each other in growing beautiful roses.
