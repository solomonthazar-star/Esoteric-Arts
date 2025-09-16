---
layout: page
title: Authors
permalink: /authors/
---

# Meet Our Authors

<div class="authors-grid">
{% for author in site.data.authors %}
  <div class="author-card">
    <h2>{{ author.name }}</h2>
    <ul>
      {% for work in author.works %}
        <li><a href="{{ work.link }}" target="_blank">{{ work.title }}</a></li>
      {% endfor %}
    </ul>
  </div>
{% endfor %}
</div>
