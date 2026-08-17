---
layout: default
title: "Umang Bhatt"
lang: en
permalink: /en/authors/umang/
---

<div style="display: flex; align-items: center; margin-bottom: 2rem;">
  <img src="{{ site.baseurl }}/assets/images/authors/umang.jpg" alt="Umang Bhatt" style="width: 120px; height: 120px; border-radius: 50%; margin-right: 2rem; object-fit: cover;">
  <div>
    <h1 style="margin: 0 0 0.5rem 0;">Umang Bhatt</h1>
    <p style="font-size: 1.1rem; color: #606c71; margin: 0;">Rose enthusiast. </p>
  </div>
</div>

---

## Articles by Umang

{% assign lang_posts = site.posts | where: "lang", "en" %}
{% assign sole_posts = lang_posts | where: "post_author", "umang" %}
{% assign co_posts = lang_posts | where: "post_authors", "umang" %}
{% assign author_posts = sole_posts | concat: co_posts | sort: "date" | reverse %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← Back to Articles]({{ site.baseurl }}/en/)
