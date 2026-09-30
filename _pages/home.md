---
layout: page
title: Home
permalink: /
nav: false
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
    <span class="za-status">Applying for PhD and research-oriented MSc programmes in healthcare AI, Europe, 2027 intake</span>
    <p>
      I develop explainable, well-calibrated machine learning models for biomedical data:
      clinical tabular records, medical images and physiological signals.
    </p>
    <div class="za-actions">
      <a class="za-btn" href="{{ 'assets/pdf/CV-ZahraAmini.pdf' | relative_url }}">Download CV</a>
      <a class="za-btn" href="#research-outputs">Research outputs</a>
      <a class="za-btn" href="mailto:amini75zahra@gmail.com">Contact</a>
    </div>
    <div class="za-links">
      <!-- TODO: add your Google Scholar and ORCID URLs -->
      <a href="mailto:amini75zahra@gmail.com" title="Email"><i class="fa-solid fa-envelope"></i></a>
      <!-- <a href="https://scholar.google.com/citations?user=YOUR_ID" target="_blank" rel="noopener" title="Google Scholar"><i class="ai ai-google-scholar"></i></a> -->
      <!-- <a href="https://orcid.org/YOUR-ORCID" target="_blank" rel="noopener" title="ORCID"><i class="ai ai-orcid"></i></a> -->
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

<!-- ============ 3. RESEARCH OUTPUTS ============ -->
<section class="za-section" id="research-outputs">
  <h2>Research outputs</h2>
  <div class="za-grid">
    <div class="za-card">
      <span class="za-tag pending">Manuscript under review</span>
      <h3>A calibrated prediction model for general anaesthesia triage in paediatric dentistry: development, explainability, and preliminary external evaluation</h3>
      <p>Seyed-Ali Sadegh-Zadeh, Mahshid Bagheri, <b>Zahra Amini</b>, Shayan Saadat, Mohammad Amin Barati, Delaram Jarchi</p>
      <p class="za-more">A calibrated ML prediction model on clinical tabular data for general anaesthesia triage, with explainable AI (XAI) techniques to ensure clinical transparency.</p>
      <!-- TODO: add links to the preprint and code when available -->
    </div>
    <div class="za-card">
      <span class="za-tag pending">Book, in press</span>
      <h3>Introduction to Artificial Intelligence in Healthcare</h3>
      <p><b>Zahra Amini</b> (lead author), et al. Shahid Beheshti University of Medical Sciences Press.</p>
      <p class="za-more">An interdisciplinary textbook bridging machine learning, data analytics and healthcare, for medical students and professionals.</p>
    </div>
    <div class="za-card">
      <span class="za-tag">B.Sc. thesis, Spring 2020</span>
      <h3>Large-scale semantic point cloud segmentation with superpoint graphs</h3>
      <p><b>Zahra Amini</b>. Department of Software Engineering, Sirjan University of Technology. Supervisor: Dr. Amir Salarpour. Grade: 20/20.</p>
      <p class="za-more">A 3D point cloud processing framework for semantic segmentation.</p>
    </div>
  </div>
  <p style="margin-top:1rem"><a href="{{ '/publications/' | relative_url }}">Details and full list</a></p>
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
    <!-- TODO: replace MONTH YEAR with the real dates -->
    <li><span class="za-date">MONTH YEAR</span><div>Paediatric dentistry triage manuscript submitted for review.</div></li>
    <li><span class="za-date">MONTH YEAR</span><div>Textbook <i>Introduction to Artificial Intelligence in Healthcare</i> in press with Shahid Beheshti University of Medical Sciences Press.</div></li>
    <li><span class="za-date">2025</span><div>Named "The AI Luminary" and ranked #3 in Data Science (Iran) by Favikon.</div></li>
  </ul>
</section>

<!-- ============ 8. RECOMMENDATIONS ============ -->
<section class="za-section" id="recommendations">
<style>
  #recommendations .rs-bar { display: flex; justify-content: space-between; align-items: center; margin-bottom: .6rem; font-size: .95rem; }
  #recommendations .rs-arrows { display: flex; gap: .4rem; }
  #recommendations .rs-arrow { width: 2rem; height: 2rem; padding: 0; border: 1px solid var(--global-divider-color); border-radius: 50%; background: transparent; color: var(--global-text-color); cursor: pointer; line-height: 1; }
  #recommendations .rs-arrow:hover:not(:disabled) { border-color: var(--global-theme-color); color: var(--global-theme-color); }
  #recommendations .rs-arrow:focus-visible { outline: 2px solid var(--global-theme-color); outline-offset: 2px; }
  #recommendations .rs-arrow:disabled { opacity: .35; cursor: default; }
  #recommendations .rs-track { display: flex; gap: 1.25rem; overflow-x: auto; scroll-snap-type: x mandatory; scrollbar-width: none; padding: 14px 4px 24px; }
  #recommendations .rs-track::-webkit-scrollbar { display: none; }
  #recommendations a.rs-slide { flex: 0 0 calc((100% - 2.5rem) / 3); min-width: 250px; scroll-snap-align: start; display: flex; }
  @media (max-width: 768px) { #recommendations a.rs-slide { flex-basis: 82%; } }

  /* Same card design as the Recommendations page */
  #recommendations .mentor-card { background-color: var(--global-card-bg-color); border: 1px solid var(--global-divider-color); border-radius: 20px; transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); overflow: hidden; width: 100%; display: flex; flex-direction: column; align-items: center; padding: 30px 15px 15px 15px; text-align: center; position: relative; }
  #recommendations .mentor-card:hover { transform: translateY(-8px); box-shadow: 0 15px 35px rgba(0,0,0,0.15); border-color: var(--global-theme-color); }
  #recommendations .mentor-img-wrapper { position: relative; margin-bottom: 15px; width: 100px; height: 100px; }
  #recommendations .mentor-img-wrapper img.main-profile { width: 100%; height: 100%; object-fit: cover; border-radius: 50%; border: 4px solid var(--global-card-bg-color); outline: 2px solid var(--global-theme-color); box-shadow: 0 8px 20px rgba(0,0,0,0.12); transition: transform 0.4s ease; }
  #recommendations .inst-badge-logo { position: absolute; bottom: -4px; right: -4px; width: 36px; height: 36px; background-color: #ffffff; border-radius: 50%; padding: 4px; border: 2px solid var(--global-card-bg-color); box-shadow: 0 4px 10px rgba(0,0,0,0.2); object-fit: contain; z-index: 5; transition: transform 0.3s ease; }
  #recommendations .mentor-card:hover .mentor-img-wrapper img.main-profile { transform: scale(1.05); }
  #recommendations .mentor-card:hover .inst-badge-logo { transform: scale(1.15); }
  #recommendations .mentor-name { font-weight: 700; font-size: 1.15rem; color: var(--global-text-color); margin-bottom: 6px; }
  #recommendations .mentor-desc { font-size: 0.85rem; font-weight: 500; color: var(--global-text-muted-color); line-height: 1.4; margin-bottom: 15px; display: -webkit-box; -webkit-line-clamp: 2; -webkit-box-orient: vertical; overflow: hidden; padding: 0 5px; }
  #recommendations .mentor-relation { font-size: 0.85rem; margin-bottom: 18px; line-height: 1.4; padding: 10px; background-color: rgba(128, 128, 128, 0.05); border-radius: 12px; width: 100%; }
  #recommendations .relation-label { color: var(--global-text-muted-color); font-weight: 500; font-size: 0.8rem; font-style: italic; }
  #recommendations .relation-value { color: var(--global-theme-color); font-weight: 700; text-transform: uppercase; font-size: 0.75rem; letter-spacing: 0px; display: block; margin-top: 4px; }
  #recommendations .mentor-badge { background-color: transparent; color: var(--global-theme-color); border: 1px solid var(--global-theme-color); font-weight: 600; padding: 5px 12px; border-radius: 30px; font-size: 0.7rem; margin-bottom: 20px; display: inline-block; }
  #recommendations .view-profile-btn { margin-top: auto; width: 100%; padding-top: 15px; border-top: 1px dashed var(--global-divider-color); }
  #recommendations .view-profile-btn span { font-size: 0.8rem; font-weight: 700; color: var(--global-text-muted-color); text-transform: uppercase; letter-spacing: 1px; transition: color 0.3s ease; }
  #recommendations .mentor-card:hover .view-profile-btn span { color: var(--global-theme-color); }
  #recommendations a.mentor-link-wrapper { text-decoration: none !important; color: inherit !important; }
</style>
<h2>Recommendations</h2>
<div class="rs-bar">
  <a href="{{ '/recommendations/' | relative_url }}">View all recommendations</a>
  <div class="rs-arrows">
    <button class="rs-arrow" id="rs-prev" type="button" aria-label="Previous">&#8592;</button>
    <button class="rs-arrow" id="rs-next" type="button" aria-label="Next">&#8594;</button>
  </div>
</div>
{% assign rs_categories = site.people | map: "category" | compact | uniq %}
<div class="rs-track" id="rs-track">
{% for category in rs_categories %}
{% for person in site.people %}
{% if person.category == category %}
<a href="{{ person.url | relative_url }}" class="mentor-link-wrapper rs-slide">
  <div class="mentor-card">
    <div class="mentor-img-wrapper">
      <img src="{{ person.img | relative_url }}" class="main-profile" alt="{{ person.title }}">
      {% if person.university_logo %}
      <img src="{{ person.university_logo | relative_url }}" class="inst-badge-logo" alt="Institution Logo" title="Institution">
      {% endif %}
    </div>
    <h3 class="mentor-name">{{ person.title }}</h3>
    <p class="mentor-desc">{{ person.description | split: '|' | first | strip }}</p>
    {% if person.relation %}
    <div class="mentor-relation">
      <span class="relation-label">Supervised me as:</span>
      <span class="relation-value">{{ person.relation }}</span>
    </div>
    {% endif %}
    {% if person.badge %}
    <div class="mentor-badge"><i class="fas fa-award mr-1"></i> {{ person.badge }}</div>
    {% endif %}
    <div class="view-profile-btn"><span>View Profile &rarr;</span></div>
  </div>
</a>
{% endif %}
{% endfor %}
{% endfor %}
</div>
<script>
  (function () {
    var track = document.getElementById('rs-track');
    var prev = document.getElementById('rs-prev');
    var next = document.getElementById('rs-next');
    if (!track || !prev || !next) return;
    var reduce = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
    function step(dir) {
      var slide = track.querySelector('.rs-slide');
      if (!slide) return;
      var gap = parseFloat(getComputedStyle(track).columnGap) || 20;
      var unit = slide.getBoundingClientRect().width + gap;
      var perPage = Math.max(1, Math.round(track.clientWidth / unit));
      track.scrollBy({ left: dir * perPage * unit, behavior: reduce ? 'auto' : 'smooth' });
    }
    function update() {
      prev.disabled = track.scrollLeft <= 2;
      next.disabled = track.scrollLeft + track.clientWidth >= track.scrollWidth - 2;
    }
    prev.addEventListener('click', function () { step(-1); });
    next.addEventListener('click', function () { step(1); });
    track.addEventListener('scroll', update, { passive: true });
    window.addEventListener('resize', update);
    update();
  })();
</script>
</section>

<!-- ============ 9. CONTACT ============ -->
<section class="za-section" id="contact">
  <div class="za-contact">
    <h2 style="border:0;margin-bottom:.6rem">Open to PhD and MSc opportunities in healthcare AI</h2>
    <p>I am applying to programmes across Europe. If our research interests align, I would be glad to hear from you.</p>
    <div class="za-actions" style="justify-content:center">
      <a class="za-btn primary" href="mailto:amini75zahra@gmail.com">Email me</a>
      <a class="za-btn primary" href="{{ 'assets/pdf/CV-ZahraAmini.pdf' | relative_url }}">Download CV</a>
    </div>
  </div>
</section>
