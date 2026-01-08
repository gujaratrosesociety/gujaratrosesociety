---
layout: default
title: "Jay Patel"
lang: en
permalink: /en/authors/jay/
---

# Jay Patel

---

## Articles by Jay

{% assign author_posts = site.posts | where: "author", "jay" | where: "lang", "en" %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← Back to Articles]({{ site.baseurl }}/en/)
