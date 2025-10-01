---
layout: default
title: "Seminar Series"
---

{% assign today = site.time %}

# Upcoming Seminars

<ul>
  {% assign upcoming = site.posts | sort: "date" %}
  {% for post in upcoming %}
    {% if post.date > today %}
      <li>
        <strong>{{ post.date | date: "%B %d, %Y" }}</strong>:
        {{ site.baseurl }}{{ post.url }}{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

# Past Seminars

<ul>
  {% assign past = site.posts | sort: "date" | reverse %}
  {% for post in past %}
    {% if post.date <= today %}
      <li>
        <strong>{{ post.date | date: "%B %d, %Y" }}</strong>:
        {{ site.baseurl }}{{ post.url }}{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
