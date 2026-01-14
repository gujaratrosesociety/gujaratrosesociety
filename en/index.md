---
layout: default
title: Gujarat Rose Society
lang: en
permalink: /en/
---

# Gujarat Rose Society

A community of rose enthusiasts sharing knowledge, tools, and insights for rose cultivation in Gujarat.

---

## Rose Growing Guide

{% for section in site.data.sections %}
{% assign section_posts = site.posts | where: "lang", "en" | where: "section", section.id %}
{% if section_posts.size > 0 %}
<div class="guide-section">
  <h3 class="section-title">{{ section.en.title }}</h3>
  <p class="section-description">{{ section.en.description }}</p>
  <ul class="section-posts">
    {% for post in section_posts %}
    <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</div>
{% endif %}
{% endfor %}

---

## About Us

The Gujarat Rose Society is a dedicated community of rose enthusiasts, gardeners, and horticulturists who share a passion for cultivating beautiful roses in Gujarat's unique climate. We develop innovative tools, share best practices, and support each other in growing beautiful roses.
