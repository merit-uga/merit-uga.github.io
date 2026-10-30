---
layout: page
permalink: /teaching/
title: Join Us
description: Openings and teaching in MERIT.
nav: true
nav_order: 6
---

<!-- prettier-ignore-start -->

<style>
  .join-shell {
    --dssi-line: rgba(23, 23, 23, 0.12);
    --dssi-muted: #5c6670;
  }

  html[data-theme="dark"] .join-shell {
    --dssi-line: rgba(255, 255, 255, 0.14);
    --dssi-muted: #c5ccd3;
  }

  .join-hero {
    display: grid;
    grid-template-columns: minmax(0, 1.1fr) minmax(280px, 0.9fr);
    gap: 1.6rem;
    align-items: stretch;
    margin-bottom: 2.2rem;
  }

  .join-copy {
    display: flex;
    flex-direction: column;
    justify-content: center;
    min-height: 330px;
    padding: 2rem;
    border: 1px solid var(--dssi-line);
    border-radius: 8px;
    background:
      linear-gradient(135deg, rgba(186, 12, 47, 0.12), transparent 42%),
      var(--global-card-bg-color);
    animation: join-rise 0.7s ease both;
  }

  .join-copy h2 {
    margin-top: 0;
    color: var(--global-text-color);
    font-size: clamp(1.9rem, 4vw, 2.7rem);
    font-weight: 800;
  }

  .join-visual {
    min-height: 330px;
    overflow: hidden;
    border: 1px solid var(--dssi-line);
    border-radius: 8px;
    background: url("{{ '/assets/img/gallery/1000007090.jpg' | relative_url }}") center / cover;
    animation: join-float 7s ease-in-out infinite;
  }

  .join-cards {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 0.9rem;
    margin: 1.6rem 0 2.2rem;
  }

  .join-card {
    padding: 1rem;
    border: 1px solid var(--dssi-line);
    border-radius: 8px;
    background: var(--global-card-bg-color);
    animation: join-rise 0.7s ease both;
  }

  .join-card:nth-child(2) {
    animation-delay: 0.08s;
  }

  .join-card:nth-child(3) {
    animation-delay: 0.16s;
  }

  .join-card i {
    color: var(--global-theme-color);
    font-size: 1.4rem;
  }

  .join-card h3 {
    margin: 0.75rem 0 0.45rem;
    color: var(--global-text-color);
    font-size: 1.05rem;
    font-weight: 800;
  }

  .join-card p {
    margin: 0;
    color: var(--dssi-muted);
    line-height: 1.55;
  }

  .join-email {
    font-weight: 800;
  }

  .teaching-section {
    margin-top: 2.4rem;
    padding-top: 2.4rem;
    border-top: 1px solid var(--dssi-line);
  }

  .teaching-head {
    display: flex;
    align-items: end;
    justify-content: space-between;
    gap: 1.2rem;
    margin-bottom: 1rem;
  }

  .teaching-head h2 {
    margin: 0;
    color: var(--global-text-color);
    font-size: clamp(1.55rem, 3vw, 2.15rem);
    font-weight: 800;
  }

  .teaching-kicker {
    color: var(--global-theme-color);
    font-size: 0.78rem;
    font-weight: 800;
    text-transform: uppercase;
  }

  .course-marquee {
    overflow: hidden;
    padding: 0.35rem 0;
    -webkit-mask-image: linear-gradient(90deg, transparent, #000 7%, #000 93%, transparent);
    mask-image: linear-gradient(90deg, transparent, #000 7%, #000 93%, transparent);
  }

  .course-track {
    display: flex;
    width: max-content;
    gap: 0.9rem;
    animation: course-slide 22s linear infinite;
    will-change: transform;
  }

  .course-marquee:hover .course-track {
    animation-play-state: paused;
  }

  .course-card {
    flex: 0 0 310px;
    padding: 1rem;
    border: 1px solid var(--dssi-line);
    border-radius: 8px;
    background:
      linear-gradient(135deg, rgba(186, 12, 47, 0.1), transparent 45%),
      var(--global-card-bg-color);
  }

  .course-card h3 {
    margin: 0.5rem 0;
    color: var(--global-text-color);
    font-size: 1.05rem;
    font-weight: 800;
    line-height: 1.3;
  }

  .course-icon-row,
  .course-rating {
    display: flex;
    gap: 0.35rem;
    color: var(--global-theme-color);
  }

  .course-rating {
    margin-top: 0.8rem;
    color: #ba0c2f;
  }

  .course-meta {
    color: var(--dssi-muted);
    font-size: 0.9rem;
    line-height: 1.45;
  }

  @keyframes join-rise {
    from {
      opacity: 0;
      transform: translateY(16px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @keyframes join-float {
    0%,
    100% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-8px);
    }
  }

  @keyframes course-slide {
    from {
      transform: translateX(0);
    }
    to {
      transform: translateX(calc(-50% - 0.45rem));
    }
  }

  @media (max-width: 820px) {
    .join-hero,
    .join-cards,
    .teaching-head {
      grid-template-columns: 1fr;
    }

    .teaching-head {
      display: block;
    }

    .course-card {
      flex-basis: min(78vw, 310px);
    }
  }
</style>

<div class="join-shell">
  <section class="join-hero">
    <div class="join-copy">
      <h2>We Are Recruiting</h2>
      <p>
        MERIT Lab is recruiting motivated researchers interested in
        <strong>trustworthy AI for manufacturing, smart and additive manufacturing, privacy-preserving machine learning, and safe human-robot collaboration.</strong>
      </p>
    </div>
    <div class="join-visual" aria-hidden="true"></div>
  </section>

  <div class="join-cards">
    <article class="join-card">
      <i class="fa-solid fa-user-graduate" aria-hidden="true"></i>
      <h3>PhD Students</h3>
      <p><a class='join-email' href='mailto:hongyuesun@uga.edu'>Email</a> Dr. Sun with a CV, transcripts, and a short statement of research interests.</p>
    </article>

    <article class="join-card">
      <i class="fa-solid fa-laptop-code" aria-hidden="true"></i>
      <h3>UGA Undergraduates</h3>
      <p><a class='join-email' href='mailto:hongyuesun@uga.edu'>Email</a> Dr. Sun about year-round opportunities in robotics, digital twins, AI, privacy, and manufacturing.</p>
    </article>

    <article class="join-card">
      <i class="fa-solid fa-flask" aria-hidden="true"></i>
      <h3>Postdocs & Visitors</h3>
      <p><a class='join-email' href='mailto:hongyuesun@uga.edu'>Email</a> Dr. Sun with a CV and research statement describing fit with current MERIT projects.</p>
    </article>
  </div>


  <section class="teaching-section">
    <div class="teaching-head">
      <div>
        <div class="teaching-kicker">Teaching</div>
        <h2>Courses and Learning Experiences</h2>
      </div>
    </div>

    <div class="course-marquee" aria-label="MERIT teaching courses">
      <div class="course-track">
        {% for copy in (1..2) %}
          <article class="course-card">
            <div class="course-icon-row" aria-hidden="true">
              <i class="fa-solid fa-robot"></i>
              <i class="fa-solid fa-brain"></i>
              <i class="fa-solid fa-gears"></i>
            </div>
            <h3>ENGR 8990 - AI-Agents Meet Mechanical Engineering</h3>
            <div class="course-meta">UGA, Fall 2025</div>
            <div class="course-rating" aria-label="Class rating icons">
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-regular fa-star"></i>
            </div>
          </article>
          <article class="course-card">
            <div class="course-icon-row" aria-hidden="true">
              <i class="fa-solid fa-chart-line"></i>
              <i class="fa-solid fa-magnifying-glass-chart"></i>
              <i class="fa-solid fa-industry"></i>
            </div>
            <h3>ENGR 4670 / 6670 - Quality Engineering</h3>
            <div class="course-meta">UGA, Fall 2025</div>
            <div class="course-rating" aria-label="Class rating icons">
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-regular fa-star"></i>
            </div>
          </article>
          <article class="course-card">
            <div class="course-icon-row" aria-hidden="true">
              <i class="fa-solid fa-sliders"></i>
              <i class="fa-solid fa-wave-square"></i>
              <i class="fa-solid fa-circle-check"></i>
            </div>
            <h3>ENGR 8990 - Advanced Quality Control</h3>
            <div class="course-meta">UGA, Fall 2024</div>
            <div class="course-rating" aria-label="Class rating icons">
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-regular fa-star"></i>
            </div>
          </article>
          <article class="course-card">
            <div class="course-icon-row" aria-hidden="true">
              <i class="fa-solid fa-diagram-project"></i>
              <i class="fa-solid fa-screwdriver-wrench"></i>
              <i class="fa-solid fa-gauge-high"></i>
            </div>
            <h3>MCHE 4440 - Design and Control of Production Systems</h3>
            <div class="course-meta">UGA, Fall 2023 and Fall 2024</div>
            <div class="course-rating" aria-label="Class rating icons">
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-solid fa-star"></i>
              <i class="fa-regular fa-star"></i>
            </div>
          </article>
        {% endfor %}
      </div>
    </div>

    <p>
      Earlier courses at the University at Buffalo include Statistical Machine Learning for Engineers, Advanced Quality Control, Manufacturing Data Analytics,
      Statistics for Engineers, and Facility Design and Materials Handling.
    </p>
  </section>
</div>

<!-- prettier-ignore-end -->
