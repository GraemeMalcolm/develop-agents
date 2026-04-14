---
layout: default
---

<div class="module-header">
  <h1>{{ site.data.module.title }}</h1>
  <p class="module-level">Level: {{ site.data.module.level }}</p>
  <p class="module-description">{{ site.data.module.description }}</p>
</div>

<ul class="content-list">
<<<<<<< HEAD
{% assign content_pages = site.pages | where_exp: "page", "page.path contains 'content/'" | where_exp: "page", "page.name != 'media.txt'" | where_exp: "page", "page.ext == '.md'" | sort: "path" %}
{% for page in content_pages %}
  {% if page.title %}
  <li class="content-item">
    <h3><a href="{{ page.url | relative_url }}">{{ page.title }}</a></h3>
    <p class="content-duration">Duration: {{ page.duration }} minutes</p>
    <p class="content-description">{{ page.description }}</p>
=======
{% assign content_pages = site.pages | where_exp: "item", "item.path contains 'content/'" | where_exp: "item", "item.path contains '.md'" | sort: "path" %}
{% for item in content_pages %}
  {% if item.title and item.layout == 'content' %}
  <li class="content-item">
    <h3><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h3>
    <p class="content-duration">Duration: {{ item.duration }} minutes</p>
    <p class="content-description">{{ item.description }}</p>
>>>>>>> template/main
  </li>
  {% endif %}
{% endfor %}
</ul>
