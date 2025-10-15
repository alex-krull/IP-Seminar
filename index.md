---
layout: default
title: "Seminar Series"
---

{% assign today = site.time | date: "%Y%m%d" %}

# Upcoming Seminars

<ul>
{% assign sorted_posts = site.posts | sort: "date" %}
{% for post in sorted_posts %}
  {% assign post_date = post.date | date: "%Y%m%d" %}
  {% if post_date > today %}
    <li>
      <strong>{{ post.date | date: "%B %d, %Y" }}</strong>:
      {% if post.has_link %}
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      {% else %}
        {{ post.title }}
      {% endif %}
    </li>
  {% endif %}
{% endfor %}
</ul>

# Past Seminars

<ul>
{% assign sorted_posts = site.posts | sort: "date" | reverse %}
{% for post in sorted_posts %}
  {% assign post_date = post.date | date: "%Y%m%d" %}
  {% if post_date <= today %}
    <li>
      <strong>{{ post.date | date: "%B %d, %Y" }}</strong>:
      {% if post.has_link %}
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      {% else %}
        {{ post.title }}
      {% endif %}
    </li>
  {% endif %}
{% endfor %}
</ul>
