---
layout: page
permalink: /blog/
title: Blog
description: Step-by-step tutorials on Python, machine learning and more.
nav: true
nav_order: 5
---

<style>
  .bl-chips { display: flex; flex-wrap: wrap; gap: .5rem; margin: 1.2rem 0 2rem; }
  .bl-chip { padding: .3rem .9rem; border: 1px solid var(--global-divider-color); border-radius: 999px; font-size: .9rem; color: var(--global-text-color); text-decoration: none; }
  .bl-chip:hover { border-color: var(--global-theme-color); color: var(--global-theme-color); text-decoration: none; }
  .bl-chip small { color: var(--global-text-color-light); margin-left: .25rem; }
  .bl-topic { margin: 2.4rem 0 2.6rem; scroll-margin-top: 5rem; }
  .bl-topic h2 { font-size: 1.6rem; margin-bottom: 1.1rem; padding-bottom: .4rem; border-bottom: 1px solid var(--global-divider-color); }
  .bl-steps { display: flex; flex-direction: column; gap: .8rem; }
  a.bl-step-card { display: flex; gap: 1.1rem; align-items: flex-start; padding: 1rem 1.2rem; border: 1px solid var(--global-divider-color); border-radius: 8px; background-color: var(--global-card-bg-color); color: var(--global-text-color); text-decoration: none; transition: border-color .25s ease, transform .25s ease; }
  a.bl-step-card:hover { border-color: var(--global-theme-color); transform: translateX(4px); text-decoration: none; }
  .bl-num { flex: 0 0 auto; width: 2.2rem; height: 2.2rem; display: flex; align-items: center; justify-content: center; border: 1px solid var(--global-theme-color); border-radius: 50%; font-weight: 600; color: var(--global-theme-color); }
  .bl-title { margin: 0 0 .25rem; font-size: 1.15rem; color: var(--global-theme-color); }
  .bl-desc { margin: 0 0 .4rem; font-size: .95rem; line-height: 1.45; }
  .bl-meta { margin: 0; font-size: .82rem; color: var(--global-text-color-light); }
</style>

{% comment %}
  HOW THIS PAGE WORKS
  1. Edit `topic_order` to choose the sections and their order. Format: tag:Display name
  2. In each post, add the tag in front matter (tags: python) and a number (step: 1).
  3. Inside a section, posts are sorted by `step`, so the tutorial reads in order.
  4. A post with several tags appears in each of those sections.
  5. Tags that are not listed below still get their own section at the end, so no post is hidden.
{% endcomment %}
{% assign topic_order = "python:Python|ml:Machine Learning|dl:Deep Learning|nlp:NLP|cv:Computer Vision" | split: "|" %}
{% assign topics = topic_order %}
{% assign listed = "" | split: "" %}
{% for entry in topic_order %}{% assign p = entry | split: ":" %}{% assign listed = listed | push: p[0] %}{% endfor %}
{% for tag_pair in site.tags %}{% assign t = tag_pair[0] %}{% unless listed contains t %}{% capture extra_entry %}{{ t }}:{{ t }}{% endcapture %}{% assign topics = topics | push: extra_entry %}{% endunless %}{% endfor %}

<div class="bl-page">

<div class="bl-chips">
{% for entry in topics %}
{% assign parts = entry | split: ":" %}
{% assign tag = parts[0] %}
{% assign count = site.posts | where_exp: "p", "p.tags contains tag" | size %}
{% if count > 0 %}
  <a class="bl-chip" href="#topic-{{ tag | slugify }}">{{ parts[1] }}<small>{{ count }}</small></a>
{% endif %}
{% endfor %}
</div>

{% for entry in topics %}
{% assign parts = entry | split: ":" %}
{% assign tag = parts[0] %}
{% assign items = site.posts | where_exp: "p", "p.tags contains tag" | sort: "step" %}
{% if items.size > 0 %}
<section class="bl-topic" id="topic-{{ tag | slugify }}">
  <h2>{{ parts[1] }}</h2>
  <div class="bl-steps">
  {% for post in items %}
    {% assign read_time = post.content | number_of_words | divided_by: 180 | plus: 1 %}
    <a class="bl-step-card" href="{{ post.url | relative_url }}">
      {% if post.step %}<span class="bl-num">{{ post.step }}</span>{% endif %}
      <div>
        <h3 class="bl-title">{{ post.title }}</h3>
        {% if post.description %}<p class="bl-desc">{{ post.description }}</p>{% endif %}
        <p class="bl-meta">{{ read_time }} min read &nbsp;&middot;&nbsp; {{ post.date | date: "%B %d, %Y" }}</p>
      </div>
    </a>
  {% endfor %}
  </div>
</section>
{% endif %}
{% endfor %}

</div>
