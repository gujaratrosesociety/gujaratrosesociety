---
layout: default
title: "Jay Patel"
lang: en
permalink: /en/authors/jay/
---

<div style="display: flex; align-items: center; margin-bottom: 2rem;">
  <img src="{{ site.baseurl }}/assets/images/authors/jay.jpg" alt="Jay Patel" style="width: 120px; height: 120px; border-radius: 50%; margin-right: 2rem; object-fit: cover;">
  <div>
    <h1 style="margin: 0 0 0.5rem 0;">Jay Patel</h1>
    <p style="font-size: 1.1rem; color: #606c71; margin: 0;">Experienced rose grower specializing in variety selection and cultivation techniques for Gujarat's unique weather conditions.</p>
  </div>
</div>

With years of hands-on experience, Jay excels at identifying varieties that perform best in our climate and sharing practical growing advice.

---

## Articles by Jay

{% assign author_posts = site.posts | where: "author", "jay" | where: "lang", "en" %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← Back to Articles]({{ site.baseurl }}/en/)
