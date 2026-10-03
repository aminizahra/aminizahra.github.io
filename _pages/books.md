---
layout: page
title: bookshelf
permalink: /books/
nav: false
---

> What an astonishing thing a book is. It's a flat object made from a tree with flexible parts on which are imprinted lots of funny dark squiggles. But one glance at it and you're inside the mind of another person, maybe somebody dead for thousands of years. Across the millennia, an author is speaking clearly and silently inside your head, directly to you. Writing is perhaps the greatest of human inventions, binding together people who never knew each other, citizens of distant epochs. Books break the shackles of time. A book is proof that humans are capable of working magic.
>
> -- Carl Sagan, Cosmos, Part 11: The Persistence of Memory (1980)

<br>

## Books that I am reading, have read, or will read

<br>

<!-- Extract all unique categories from the books -->
{% assign categories = site.books | map: "category" | compact | uniq %}

<!-- Loop through each category -->
{% for category in categories %}
  
  <!-- Category Title -->
  <h3 class="mt-4 mb-3" style="border-bottom: 2px solid var(--global-divider-color); padding-bottom: 5px;">
    {{ category | replace: "-", " " | capitalize }}
  </h3>
  
  <!-- Grid for displaying book cards -->
  <div class="row row-cols-2 row-cols-sm-3 row-cols-md-4 g-4 mb-5">
    {% assign category_books = site.books | where: "category", category %}
    {% for book in category_books %}
      <div class="col">
        <div class="card h-100 hoverable">
          <a href="{{ book.link | default: book.url | relative_url }}" target="_blank">
            <img src="{{ book.cover | relative_url }}" class="card-img-top" alt="{{ book.title }}" style="object-fit: cover; height: 100%;">
          </a>          
          <!-- Set the color and text for the status bar -->
          {% assign status_text = book.status | default: "TO READ" | upcase %}
          {% if status_text == "FINISHED" %}
            {% assign status_color = "#93c47d" %}
          {% elsif status_text == "READING" %}
            {% assign status_color = "#ffd966" %}
          {% else %}
            {% assign status_color = "#d3d3d3" %}
          {% endif %}          
          <div class="card-footer text-center py-1" style="background-color: {{ status_color }}; font-size: 0.75rem; font-weight: bold; letter-spacing: 1px; color: #333;">
            {{ status_text }}
          </div>
        </div>
      </div>
    {% endfor %}
  </div>

{% endfor %}
