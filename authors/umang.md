---
layout: default
title: "ઉમંગ ભટ્ટ"
lang: gu
permalink: /authors/umang/
---

# ઉમંગ ભટ્ટ

ગુલાબ પ્રેમી અને ગુજરાત રોઝ સોસાયટીના સ્થાપક સભ્ય. ગુજરાતની આબોહવામાં ગુલાબની ખેતી માટે વૈજ્ઞાનિક અને ડેટા-આધારિત અભિગમો શેર કરવા માટે ઉત્સાહી.

ઉમંગ પોષણ, ખાતર ગણતરીઓ, અને ગુજરાતની અનન્ય પડકારો માટે વૈજ્ઞાનિક સિદ્ધાંતોને વ્યવહારુ ઉકેલોમાં અનુવાદિત કરવામાં વિશેષતા ધરાવે છે.

---

## ઉમંગ દ્વારા લેખો

{% assign author_posts = site.posts | where: "author", "umang" | where: "lang", "gu" %}
{% for post in author_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

[← લેખો પર પાછા જાઓ]({{ site.baseurl }}/)
