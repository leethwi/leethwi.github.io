---
layout: page
title: Categories
permalink: /categories/
---

{% assign sorted_categories = site.categories | sort %}

{% for category in sorted_categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li>
        <span style="color:#777">{{ post.date | date: "%Y-%m-%d" }}</span>
        — <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
{% endfor %}
