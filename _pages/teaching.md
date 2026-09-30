---
layout: page
permalink: /teaching/
title: teaching
description: Course materials, schedules, and resources for classes taught.
nav: true
nav_order: 6
---

<style>
  .tc-section { margin: 2.2rem 0 2.5rem; }
  .tc-section h2 { font-size: 1.6rem; margin-bottom: 1.1rem; padding-bottom: .4rem; border-bottom: 1px solid var(--global-divider-color); }
  .tc-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 1.1rem; }
  a.tc-card { display: flex; flex-direction: column; padding: 1.3rem 1.4rem; border: 1px solid var(--global-divider-color); border-radius: 8px; background-color: var(--global-card-bg-color); color: var(--global-text-color); text-decoration: none; transition: border-color .25s ease, transform .25s ease, box-shadow .25s ease; }
  a.tc-card:hover { border-color: var(--global-theme-color); transform: translateY(-4px); box-shadow: 0 10px 25px rgba(0, 0, 0, .12); text-decoration: none; }
  .tc-title { margin: 0 0 .5rem; font-size: 1.35rem; color: var(--global-theme-color); }
  .tc-meta { display: flex; flex-wrap: wrap; gap: .3rem 1.1rem; margin-bottom: .8rem; font-size: .9rem; color: var(--global-text-color-light); }
  .tc-desc { margin: 0; font-size: .95rem; line-height: 1.5; }
</style>

{% comment %}
  Edit this list to change the order or names of the categories.
  Each course file in _teachings/ needs a matching `category:` line in its front matter.
  Categories with no courses are hidden automatically.
{% endcomment %}
{% assign category_order = "Prerequisites|Data Science|Computer Vision|NLP" | split: "|" %}
{% assign present = site.teachings | map: "category" | compact | uniq %}
{% assign extra = "" | split: "" %}
{% for c in present %}{% unless category_order contains c %}{% assign extra = extra | push: c %}{% endunless %}{% endfor %}
{% assign category_list = category_order | concat: extra | push: "Uncategorized" %}

<div class="tc-page">
{% for category in category_list %}
{% if category == "Uncategorized" %}
{% assign items = site.teachings | where_exp: "c", "c.category == nil" %}
{% else %}
{% assign items = site.teachings | where: "category", category %}
{% endif %}
{% if items.size > 0 %}
<section class="tc-section">
  <h2>{{ category }}</h2>
  <div class="tc-grid">
  {% for course in items %}
    <a class="tc-card" href="{{ course.url | relative_url }}">
      <h3 class="tc-title">{{ course.title }}</h3>
      <div class="tc-meta">
        {% if course.term %}<span>{{ course.term }}</span>{% endif %}
        {% if course.instructor %}<span>{{ course.instructor }}</span>{% endif %}
      </div>
      <p class="tc-desc">{{ course.description }}</p>
    </a>
  {% endfor %}
  </div>
</section>
{% endif %}
{% endfor %}
</div>
