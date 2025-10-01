---
layout: default
title: "Seminar Series"
---

# Upcoming Seminars

<ul>
  {% for post in site.posts %}
    <li>
      <strong>{{ post.date | date: "%B %d, %Y" }}</strong>:
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
