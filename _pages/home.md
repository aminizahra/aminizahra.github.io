---
layout: page
permalink: /
title: Home
nav: true
nav_order: 1
---

<style>
  /* --- Modern Hero Section --- */
  .hero-container {
    text-align: center;
    padding: 60px 20px 80px 20px;
    margin-top: 20px;
  }
  
  .hero-title {
    font-size: 3.5rem;
    font-weight: 800;
    letter-spacing: -1px;
    color: var(--global-text-color);
    margin-bottom: 15px;
  }
  
  .hero-title span {
    color: var(--global-theme-color);
  }
  
  .hero-subtitle {
    font-size: 1.25rem;
    font-weight: 400;
    color: var(--global-text-muted-color);
    max-width: 700px;
    margin: 0 auto 40px auto;
    line-height: 1.6;
  }
  
  /* --- CTA Buttons --- */
  .hero-buttons {
    display: flex;
    gap: 20px;
    justify-content: center;
    margin-bottom: 60px;
  }
  
  .btn-hero {
    padding: 12px 30px;
    border-radius: 30px;
    font-weight: 600;
    font-size: 1rem;
    letter-spacing: 0.5px;
    text-decoration: none !important;
    transition: all 0.3s ease;
  }
  
  .btn-hero-primary {
    background-color: var(--global-theme-color);
    color: #fff !important;
    border: 2px solid var(--global-theme-color);
    box-shadow: 0 8px 20px rgba(46, 134, 193, 0.3);
  }
  
  .btn-hero-primary:hover {
    transform: translateY(-3px);
    box-shadow: 0 12px 25px rgba(46, 134, 193, 0.4);
  }
  
  .btn-hero-secondary {
    background-color: transparent;
    color: var(--global-text-color) !important;
    border: 2px solid var(--global-divider-color);
  }
  
  .btn-hero-secondary:hover {
    border-color: var(--global-theme-color);
    color: var(--global-theme-color) !important;
    transform: translateY(-3px);
  }

  /* --- Highlights / Focus Areas --- */
  .focus-cards {
    margin-top: 40px;
  }
  
  .focus-card {
    padding: 30px 20px;
    border-radius: 16px;
    background-color: var(--global-card-bg-color);
    border: 1px solid var(--global-divider-color);
    text-align: center;
    height: 100%;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  
  .focus-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 10px 30px rgba(0,0,0,0.08);
    border-color: var(--global-theme-color);
  }
  
  .focus-icon {
    font-size: 2.5rem;
    color: var(--global-theme-color);
    margin-bottom: 20px;
  }
  
  .focus-title {
    font-size: 1.2rem;
    font-weight: 700;
    margin-bottom: 12px;
    color: var(--global-text-color);
  }
  
  .focus-text {
    font-size: 0.9rem;
    color: var(--global-text-muted-color);
    line-height: 1.5;
  }
</style>

<!-- Hero Section -->
<div class="hero-container">
  <h1 class="hero-title">Hello, I'm <span>Zahra Amini</span></h1>
  <p class="hero-subtitle">
    AI Developer, Data Scientist, and Tech Educator bridging the gap between advanced Machine Learning theory and practical, real-world deployment. Founder of Hobot Academy.
  </p>
  
  <div class="hero-buttons">
    <a href="{{ '/cv/' | relative_url }}" class="btn-hero btn-hero-primary">
      <i class="fas fa-file-alt mr-2"></i> View My CV
    </a>
    <a href="{{ '/projects/' | relative_url }}" class="btn-hero btn-hero-secondary">
      <i class="fas fa-code mr-2"></i> Explore Projects
    </a>
  </div>
</div>

<hr style="border-top-color: var(--global-divider-color); margin: 20px 0 50px 0;">

<!-- Core Focus Areas (3 Columns) -->
<div class="row row-cols-1 row-cols-md-3 g-4 focus-cards mb-5">
  
  <div class="col">
    <div class="focus-card">
      <div class="focus-icon"><i class="fas fa-brain"></i></div>
      <h3 class="focus-title">Artificial Intelligence</h3>
      <p class="focus-text">Expertise in Deep Learning, Computer Vision, and Natural Language Processing (NLP) with a focus on scalable architectures.</p>
    </div>
  </div>
  
  <div class="col">
    <div class="focus-card">
      <div class="focus-icon"><i class="fas fa-chart-network"></i></div>
      <h3 class="focus-title">Data Science</h3>
      <p class="focus-text">Transforming complex, unstructured data into actionable insights using advanced statistical analysis and machine learning algorithms.</p>
    </div>
  </div>
  
  <div class="col">
    <div class="focus-card">
      <div class="focus-icon"><i class="fas fa-chalkboard-teacher"></i></div>
      <h3 class="focus-title">Tech Education</h3>
      <p class="focus-text">Passionate about democratizing AI education. Mentored thousands of students as a Lecturer and founder of Hobot Academy.</p>
    </div>
  </div>
  
</div>

<!-- Optional: Latest News/Updates Section -->
<h3 style="font-weight: 700; margin-top: 60px; margin-bottom: 20px; color: var(--global-text-color);">Latest News</h3>
{% include news.liquid limit=true %}
