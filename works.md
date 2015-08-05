---
layout: page
title: Works
permalink: /works/
---
 
<ul class="entries">
  {% for post in site.posts %}
    {{ post.layout post.title }}
  {% if post.tag == "work" %}
  <li>
    <a href="{{ post.url }}">
      <h3>{{ post.title }}</h3>
    </a>
  </li>
  {% endif %}
  {% endfor %}
</ul>
