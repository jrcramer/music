---
layout: page
---

# Works that are published

<ul class="entries">
  {% for post in site.posts %}
    {% assign b_published = false %}
    {% for tag in post.tags %}
      {% if tag == 'pub' %}{% assign b_published = true %}{% endif %}
    {% endfor %}
  {% if b_published %}
  <li>
    <a href="/music{{ post.url }}">
      {{ post.title }}
    </a>
  </li>
  {% endif %}
  {% endfor %}
</ul>