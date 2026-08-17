---
layout: default
title: "Ramesh Pandya"
lang: en
permalink: /en/authors/ramesh/
---

<div style="display: flex; align-items: center; margin-bottom: 2rem;">
  <img src="{{ site.baseurl }}/assets/images/authors/ramesh.jpg" alt="Ramesh Pandya" style="width: 120px; height: 120px; border-radius: 50%; margin-right: 2rem; object-fit: cover;">
  <div>
    <h1 style="margin: 0 0 0.5rem 0;">Ramesh Pandya</h1>
    <p style="font-size: 1.1rem; color: #606c71; margin: 0;">Rose grower from Morbi and member of the Gujarat Rose Society. He has been growing roses for several decades — ordering plants from KSG by sending a bank draft, back before the telephone made it easy. </p>
  </div>
</div>

---

## Articles by Ramesh

{% assign lang_posts = site.posts | where: "lang", "en" %}
{% assign sole_posts = lang_posts | where: "post_author", "ramesh" %}
{% assign co_posts = lang_posts | where: "post_authors", "ramesh" %}
{% assign author_posts = sole_posts | concat: co_posts | sort: "date" | reverse %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← Back to Articles]({{ site.baseurl }}/en/)
