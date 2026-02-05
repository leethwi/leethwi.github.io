---
layout: page
title: dairy
permalink: /categories/dairy/
---

{% assign posts = site.categories.dairy %}
<ul>
  {% for post in posts %}
    <li>
      {{ post.date | date: "%Y-%m-%d" }}
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
