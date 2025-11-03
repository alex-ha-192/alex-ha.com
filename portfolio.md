---
layout: default
title: "Portfolio"
permalink: /portfolio/
---

# {{ page.title }}

{% assign portfolio_posts = site.categories.portfolio | sort: 'date' | reverse %}

{% for post in portfolio_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%d %B %Y" }}
{% endfor %}
