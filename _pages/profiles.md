---
layout: page
permalink: /recommendations/
title: Recommendations
description: "Professors, managers, and colleagues who have guided my academic and professional journey."
nav: true
nav_order: 5
---

<style>
  /* Custom styles for the mentor cards */
  .mentor-card {
    border: none;
    border-radius: 12px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.08);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    overflow: hidden;
    background: #fff;
    height: 100%;
  }
  .mentor-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 25px rgba(0,0,0,0.15);
  }
  .card-header-bg {
    background: linear-gradient(135deg, #2e86c1 0%, #1a5276 100%);
    height: 80px;
    width: 100%;
  }
  .mentor-img-wrapper {
    margin-top: -50px;
    text-align: center;
  }
  .mentor-img-wrapper img {
    width: 100px;
    height: 100px;
    object-fit: cover;
    border: 4px solid #fff;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  }
  .category-title {
    margin-top: 40px;
    margin-bottom: 25px;
    padding-bottom: 10px;
    border-bottom: 2px solid #2e86c1;
    color: #333;
    font-weight: bold;
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
          <div class="mentor-card">
            
            <a href="{{ person.url | relative_url }}" style="text-decoration: none; color: inherit;">
              <!-- Colored Header Background -->
              <div class="card-header-bg"></div>
              
              <!-- Profile Image -->
              <div class="mentor-img-wrapper">
                <img src="{{ person.img | relative_url }}" alt="{{ person.title }}" class="rounded-circle">
              </div>
              
              <div class="card-body text-center mt-2">
                <!-- Name -->
                <h5 class="card-title mb-1" style="font-weight: 700;">{{ person.title }}</h5>
                <p class="text-muted" style="font-size: 0.9rem; line-height: 1.4; height: 40px; overflow: hidden;">
                  <!-- Displaying the first part of the description -->
                  {{ person.description | split: '|' | first }}
                </p>
                
                <!-- Badge (e.g., Recommendation Letter) -->
                <div class="mt-3">
                  {% if person.badge %}
                    <span class="badge" style="background-color: #2e86c1; font-weight: normal; padding: 6px 10px;">
                      <i class="fas fa-certificate mr-1"></i> {{ person.badge }}
                    </span>
                  {% endif %}
                </div>
              </div>
            </a>
            
            <!-- View Profile Button -->
            <div class="card-footer bg-white border-0 text-center pb-4">
              <a href="{{ person.url | relative_url }}" class="btn btn-outline-primary btn-sm rounded-pill" style="border-color: #2e86c1; color: #2e86c1;">
                View Profile <i class="fas fa-arrow-right ml-1"></i>
              </a>
            </div>
            
          </div>
        </div>
      {% endif %}
    {% endfor %}
    
  </div>
{% endfor %}
