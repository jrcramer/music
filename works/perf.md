---
layout: page
---

# Works that are performed

<ul class="entries">
  {% for post in site.posts %}
    {% assign b_performed = false %}
    {% for tag in post.tags %}
      {% if tag == 'perf' %}{% assign b_performed = true %}{% endif %}
    {% endfor %}
  {% if b_performed %}
  <li>
    <a href="/music{{ post.url }}">
      {{ post.title }}
    </a>
  </li>
  {% endif %}
  {% endfor %}
</ul>

All [works](index.html) or works that are [published](pub.html)