---
layout: default
title: "Seminar Series"
---

# All Seminars

<ul>
{% assign all_posts = site.posts | sort: "date" | reverse %}
{% for post in all_posts %}
  <li>
    <strong>{{ post.date | date: "%B %d, %Y" }}</strong>:
    <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
