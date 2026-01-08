---
layout: default
title: "જય પટેલ"
lang: gu
permalink: /authors/jay/
---

<div style="display: flex; align-items: center; margin-bottom: 2rem;">
  <img src="{{ site.baseurl }}/assets/images/authors/jay.jpg" alt="જય પટેલ" style="width: 120px; height: 120px; border-radius: 50%; margin-right: 2rem; object-fit: cover;">
  <div>
    <h1 style="margin: 0 0 0.5rem 0;">જય પટેલ</h1>
    <p style="font-size: 1.1rem; color: #606c71; margin: 0;">ગુજરાતની અનન્ય હવામાન પરિસ્થિતિઓ માટે જાતની પસંદગી અને ખેતી તકનીકોમાં વિશેષતા ધરાવતા અનુભવી ગુલાબ ઉગાડનાર.</p>
  </div>
</div>

જય વર્ષોના અનુભવ સાથે, આપણા વાતાવરણમાં શ્રેષ્ઠ પ્રદર્શન કરતી જાતો ઓળખવામાં અને વ્યવહારુ ઉગાડવાની સલાહ શેર કરવામાં નિષ્ણાત છે.

---

## જય દ્વારા લેખો

{% assign author_posts = site.posts | where: "author", "jay" | where: "lang", "gu" %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← લેખો પર પાછા જાઓ]({{ site.baseurl }}/)
