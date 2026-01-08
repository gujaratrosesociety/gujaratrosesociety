---
layout: default
title: "ઉમંગ ભટ્ટ"
lang: gu
permalink: /authors/umang/
---

<div style="display: flex; align-items: center; margin-bottom: 2rem;">
  <img src="{{ site.baseurl }}/assets/images/authors/umang.jpg" alt="ઉમંગ ભટ્ટ" style="width: 120px; height: 120px; border-radius: 50%; margin-right: 2rem; object-fit: cover;">
  <div>
    <h1 style="margin: 0 0 0.5rem 0;">ઉમંગ ભટ્ટ</h1>
    <p style="font-size: 1.1rem; color: #606c71; margin: 0;">ગુલાબ પ્રેમી અને ગુજરાત રોઝ સોસાયટીના સભ્ય. </p>
  </div>
</div>

---

## ઉમંગ દ્વારા લેખો

{% assign author_posts = site.posts | where: "author", "umang" | where: "lang", "gu" %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← લેખો પર પાછા જાઓ]({{ site.baseurl }}/)
