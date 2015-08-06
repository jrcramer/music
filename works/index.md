---
layout: page
title: Works
permalink: /works/
---

<ul class="entries">
  {% for post in site.posts %}
  {% if post.layout == "work" %}
  <li>
    <a href="/music{{ post.url }}">
      {{ post.title }}
    </a>
  </li>
  {% endif %}
  {% endfor %}
</ul>

Works that are [performed](perf.html) or [published](pub.html)