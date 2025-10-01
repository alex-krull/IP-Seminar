---
layout: default
title: "Seminar Series"
---

# Upcoming Seminars

<ul>
{% assign today = site.date %}
{% assign upcoming = site.posts | where_exp: "post", "post.eventdate > today" | sort: "date" %}
{% for post in upcoming %}
  <li>
    <strong>{{ post.eventdate | date: "%B %d, %Y" }}</strong>:
    <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

# Past Seminars

<ul>
{% assign past = site.posts | where_exp: "post", "post.eventdate <= today" | sort: "date" | reverse %}
{% for post in past %}
  <li>
    <strong>{{ post.eventdate | date: "%B %d, %Y" }}</strong>:
    <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
