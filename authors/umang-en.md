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
    <p style="font-size: 1.1rem; color: #606c71; margin: 0;">Rose enthusiast and founding member of Gujarat Rose Society. Passionate about sharing scientific and data-driven approaches to rose cultivation.</p>
  </div>
</div>

Umang specializes in nutrition, fertilizer calculations, and translating scientific principles into practical solutions for Gujarat's unique challenges.

---

## Articles by Umang

{% assign author_posts = site.posts | where: "author", "umang" | where: "lang", "en" %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← Back to Articles]({{ site.baseurl }}/en/)
