---
layout: page
permalink: /people/
title: People
description: 
nav: true
nav_order: 7
---

<div class="row row-cols-1 row-cols-md-3 g-4">
  {% for person in site.people %}
  <div class="col">
    <div class="card h-100 hoverable">
      <a href="{{ person.url | relative_url }}">
        <img src="{{ person.image | relative_url }}" class="card-img-top" alt="{{ person.title }}" style="object-fit: cover; height: 250px;">
      </a>
      <div class="card-body text-center">
        <h5 class="card-title">
          <a href="{{ person.url | relative_url }}" style="color: inherit; text-decoration: none;">{{ person.title }}</a>
        </h5>
        <p class="card-text">{{ person.role }}</p>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
