---
layout: default
title: "Umang Bhatt"
lang: en
permalink: /en/authors/umang/
---

# Umang Bhatt

Rose enthusiast and founding member of Gujarat Rose Society. Passionate about sharing scientific and data-driven approaches to rose cultivation in Gujarat's climate.

Umang specializes in nutrition, fertilizer calculations, and translating scientific principles into practical solutions for Gujarat's unique challenges.

---

## Articles by Umang

{% assign author_posts = site.posts | where: "author", "umang" | where: "lang", "en" %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← Back to Articles]({{ site.baseurl }}/en/)
