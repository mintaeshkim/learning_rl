---
layout: default
title: Categories
permalink: /categories/
---

# 📚 Categories

Browse blog posts by category.

<ul>
  {% assign sorted_categories = site.categories | sort %}
  {% for category in sorted_categories %}
    <li>
      <a href="#{{ category[0] | slugify }}">
        {{ category[0] }} ({{ category[1].size }})
      </a>
    </li>
  {% endfor %}
</ul>

---

{% for category in sorted_categories %}
  <h2 id="{{ category[0] | slugify }}">{{ category[0] }}</h2>
  <ul>
    {% for post in category[1] %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <small>({{ post.date | date: "%Y-%m-%d" }})</small>
      </li>
    {% endfor %}
  </ul>
{% endfor %}
