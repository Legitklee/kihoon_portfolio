---
layout: default
title: Projects
permalink: /projects/
---

# 🛠 Projects

<ul class="project-list">
  {% for post in site.posts %}
    {% if post.tags contains "project" %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span> — {{ post.date | date: "%b %-d, %Y" }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>
