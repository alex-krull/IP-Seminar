---
layout: default
title: "All Seminars"
---

# All Seminars

{% assign curDate = site.time | date: '%s' %}
{% for post in site.posts %}
    {% assign postStartDate = post.date | date: '%s' %}
    {% if postStartDate >= curDate %}
        Post datas here
    {% endif %}
{% endfor %}
