---
title: "장기 게임 개발기"
permalink: /janggi/
---

## 장기 글 목록

{% raw %}
{% assign posts = site.categories.janggi | sort: "date" | reverse %}
{% for post in posts %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
{% endraw %}
