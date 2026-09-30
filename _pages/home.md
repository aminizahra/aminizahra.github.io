---
layout: page
permalink: /
title: Home
nav: true
nav_order: 1
description: Zahra Amini - Machine learning researcher in healthcare AI
---

<style>
  .za-hero { display: flex; gap: 2.5rem; align-items: center; flex-wrap: wrap; margin: 1rem 0 2.5rem; }
  .za-hero-photo { width: 190px; height: 190px; border-radius: 50%; object-fit: cover; flex: 0 0 auto; }
  .za-hero-text { flex: 1 1 320px; min-width: 0; }
  .za-hero-text h1 { font-size: 2.2rem; margin-bottom: .25rem; }
  .za-role { font-size: 1.15rem; color: var(--global-text-color-light); margin-bottom: 1rem; }
  .za-status { display: inline-block; padding: .3rem .8rem; border: 1px solid var(--global-theme-color); border-radius: 999px; font-size: .9rem; margin-bottom: 1.1rem; }
  .za-actions { display: flex; flex-wrap: wrap; gap: .6rem; margin: 1.1rem 0; }
  .za-btn { padding: .5rem 1.1rem; border-radius: 4px; border: 1px solid var(--global-theme-color); color: var(--global-theme-color); text-decoration: none; font-weight: 500; }
  .za-btn:hover { background: var(--global-theme-color); color: var(--global-bg-color); text-decoration: none; }
  .za-btn.primary { background: var(--global-theme-color); color: var(--global-bg-color); }
  .za-btn.primary:hover { opacity: .88; }
  .za-links { display: flex; flex-wrap: wrap; gap: 1.1rem; font-size: 1.6rem; }
  .za-links a { color: var(--global-text-color-light); }
  .za-links a:hover { color: var(--global-theme-color); }
  .za-section { margin: 3rem 0; }
  .za-section > h2 { font-size: 1.5rem; margin-bottom: 1.1rem; padding-bottom: .4rem; border-bottom: 1px solid var(--global-divider-color); }
  .za-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 1.1rem; }
  .za-card { padding: 1.1rem 1.2rem; border: 1px solid var(--global-divider-color); border-radius: 6px; background: var(--global-card-bg-color); }
  .za-card h3 { font-size: 1.1rem; margin: 0 0 .5rem; }
  .za-card p { margin: 0 0 .6rem; font-size: .95rem; }
  .za-card .za-more { font-size: .9rem; }
  .za-tag { display: inline-block; font-size: .78rem; padding: .1rem .55rem; margin-bottom: .5rem; border: 1px solid var(--global-divider-color); border-radius: 4px; color: var(--global-text-color-light); }
  .za-tag.pending { border-color: var(--global-theme-color); color: var(--global-theme-color); }
  .za-timeline { list-style: none; padding: 0; margin: 0; }
  .za-timeline li { display: grid; grid-template-columns: 9rem 1fr; gap: 1rem; padding: .8rem 0; border-bottom: 1px solid var(--global-divider-color); }
  .za-timeline li:last-child { border-bottom: 0; }
  .za-date { color: var(--global-text-color-light); font-size: .92rem; }
  .za-stats { display: grid; grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); gap: 1rem; text-align: center; }
  .za-stat b { display: block; font-size: 1.8rem; color: var(--global-theme-color); }
  .za-stat span { font-size: .9rem; color: var(--global-text-color-light); }
  .za-quote { border-left: 3px solid var(--global-theme-color); padding: .2rem 0 .2rem 1rem; margin: 0 0 1rem; }
  .za-quote footer { font-size: .9rem; color: var(--global-text-color-light); margin-top: .3rem; }
  .za-contact { text-align: center; padding: 2rem 1rem; border: 1px solid var(--global-divider-color); border-radius: 6px; }
  @media (max-width: 576px) {
    .za-hero { justify-content: center; text-align: center; }
    .za-actions, .za-links { justify-content: center; }
    .za-timeline li { grid-template-columns: 1fr; gap: .1rem; }
  }
</style>

<!-- ============ 1. HERO ============ -->
<section class="za-hero">
  <!-- TODO: put a professional portrait at assets/img/prof_pic.jpg -->
  <img class="za-hero-photo" src="{{ '/assets/img/prof_pic.jpg' | relative_url }}" alt="Portrait of Zahra Amini">
  <div class="za-hero-text">
    <h1>Zahra Amini</h1>
    <p class="za-role">Machine learning researcher in healthcare AI</p>
    <span class="za-status">Seeking a fully funded PhD position in the UK, starting 2027</span>
    <p>
      I develop explainable, well-calibrated machine learning models for biomedical data:
      clinical tabular records, medical images and physiological signals.
      I currently work as a Research Assistant at the University of Staffordshire.
    </p>
    <div class="za-actions">
      <a class="za-btn primary" href="{{ '/assets/pdf/CV-Zahra-Amini.pdf' | relative_url }}">Download CV</a>
      <a class="za-btn" href="#publications">Publications</a>
      <a class="za-btn" href="mailto:amini75zahra@gmail.com">Contact</a>
    </div>
    <div class="za-links">
      <!-- TODO: add your Google Scholar and ORCID URLs -->
      <a href="mailto:amini75zahra@gmail.com" title="Email"><i class="fa-solid fa-envelope"></i></a>
      <a href="https://scholar.google.com/citations?user=YOUR_ID" target="_blank" rel="noopener" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>
      <a href="https://orcid.org/YOUR-ORCID" target="_blank" rel="noopener" title="ORCID"><i class="ai ai-orcid"></i></a>
      <a href="https://linkedin.com/in/zahraamini-ai" target="_blank" rel="noopener" title="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>
      <a href="https://github.com/aminizahra" target="_blank" rel="noopener" title="GitHub"><i class="fa-brands fa-github"></i></a>
      <a href="https://kaggle.com/aminizahra" target="_blank" rel="noopener" title="Kaggle"><i class="fa-brands fa-kaggle"></i></a>
    </div>
  </div>
</section>

<!-- ============ 2. RESEARCH INTERESTS ============ -->
<section class="za-section" id="research">
  <h2>Research interests</h2>
  <div class="za-grid">
    <div class="za-card">
      <h3>Explainable and calibrated clinical ML</h3>
      <p>Prediction models for clinical decision support whose probabilities can be trusted and whose decisions can be explained to clinicians.</p>
      <p class="za-more">Example: general anaesthesia triage in paediatric dentistry.</p>
    </div>
    <div class="za-card">
      <h3>Medical image and 3D segmentation</h3>
      <p>Deep learning for semantic segmentation, from U-Net on medical images to superpoint graphs on large-scale 3D point clouds.</p>
      <p class="za-more">Example: B.Sc. thesis on point cloud segmentation.</p>
    </div>
    <div class="za-card">
      <h3>Time-series and anomaly detection</h3>
      <p>Signal processing and unsupervised models for sensor and bio-signal data, including predictive maintenance in heavy industry.</p>
      <p class="za-more">Example: Isolation Forest models at NICICO.</p>
    </div>
  </div>
</section>

<!-- ============ 3. PUBLICATIONS ============ -->
<section class="za-section" id="publications">
  <h2>Selected publications</h2>
  <div class="za-grid">
    <div class="za-card">
      <span class="za-tag pending">Under review</span>
      <h3>A calibrated prediction model for general anaesthesia triage in paediatric dentistry</h3>
      <p>Sadegh-Zadeh S.-A., Bagheri M., <b>Amini Z.</b>, Saadat S., Barati M. A., Jarchi D.</p>
      <p class="za-more">Development, explainability and preliminary external evaluation.</p>
      <!-- TODO: link the preprint here when available -->
    </div>
    <div class="za-card">
      <span class="za-tag pending">In press</span>
      <h3>Introduction to Artificial Intelligence in Healthcare</h3>
      <p><b>Amini Z.</b> (lead author) et al. Shahid Beheshti University of Medical Sciences Press.</p>
      <p class="za-more">Textbook for medical students and professionals.</p>
    </div>
    <div class="za-card">
      <span class="za-tag">B.Sc. thesis, 20/20</span>
      <h3>Large-scale semantic point cloud segmentation with superpoint graphs</h3>
      <p><b>Amini Z.</b> Supervised by Dr. Amir Salarpour, Sirjan University of Technology, 2020.</p>
    </div>
  </div>
  <p style="margin-top:1rem"><a href="{{ '/publications/' | relative_url }}">All publications</a></p>
</section>

<!-- ============ 4. PROJECTS ============ -->
<section class="za-section" id="projects">
  <h2>Selected projects</h2>
  <!-- TODO: replace with your 3 strongest projects, one per research theme -->
  <div class="za-grid">
    <div class="za-card">
      <h3>Project title (explainable ML)</h3>
      <p>One sentence on the problem, one on the method, one on the result.</p>
      <a class="za-more" href="https://github.com/aminizahra">Code on GitHub</a>
    </div>
    <div class="za-card">
      <h3>Project title (medical image segmentation)</h3>
      <p>One sentence on the problem, one on the method, one on the result.</p>
      <a class="za-more" href="https://github.com/aminizahra">Code on GitHub</a>
    </div>
    <div class="za-card">
      <h3>Project title (time-series)</h3>
      <p>One sentence on the problem, one on the method, one on the result.</p>
      <a class="za-more" href="https://github.com/aminizahra">Code on GitHub</a>
    </div>
  </div>
  <p style="margin-top:1rem"><a href="{{ '/projects/' | relative_url }}">All projects</a></p>
</section>

<!-- ============ 5. RESEARCH EXPERIENCE ============ -->
<section class="za-section" id="experience">
  <h2>Research experience</h2>
  <ul class="za-timeline">
    <li>
      <span class="za-date">2024 to present</span>
      <div><b>Research Assistant</b>, University of Staffordshire<br>
      Supervisor: Dr. Seyed-Ali Sadegh-Zadeh. Calibrated, explainable triage model on clinical tabular data.</div>
    </li>
    <li>
      <span class="za-date">2024 and 2025</span>
      <div><b>Data Scientist and Research Consultant</b>, NICICO<br>
      Anomaly detection and predictive maintenance on sensor time series; an LLM assistant over internal technical documents.</div>
    </li>
    <li>
      <span class="za-date">2019 to 2021</span>
      <div><b>Research Assistant and thesis student</b>, Sirjan University of Technology<br>
      Supervisor: Dr. Amir Salarpour. Scalable 3D point cloud segmentation.</div>
    </li>
  </ul>
  <p style="margin-top:.8rem"><a href="{{ '/cv/' | relative_url }}">Full CV</a></p>
</section>

<!-- ============ 6. TEACHING AND IMPACT ============ -->
<section class="za-section" id="impact">
  <h2>Teaching and impact</h2>
  <div class="za-stats">
    <div class="za-stat"><b>200+</b><span>medical students taught in Neuro-AI</span></div>
    <div class="za-stat"><b>200+</b><span>students mentored in the AI scholarship</span></div>
    <div class="za-stat"><b>Master</b><span>Kaggle, 2021 to 2025</span></div>
    <div class="za-stat"><b>#3</b><span>Data Science in Iran, Favikon 2025</span></div>
  </div>
  <p style="margin-top:1.1rem">
    I founded Hobot Academy and have taught machine learning, deep learning and applied mathematics since 2022.
    <a href="{{ '/teaching/' | relative_url }}">Courses and notes</a>
  </p>
</section>

<!-- ============ 7. NEWS ============ -->
<!-- TODO: keep only real, dated items. Remove this section if you have fewer than 3. -->
<section class="za-section" id="news">
  <h2>News</h2>
  <ul class="za-timeline">
    <li><span class="za-date">2026</span><div>Paediatric dentistry triage manuscript submitted for review.</div></li>
    <li><span class="za-date">2026</span><div>Textbook <i>Introduction to Artificial Intelligence in Healthcare</i> accepted by SBMU Press.</div></li>
    <li><span class="za-date">2025</span><div>Named "The AI Luminary" and ranked #3 in Data Science (Iran) by Favikon.</div></li>
  </ul>
</section>

<!-- ============ 8. RECOMMENDATIONS ============ -->
<section class="za-section" id="recommendations">
  <h2>Recommendations</h2>
  <!-- TODO: use short excerpts only with the writer's permission -->
  <blockquote class="za-quote">
    Short excerpt from a recommendation letter.
    <footer>Name, title, institution</footer>
  </blockquote>
  <a href="{{ '/recommendations/' | relative_url }}">Read all recommendations</a>
</section>

<!-- ============ 9. CONTACT ============ -->
<section class="za-section" id="contact">
  <div class="za-contact">
    <h2 style="border:0;margin-bottom:.6rem">Open to PhD opportunities in healthcare AI</h2>
    <p>If our research interests align, I would be glad to hear from you.</p>
    <div class="za-actions" style="justify-content:center">
      <a class="za-btn primary" href="mailto:amini75zahra@gmail.com">Email me</a>
      <a class="za-btn" href="{{ '/assets/pdf/CV-Zahra-Amini.pdf' | relative_url }}">Download CV</a>
    </div>
  </div>
</section>
