---
layout: default
title: "રમેશ પંડ્યા"
lang: gu
permalink: /authors/ramesh/
---

<div style="display: flex; align-items: center; margin-bottom: 2rem;">
  <img src="{{ site.baseurl }}/assets/images/authors/ramesh.jpg" alt="રમેશ પંડ્યા" style="width: 120px; height: 120px; border-radius: 50%; margin-right: 2rem; object-fit: cover;">
  <div>
    <h1 style="margin: 0 0 0.5rem 0;">રમેશ પંડ્યા</h1>
    <p style="font-size: 1.1rem; color: #606c71; margin: 0;">મોરબીના ગુલાબ ઉગાડનાર અને ગુજરાત રોઝ સોસાયટીના સભ્ય. અનેક દાયકાઓથી ગુલાબ ઉગાડે છે — ફોન નહોતા એ જમાનામાં ડ્રાફ્ટ મોકલીને KSG પાસેથી છોડ મંગાવતા. </p>
  </div>
</div>

---

## રમેશ દ્વારા લેખો

{% assign author_posts = site.posts | where: "lang", "gu" | where_exp: "post", "post.post_author == 'ramesh' or post.post_authors contains 'ramesh'" %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← લેખો પર પાછા જાઓ]({{ site.baseurl }}/)
