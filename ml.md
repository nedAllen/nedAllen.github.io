---
title: ML 노트
permalink: /ml/
---

## 글 목록

{% assign posts = site.categories.ml | sort: "date" | reverse %}
{% for post in posts %}
- [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}
