---
title: 장기 게임 개발기
permalink: /janggi/
---

## 장기 글 목록

{% assign posts = site.categories.janggi | sort: "date" | reverse %}
{% for post in posts %}
- [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}
