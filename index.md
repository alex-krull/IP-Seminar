---
layout: default
title: "Seminar Series"
---

{% assign today = site.time %}

# Upcoming Seminars

<ul>
{% assign upcoming = site.posts | sort: "eventdate" %}
{% for post in upcoming %}
  {% if post.eventdate > today %}
    <li>
      <strong>{{ post.eventdate | date: "%B %d, %Y" }}</strong>:
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>

# Past Seminars

<ul>
{% assign past = site.posts | sort: "eventdate" | reverse %}
{% for post in past %}
  {% if post.eventdate <= today %}
    <li>
      <strong>{{ post.eventdate | date: "%B %d, %Y" }}</strong>:
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>
