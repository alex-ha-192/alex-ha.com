---
layout: page
title: "Portfolio"
permalink: /portfolio/
---

<h1>{{ page.title }}</h1>

<ul>
  {% for post in site.categories.portfolio %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>({{ post.date | date: "%d %B %Y" }})</small>
    </li>
  {% endfor %}
</ul>
