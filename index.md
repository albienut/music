---
layout: default
title: Главная
---

<h1>Блог</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%d.%m.%Y" }}
    </li>
  {% endfor %}
</ul>