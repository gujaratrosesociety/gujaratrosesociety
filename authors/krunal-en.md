---
layout: default
title: "Krunal"
lang: en
permalink: /en/authors/krunal/
---

<div style="display: flex; align-items: center; margin-bottom: 2rem;">
  <img src="{{ site.baseurl }}/assets/images/authors/krunal.jpg" alt="Krunal" style="width: 120px; height: 120px; border-radius: 50%; margin-right: 2rem; object-fit: cover;">
  <div>
    <h1 style="margin: 0 0 0.5rem 0;">Krunal</h1>
    <p style="font-size: 1.1rem; color: #606c71; margin: 0;">Rose enthusiast and member of Gujarat Rose Society.</p>
  </div>
</div>

---

## Articles by Krunal

{% assign author_posts = site.posts | where: "post_author", "krunal" | where: "lang", "en" %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← Back to Articles]({{ site.baseurl }}/en/)
