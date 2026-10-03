---
layout: page
permalink: /proposals/
title: Proposals
description: Research directions for PhD applications, with a public outline of each proposal. Full proposals are shared privately on request.
nav: true
nav_order: 3
---

<style>
  .pr-intro { margin-bottom: 1.8rem; }
  .pr-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(320px, 1fr)); gap: 1.2rem; align-items: stretch; }
  .pr-card { display: flex; flex-direction: column; padding: 1.4rem 1.5rem; border: 1px solid var(--global-divider-color); border-radius: 10px; background-color: var(--global-card-bg-color); transition: border-color .25s ease, box-shadow .25s ease; }
  .pr-card.featured { grid-column: 1 / -1; }
  .pr-card:hover { border-color: var(--global-theme-color); box-shadow: 0 10px 25px rgba(0, 0, 0, .12); }
  .pr-top { display: flex; justify-content: space-between; align-items: center; gap: .6rem; margin-bottom: .7rem; font-size: .78rem; }
  .pr-theme { padding: .15rem .65rem; border: 1px solid var(--global-theme-color); border-radius: 999px; color: var(--global-theme-color); font-weight: 600; text-transform: uppercase; letter-spacing: .05em; }
  .pr-badge { color: var(--global-text-color-light); }
  .pr-title { margin: 0 0 .7rem; font-size: 1.25rem; line-height: 1.3; }
  .pr-title a { color: var(--global-text-color); text-decoration: none; }
  .pr-title a:hover { color: var(--global-theme-color); }
  .pr-focus { margin: 0 0 .9rem; font-size: .95rem; line-height: 1.5; }
  .pr-methods { display: flex; flex-wrap: wrap; gap: .4rem; margin-bottom: 1.2rem; }
  .pr-method { padding: .1rem .6rem; border: 1px solid var(--global-divider-color); border-radius: 4px; font-size: .78rem; color: var(--global-text-color-light); }
  .pr-actions { display: flex; flex-wrap: wrap; gap: .6rem; margin-top: auto; padding-top: .9rem; border-top: 1px dashed var(--global-divider-color); }
  .pr-btn { display: inline-block; padding: .4rem 1rem; border: 1px solid var(--global-theme-color); border-radius: 4px; color: var(--global-theme-color); font-size: .9rem; font-weight: 500; text-decoration: none; }
  .pr-btn:hover { background: var(--global-theme-color); color: var(--global-bg-color); text-decoration: none; }
  .pr-btn.primary { background: var(--global-theme-color); color: var(--global-bg-color); }
  .pr-btn.primary:hover { opacity: .88; }
  .pr-cta { margin-top: 2.5rem; padding: 1.8rem 1rem; text-align: center; border: 1px solid var(--global-divider-color); border-radius: 10px; }
  .pr-cta h2 { margin: 0 0 .5rem; font-size: 1.4rem; }
  .pr-cta p { margin: 0 auto 1rem; max-width: 36rem; }
</style>

{% comment %}
  Every file in the _proposals/ folder becomes one card here.
  Cards are sorted by the `order` number in each file's front matter.
{% endcomment %}
{% assign items = site.proposals | sort: "order" %}

<div class="pr-intro">
  Each card gives a public outline of a research proposal. Full proposals are shared privately on request and can be adapted to a specific supervisor, group or call.
</div>

<div class="pr-grid">
{% for p in items %}
  <article class="pr-card{% if p.featured %} featured{% endif %}">
    <div class="pr-top">
      <span class="pr-theme">{{ p.theme }}</span>
      {% if p.badge %}<span class="pr-badge">{{ p.badge }}</span>{% endif %}
    </div>
    <h3 class="pr-title"><a href="{{ p.url | relative_url }}">{{ p.title }}</a></h3>
    {% if p.description %}<p class="pr-focus">{{ p.description }}</p>{% endif %}
    {% if p.methods %}
    <div class="pr-methods">{% for m in p.methods %}<span class="pr-method">{{ m }}</span>{% endfor %}</div>
    {% endif %}
    <div class="pr-actions">
      <a class="pr-btn primary" href="{{ p.url | relative_url }}">View outline &rarr;</a>
      <a class="pr-btn" href="mailto:amini75zahra@gmail.com?subject=Research%20proposal%20request%3A%20{{ p.theme | uri_escape }}">Request full proposal</a>
    </div>
  </article>
{% endfor %}
</div>

<div class="pr-cta">
  <h2>Interested in a proposal?</h2>
  <p>Tell me about your group or call, and I will send the version that fits your research direction.</p>
  <a class="pr-btn primary" href="mailto:amini75zahra@gmail.com?subject=Research%20proposal%20request">Request a proposal</a>
</div>
