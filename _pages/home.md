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
    padding: 80px 20px 60px 20px;
    position: relative;
  }
  
  .hero-title {
    font-size: 3.5rem;
    font-weight: 800;
    letter-spacing: -1px;
    color: var(--global-text-color);
    margin-bottom: 20px;
    line-height: 1.2;
  }
  
  .hero-title span.accent {
    color: var(--global-theme-color);
    position: relative;
    display: inline-block;
  }
  
  .hero-subtitle {
    font-size: 1.15rem;
    font-weight: 400;
    color: var(--global-text-muted-color);
    max-width: 750px;
    margin: 0 auto 40px auto;
    line-height: 1.7;
  }

  .highlight-badge {
    display: inline-block;
    background-color: rgba(46, 134, 193, 0.1);
    color: var(--global-theme-color);
    border: 1px solid rgba(46, 134, 193, 0.3);
    padding: 5px 15px;
    border-radius: 20px;
    font-size: 0.85rem;
    font-weight: 600;
    margin-bottom: 20px;
    letter-spacing: 0.5px;
  }
  
  /* --- CTA Buttons --- */
  .hero-buttons {
    display: flex;
    gap: 15px;
    justify-content: center;
    margin-bottom: 60px;
    flex-wrap: wrap;
  }
  
  .btn-hero {
    padding: 12px 28px;
    border-radius: 30px;
    font-weight: 600;
    font-size: 0.95rem;
    letter-spacing: 0.5px;
    text-decoration: none !important;
    transition: all 0.3s ease;
    display: flex;
    align-items: center;
    gap: 8px;
  }
  
  .btn-hero-primary {
    background-color: var(--global-theme-color);
    color: #fff !important;
    border: 2px solid var(--global-theme-color);
    box-shadow: 0 8px 20px rgba(46, 134, 193, 0.25);
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

  /* --- Expertise Cards --- */
  .focus-cards {
    margin-top: 40px;
  }
  
  .focus-card {
    padding: 35px 25px;
    border-radius: 16px;
    background-color: var(--global-card-bg-color);
    border: 1px solid var(--global-divider-color);
    text-align: center;
    height: 100%;
    transition: transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275), box-shadow 0.4s ease;
  }
  
  .focus-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 15px 35px rgba(0,0,0,0.1);
    border-color: var(--global-theme-color);
  }
  
  .focus-icon {
    font-size: 2.5rem;
    color: var(--global-theme-color);
    margin-bottom: 20px;
  }
  
  .focus-title {
    font-size: 1.15rem;
    font-weight: 700;
    margin-bottom: 12px;
    color: var(--global-text-color);
  }
  
  .focus-text {
    font-size: 0.9rem;
    color: var(--global-text-muted-color);
    line-height: 1.6;
  }
</style>

<!-- Hero Section -->
<div class="hero-container">
  <div class="highlight-badge">
    <i class="fas fa-trophy mr-1"></i> Ranked #3 in Data Science (Iran) by Favikon
  </div>
  
  <h1 class="hero-title">Bridging <span class="accent">Healthcare</span> & <span class="accent">AI</span></h1>
  
  <p class="hero-subtitle">
    I am <strong>Zahra Amini</strong>, an AI Developer, Data Scientist, and Tech Educator. My research bridges advanced Machine Learning and clinical applications, focusing on Explainable AI (XAI), Medical Image Segmentation, and Time-Series Signal Processing.
  </p>
  
  <div class="hero-buttons">
    <a href="{{ '/about/' | relative_url }}" class="btn-hero btn-hero-primary">
      <i class="fas fa-user"></i> More About Me
    </a>
    <a href="{{ '/cv/' | relative_url }}" class="btn-hero btn-hero-secondary">
      <i class="fas fa-file-pdf"></i> View Resume
    </a>
    <a href="{{ '/recommendations/' | relative_url }}" class="btn-hero btn-hero-secondary">
      <i class="fas fa-award"></i> Recommendations
    </a>
  </div>
</div>

<hr style="border-top-color: var(--global-divider-color); margin: 20px 0 60px 0;">

<!-- Core Expertise Areas (3 Columns based on CV) -->
<h3 style="font-weight: 800; text-align: center; margin-bottom: 40px; color: var(--global-text-color);">Core Expertise</h3>

<div class="row row-cols-1 row-cols-md-3 g-4 focus-cards mb-5">
  
  <div class="col">
    <div class="focus-card">
      <div class="focus-icon"><i class="fas fa-heartbeat"></i></div>
      <h3 class="focus-title">Biomedical AI & XAI</h3>
      <p class="focus-text">Developing Explainable AI models for clinical decision support, including calibrated ML prediction systems for healthcare triage and anomaly detection.</p>
    </div>
  </div>
  
  <div class="col">
    <div class="focus-card">
      <div class="focus-icon"><i class="fas fa-cube"></i></div>
      <h3 class="focus-title">Advanced Computer Vision</h3>
      <p class="focus-text">Specializing in Medical Image Semantic Segmentation (U-Net) and large-scale 3D Point Cloud Processing using state-of-the-art Deep Learning architectures.</p>
    </div>
  </div>
  
  <div class="col">
    <div class="focus-card">
      <div class="focus-icon"><i class="fas fa-chalkboard-teacher"></i></div>
      <h3 class="focus-title">AI Education & Leadership</h3>
      <p class="focus-text">Founder of Hobot Academy and lead author of "Introduction to AI in Healthcare." Mentored hundreds of students in deploying real-world machine learning models.</p>
    </div>
  </div>
  
</div>

<hr style="border-top-color: var(--global-divider-color); margin: 60px 0 40px 0;">

<!-- Latest News Integration -->
<h3 style="font-weight: 800; margin-bottom: 25px; color: var(--global-text-color);">Recent Updates</h3>
{% include news.liquid limit=true %}
