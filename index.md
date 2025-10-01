---
layout: default
title: "Seminar Series"
---

# Upcoming Seminars

<ul>
{% assign today = site.time %}
{% assign upcoming = site.posts | where_exp: "post", "post.date > today" | sort: "date" | reverse %}
{% for post in upcoming %}
  <li>
    <strong>{{ post.date | date: "%B %d, %Y" }}</strong>:
    <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

# Past Seminars

<ul>
{% assign past = site.posts | where_exp: "post", "post.date <= today" | sort: "date" | reverse %}
{% for post in past %}
  <li>
    <strong>{{ post.date | date: "%B %d, %Y" }}</strong>:
    <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
