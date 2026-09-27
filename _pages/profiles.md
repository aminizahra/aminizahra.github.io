---
layout: page
permalink: /recommendations/
title: Recommendations
description: "Professors, managers, and colleagues who have guided my academic and professional journey."
nav: true
nav_order: 5
---

<style>
  /* --- Chic & Minimalist Card Design --- */
  
  .category-title {
    margin-top: 50px;
    margin-bottom: 30px;
    padding-bottom: 12px;
    border-bottom: 1px solid var(--global-divider-color);
    color: var(--global-text-color);
    font-weight: 800;
    font-size: 1.8rem;
    letter-spacing: 0.5px;
  }

  .mentor-card {
    background-color: var(--global-card-bg-color);
    border: 1px solid var(--global-divider-color);
    border-radius: 20px;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    overflow: hidden;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 35px 20px 20px 20px;
    text-align: center;
    position: relative;
  }

  .mentor-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 15px 35px rgba(0,0,0,0.15);
    border-color: var(--global-theme-color);
  }

  .mentor-img-wrapper {
    position: relative;
    margin-bottom: 20px;
    width: 120px;
    height: 120px;
  }

  .mentor-img-wrapper img.main-profile {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 50%;
    border: 4px solid var(--global-card-bg-color);
    outline: 2px solid var(--global-theme-color);
    box-shadow: 0 8px 20px rgba(0,0,0,0.12);
    transition: transform 0.4s ease;
  }

  .inst-badge-logo {
    position: absolute;
    bottom: -2px;
    right: -2px;
    width: 42px;
    height: 42px;
    background-color: #ffffff;
    border-radius: 50%;
    padding: 5px;
    border: 2px solid var(--global-card-bg-color);
    box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    object-fit: contain;
    z-index: 5;
    transition: transform 0.3s ease;
  }

  .mentor-card:hover .mentor-img-wrapper img.main-profile {
    transform: scale(1.05);
  }
  
  .mentor-card:hover .inst-badge-logo {
    transform: scale(1.15);
  }

  .mentor-name {
    font-weight: 700;
    font-size: 1.3rem;
    color: var(--global-text-color);
    margin-bottom: 8px;
  }

  .mentor-desc {
    font-size: 0.95rem;
    font-weight: 500;
    color: var(--global-text-muted-color);
    line-height: 1.4;
    margin-bottom: 18px;
    display: -webkit-box;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    overflow: hidden;
    padding: 0 10px;
  }

  .mentor-relation {
    font-size: 0.85rem;
    margin-bottom: 20px;
    line-height: 1.5;
    padding: 10px 15px;
    background-color: rgba(128, 128, 128, 0.05); 
    border-radius: 12px;
    width: 95%;
  }

  .relation-label {
    color: var(--global-text-muted-color);
    font-weight: 500;
    font-style: italic; 
  }

  .relation-value {
    color: var(--global-theme-color);
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    display: block;
    margin-top: 4px;
  }

  .mentor-badge {
    background-color: transparent;
    color: var(--global-theme-color);
    border: 1px solid var(--global-theme-color);
    font-weight: 600;
    padding: 6px 16px;
    border-radius: 30px;
    font-size: 0.75rem;
    letter-spacing: 0.5px;
    margin-bottom: 25px;
    display: inline-block;
  }

  .view-profile-btn {
    margin-top: auto;
    width: 100%;
    padding-top: 15px;
    border-top: 1px dashed var(--global-divider-color);
  }

  .view-profile-btn span {
    font-size: 0.85rem;
    font-weight: 700;
    color: var(--global-text-muted-color);
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: color 0.3s ease;
  }

  .mentor-card:hover .view-profile-btn span {
    color: var(--global-theme-color);
  }

  a.mentor-link-wrapper {
    text-decoration: none !important;
    color: inherit !important;
    display: block;
    height: 100%;
  }
</style>

<!-- Extract unique categories from the _people collection -->
{% assign categories = site.people | map: "category" | compact | uniq %}

<!-- Iterate over each category -->
{% for category in categories %}
  <h2 class="category-title">{{ category }}</h2>
  
  <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4 mb-5">    
    <!-- Iterate over people belonging to the current category -->
    {% for person in site.people %}
      {% if person.category == category %}
        <div class="col">          
          <a href="{{ person.url | relative_url }}" class="mentor-link-wrapper">
            <div class="mentor-card">              
              <!-- Profile Image & University Badge -->
              <div class="mentor-img-wrapper">
                <img src="{{ person.img | relative_url }}" class="main-profile" alt="{{ person.title }}">
                {% if person.university_logo %}
                  <img src="{{ person.university_logo | relative_url }}" class="inst-badge-logo" alt="Institution Logo" title="Institution">
                {% endif %}
              </div>              
              <!-- Name -->
              <h3 class="mentor-name">{{ person.title }}</h3>              
              <!-- Role / Description (Institution highlighted) -->
              <p class="mentor-desc">
                {{ person.description | split: '|' | first | strip }}
              </p>              
              <!-- Role / Relationship (Moved below the description with a chic box) -->
              {% if person.relation %}
                <div class="mentor-relation">
                  <span class="relation-label">Supervised me as:</span>
                  <span class="relation-value">{{ person.relation }}</span>
                </div>
              {% endif %}              
              <!-- Badge -->
              {% if person.badge %}
                <div class="mentor-badge">
                  <i class="fas fa-award mr-1"></i> {{ person.badge }}
                </div>
              {% endif %}              
              <!-- Footer / View Profile -->
              <div class="view-profile-btn">
                <span>View Profile &rarr;</span>
              </div>              
            </div>
          </a>          
        </div>
      {% endif %}
    {% endfor %}
    
  </div>
{% endfor %}
