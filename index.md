---
layout: default
title: "Seminar Series"
---

# Upcoming Seminars

A new academic year is about to begin, and we are restarting our Imaging Seminar Series.
This seminar is part of the IMAGINE+ and Cosimo networks.
This series is dedicated to exploring cutting-edge developments in imaging, image processing, inverse problems, and their applications. Our intent is to facilitate communication between users and developers of image analysis tools.
As an upgrade from previous iterations of the seminar, we are happy to announce that lunch will be provided after the seminar.

<ul>
{% assign today = site.time | date: "%Y-%m-%d" %}
{% for post in site.posts %}
  {% if post.date > today %}
    <li>
      <strong>{{ post.date | date: "%B %d, %Y" }}</strong>:
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>

# Past Seminars

<ul>
{% for post in site.posts %}
  {% if post.date <= today %}
    <li>
      <strong>{{ post.date | date: "%B %d, %Y" }}</strong>:
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>




