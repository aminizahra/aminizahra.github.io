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
  .rcs-bar { display: flex; justify-content: space-between; align-items: center; margin-bottom: .9rem; font-size: .95rem; }
  .rcs-arrows { display: flex; gap: .4rem; }
  .rcs-arrow { width: 2rem; height: 2rem; padding: 0; border: 1px solid var(--global-divider-color); border-radius: 50%; background: transparent; color: var(--global-text-color); cursor: pointer; line-height: 1; }
  .rcs-arrow:hover:not(:disabled) { border-color: var(--global-theme-color); color: var(--global-theme-color); }
  .rcs-arrow:focus-visible { outline: 2px solid var(--global-theme-color); outline-offset: 2px; }
  .rcs-arrow:disabled { opacity: .35; cursor: default; }
  .rcs-track { display: flex; gap: 1rem; overflow-x: auto; scroll-snap-type: x mandatory; scrollbar-width: none; padding: .2rem 0 .4rem; }
  .rcs-track::-webkit-scrollbar { display: none; }
  .rcs-card { flex: 0 0 calc((100% - 2rem) / 3); min-width: 250px; scroll-snap-align: start; display: flex; flex-direction: column; align-items: center; text-align: center; padding: 1.5rem 1rem 0; border: 1px solid var(--global-divider-color); border-radius: 14px; background: var(--global-card-bg-color); }
  .rcs-avatar { position: relative; width: 96px; height: 96px; margin-bottom: 1rem; border-radius: 50%; box-shadow: 0 0 0 3px var(--global-theme-color); display: flex; align-items: center; justify-content: center; font-weight: 600; font-size: 1.4rem; color: var(--global-text-color-light); background: var(--global-bg-color); }
  .rcs-photo { position: absolute; inset: 0; width: 100%; height: 100%; object-fit: cover; border-radius: 50%; }
  .rcs-logo { position: absolute; right: -4px; bottom: -4px; width: 30px; height: 30px; padding: 2px; object-fit: contain; border-radius: 50%; background: #fff; border: 1px solid var(--global-divider-color); }
  .rcs-name { font-size: 1.05rem; font-weight: 600; margin: 0 0 .3rem; }
  .rcs-title { font-size: .85rem; line-height: 1.35; min-height: 2.7em; margin: 0 0 .9rem; }
  .rcs-as { width: 100%; min-height: 3.6rem; display: flex; flex-direction: column; justify-content: center; gap: .15rem; padding: .55rem .6rem; border-radius: 8px; background: rgba(127, 127, 127, .09); }
  .rcs-as em { font-size: .8rem; }
  .rcs-as strong { font-size: .72rem; font-weight: 500; letter-spacing: .04em; text-transform: uppercase; color: var(--global-theme-color); }
  .rcs-letter { display: inline-flex; align-items: center; gap: .4rem; margin: .9rem 0 1.1rem; padding: .25rem .85rem; font-size: .75rem; border: 1px solid var(--global-theme-color); border-radius: 999px; color: var(--global-theme-color); text-decoration: none; }
  .rcs-letter:hover { background: var(--global-theme-color); color: var(--global-bg-color); text-decoration: none; }
  .rcs-profile { width: 100%; margin-top: auto; padding: .85rem 0; border-top: 1px dashed var(--global-divider-color); font-size: .75rem; font-weight: 600; letter-spacing: .1em; text-transform: uppercase; color: var(--global-text-color); text-decoration: none; }
  .rcs-profile:hover { color: var(--global-theme-color); text-decoration: none; }
  @media (max-width: 768px) { .rcs-card { flex-basis: 82%; } }
</style>
<h2>Recommendations</h2>
<div class="rcs-bar">
  <a href="{{ '/recommendations/' | relative_url }}">View all recommendations</a>
  <div class="rcs-arrows">
    <button class="rcs-arrow" id="rcs-prev" type="button" aria-label="Previous">&#8592;</button>
    <button class="rcs-arrow" id="rcs-next" type="button" aria-label="Next">&#8594;</button>
  </div>
</div>
<!-- TODO for every card below:
     1. photo:  src of <img class="rcs-photo">  (same image your Recommendations page uses)
     2. logo:   src of <img class="rcs-logo">   (institution logo)
     3. letter: href of <a class="rcs-letter">  (direct letter URL; it opens the Recommendations page for now)
     If a photo or logo file is missing, it is hidden (initials show instead). -->
<div class="rcs-track" id="rcs-track">
  <div class="rcs-card">
    <div class="rcs-avatar"><span>AP</span><img class="rcs-photo" src="{{ '/assets/img/people/ahmad-pouramini.jpg' | relative_url }}" alt="Dr. Ahmad Pouramini" onerror="this.remove()"><img class="rcs-logo" src="{{ '/assets/img/logos/sirjan.png' | relative_url }}" alt="Institution logo" onerror="this.remove()"></div>
    <h3 class="rcs-name">Dr. Ahmad Pouramini</h3>
    <p class="rcs-title">Assistant Professor at Sirjan University of Technology</p>
    <div class="rcs-as"><em>Supervised me as:</em><strong>Teaching Assistant &amp; Student</strong></div>
    <a class="rcs-letter" href="{{ '/recommendations/' | relative_url }}"><i class="fa-solid fa-award"></i> Recommendation Letter</a>
    <a class="rcs-profile" href="{{ '/people/ahmad-pouramini/' | relative_url }}">View Profile &rarr;</a>
  </div>
  <div class="rcs-card">
    <div class="rcs-avatar"><span>AS</span><img class="rcs-photo" src="{{ '/assets/img/people/amir-salarpour.jpg' | relative_url }}" alt="Dr. Amir Salarpour" onerror="this.remove()"><img class="rcs-logo" src="{{ '/assets/img/logos/clemson.png' | relative_url }}" alt="Institution logo" onerror="this.remove()"></div>
    <h3 class="rcs-name">Dr. Amir Salarpour</h3>
    <p class="rcs-title">PostDoctoral Researcher at Clemson University</p>
    <div class="rcs-as"><em>Supervised me as:</em><strong>Research Assistant, Teaching Assistant &amp; Thesis Student</strong></div>
    <a class="rcs-letter" href="{{ '/recommendations/' | relative_url }}"><i class="fa-solid fa-award"></i> Recommendation Letter</a>
    <a class="rcs-profile" href="{{ '/people/amir-salarpour/' | relative_url }}">View Profile &rarr;</a>
  </div>
  <div class="rcs-card">
    <div class="rcs-avatar"><span>SK</span><img class="rcs-photo" src="{{ '/assets/img/people/somayeh-khajehasani.jpg' | relative_url }}" alt="Somayeh Khajehasani" onerror="this.remove()"><img class="rcs-logo" src="{{ '/assets/img/logos/sirjan.png' | relative_url }}" alt="Institution logo" onerror="this.remove()"></div>
    <h3 class="rcs-name">Somayeh Khajehasani</h3>
    <p class="rcs-title">Lecturer at Sirjan University of Technology</p>
    <div class="rcs-as"><em>Supervised me as:</em><strong>Teaching Assistant &amp; Student</strong></div>
    <a class="rcs-letter" href="{{ '/recommendations/' | relative_url }}"><i class="fa-solid fa-award"></i> Recommendation Letter</a>
    <a class="rcs-profile" href="{{ '/people/somayeh-khajehasani/' | relative_url }}">View Profile &rarr;</a>
  </div>
  <div class="rcs-card">
    <div class="rcs-avatar"><span>HS</span><img class="rcs-photo" src="{{ '/assets/img/people/hossein-sameti.jpg' | relative_url }}" alt="Dr. Hossein Sameti" onerror="this.remove()"><img class="rcs-logo" src="{{ '/assets/img/logos/sharif.png' | relative_url }}" alt="Institution logo" onerror="this.remove()"></div>
    <h3 class="rcs-name">Dr. Hossein Sameti</h3>
    <p class="rcs-title">Associate Professor at Sharif University of Technology</p>
    <div class="rcs-as"><em>Supervised me as:</em><strong>Colleague &amp; AI Instructor</strong></div>
    <a class="rcs-letter" href="{{ '/recommendations/' | relative_url }}"><i class="fa-solid fa-award"></i> Recommendation Letter</a>
    <a class="rcs-profile" href="{{ '/people/hossein-sameti/' | relative_url }}">View Profile &rarr;</a>
  </div>
  <div class="rcs-card">
    <div class="rcs-avatar"><span>MA</span><img class="rcs-photo" src="{{ '/assets/img/people/mahmoud-alipour.jpg' | relative_url }}" alt="Mahmoud Alipour" onerror="this.remove()"><img class="rcs-logo" src="{{ '/assets/img/logos/jetco.png' | relative_url }}" alt="Institution logo" onerror="this.remove()"></div>
    <h3 class="rcs-name">Mahmoud Alipour</h3>
    <p class="rcs-title">Head of ADAS Group at JETCO</p>
    <div class="rcs-as"><em>Supervised me as:</em><strong>Teaching Assistant</strong></div>
    <a class="rcs-letter" href="{{ '/recommendations/' | relative_url }}"><i class="fa-solid fa-award"></i> Recommendation Letter</a>
    <a class="rcs-profile" href="{{ '/people/mahmoud-alipour/' | relative_url }}">View Profile &rarr;</a>
  </div>
  <div class="rcs-card">
    <div class="rcs-avatar"><span>PH</span><img class="rcs-photo" src="{{ '/assets/img/people/pooria-haddad.jpg' | relative_url }}" alt="Pooria Haddad" onerror="this.remove()"><img class="rcs-logo" src="{{ '/assets/img/logos/filoger.png' | relative_url }}" alt="Institution logo" onerror="this.remove()"></div>
    <h3 class="rcs-name">Pooria Haddad</h3>
    <p class="rcs-title">Head of Filoger Artificial Intelligence Company</p>
    <div class="rcs-as"><em>Supervised me as:</em><strong>Lecturer &amp; AI Mentor</strong></div>
    <a class="rcs-letter" href="{{ '/recommendations/' | relative_url }}"><i class="fa-solid fa-award"></i> Work Experience Certificate</a>
    <a class="rcs-profile" href="{{ '/people/pooria-haddad-filoger/' | relative_url }}">View Profile &rarr;</a>
  </div>
</div>
<script>
  (function () {
    var track = document.getElementById('rcs-track');
    var prev = document.getElementById('rcs-prev');
    var next = document.getElementById('rcs-next');
    if (!track || !prev || !next) return;
    var reduce = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
    function step(dir) {
      var card = track.querySelector('.rcs-card');
      var w = card ? card.getBoundingClientRect().width + 16 : 300;
      track.scrollBy({ left: dir * w, behavior: reduce ? 'auto' : 'smooth' });
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
