---
layout: default
title: "GiHoon Kim"
permalink: /
description: "GiHoon Kim is a Ph.D. student at Seoul National University researching controllable generation with diffusion models."
---

<main id="main-content" class="site-page home-page">
  <section class="hero" aria-labelledby="home-title">
    <div class="hero__copy">
      <p class="eyebrow">Researcher in generative AI <span aria-hidden="true">/</span> Seoul, Korea</p>
      <h1 id="home-title">GiHoon <em>Kim.</em></h1>
      <p class="hero__role">Ph.D. student in Data Science<br>Seoul National University</p>
      <p class="hero__lead">I study <strong>controllable generation with diffusion models</strong>—how to adapt them without distributional drift, and how to guide denoising using the frequency content of intermediate samples.</p>
      <p class="hero__advisor">Learning Adaptation Algorithm Lab · Advised by Prof. Taesup Kim</p>
      <div class="hero__actions">
        <a class="action-link action-link--solid" href="{{ '/publications/' | relative_url }}">Explore publications</a>
        <a class="action-link action-link--outline" href="{{ '/files/Gihoon_CV.pdf' | relative_url }}" download>Download CV <span class="file-tag">PDF</span></a>
      </div>
      <div class="hero__profiles" aria-label="Research profiles">
        <a href="mailto:gihoon.kim@snu.ac.kr">Email</a>
        <a href="{{ site.author.googlescholar }}" target="_blank" rel="noopener noreferrer">Google Scholar</a>
        <a href="https://github.com/{{ site.author.github }}" target="_blank" rel="noopener noreferrer">GitHub</a>
        <a href="https://www.linkedin.com/in/{{ site.author.linkedin }}" target="_blank" rel="noopener noreferrer">LinkedIn</a>
      </div>
    </div>
    <figure class="hero__portrait">
      <div class="hero__portrait-frame">
        <img src="{{ '/images/profile.webp' | relative_url }}" alt="Portrait of GiHoon Kim" width="354" height="472" fetchpriority="high">
      </div>
      <figcaption>Researching diffusion models<br>at Seoul National University.</figcaption>
    </figure>
  </section>

  <section class="latest-note" aria-label="Latest research news">
    <span class="latest-note__label">Latest</span>
    <p><strong>2026</strong> · <em>Preserve and Personalize</em> appeared at ICLR; two new preprints explore spectral guidance and multimodal assistant safety.</p>
    <a href="{{ '/publications/' | relative_url }}">See all work</a>
  </section>

  <section id="research" class="content-section research-section" aria-labelledby="research-title">
    <div class="section-heading">
      <p class="eyebrow">What I work on</p>
      <h2 id="research-title">Research with control at its core.</h2>
      <p>My work connects the behavior of generative models to practical methods for directing what they produce.</p>
    </div>
    <div class="research-grid">
      <article class="research-card">
        <span class="research-card__marker" aria-hidden="true"></span>
        <h3>Preserving distributions</h3>
        <p>Training objectives for personalized text-to-image models that limit drift from the original model.</p>
      </article>
      <article class="research-card">
        <span class="research-card__marker" aria-hidden="true"></span>
        <h3>Guiding generation</h3>
        <p>Inference-time methods that use spectral information in intermediate samples to steer denoising.</p>
      </article>
      <article class="research-card">
        <span class="research-card__marker" aria-hidden="true"></span>
        <h3>Beyond images</h3>
        <p>Applications spanning 3D facial animation and evaluations of multimodal AI systems.</p>
      </article>
    </div>
  </section>

  <section class="content-section featured-section" aria-labelledby="featured-title">
    <div class="section-heading section-heading--row">
      <div>
        <p class="eyebrow">Selected work</p>
        <h2 id="featured-title">Research highlights</h2>
      </div>
      <a class="text-link" href="{{ '/publications/' | relative_url }}">View all publications</a>
    </div>
    <div class="publication-list">
      {% assign featured = site.publications | where: "featured", true | sort: "date" | reverse %}
      {% for post in featured %}
        {% include archive-single-publication.html %}
      {% endfor %}
    </div>
  </section>

  <section class="content-section background-section" aria-labelledby="background-title">
    <div class="section-heading">
      <p class="eyebrow">Background</p>
      <h2 id="background-title">The path behind the work</h2>
    </div>
    <div class="background-grid">
      <div>
        <h3>Education</h3>
        <ol class="timeline-list">
          <li><span>2024 — Present</span><strong>Ph.D. in Data Science</strong><small>Seoul National University · Learning Adaptation Algorithm Lab</small></li>
          <li><span>2021 — 2023</span><strong>M.S. in Culture Technology</strong><small>KAIST · Visual Media Lab</small></li>
          <li><span>2015 — 2021</span><strong>B.S. in Computer Science &amp; Electronic Engineering</strong><small>Handong Global University</small></li>
        </ol>
      </div>
      <div>
        <h3>Experience &amp; recognition</h3>
        <ol class="timeline-list">
          <li><span>2025 — 2026</span><strong>NRF Research Encouragement Grant</strong><small>Principal Investigator · National Research Foundation of Korea</small></li>
          <li><span>2022 — 2023</span><strong>Research Intern, Image/Vision</strong><small>NAVER CLOVA (Cloud) · 3D-aware hairstyle transfer</small></li>
          <li><span>2020</span><strong>Undergraduate Paper Award</strong><small>Institute of Control, Robotics and Systems (ICROS)</small></li>
        </ol>
      </div>
    </div>
  </section>

  <section id="contact" class="contact-panel" aria-labelledby="contact-title">
    <div>
      <p class="eyebrow">Get in touch</p>
      <h2 id="contact-title">Have a research idea<br>to explore together?</h2>
      <p>I welcome conversations about generative modeling, controllable generation, and collaboration.</p>
    </div>
    <a class="action-link action-link--light" href="mailto:gihoon.kim@snu.ac.kr">gihoon.kim@snu.ac.kr</a>
  </section>
</main>
