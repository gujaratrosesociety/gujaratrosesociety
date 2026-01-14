---
layout: default
title: "કૃણાલ"
lang: gu
permalink: /authors/krunal/
---

<div style="display: flex; align-items: center; margin-bottom: 2rem;">
  <img src="{{ site.baseurl }}/assets/images/authors/krunal.jpg" alt="કૃણાલ" style="width: 120px; height: 120px; border-radius: 50%; margin-right: 2rem; object-fit: cover;">
  <div>
    <h1 style="margin: 0 0 0.5rem 0;">કૃણાલ</h1>
    <p style="font-size: 1.1rem; color: #606c71; margin: 0;">ગુલાબ પ્રેમી.</p>
  </div>
</div>

---

## કૃણાલ દ્વારા લેખો

{% assign author_posts = site.posts | where: "post_author", "krunal" | where: "lang", "gu" %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← લેખો પર પાછા જાઓ]({{ site.baseurl }}/)
