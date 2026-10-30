---
layout: page
title: News
permalink: /news/
description: Recent MERIT Lab awards, grants, papers, and milestones.
nav: true
nav_order: 4
---

<style>
  .news-page-shell {
    --news-blue: #003cff;
    --news-red: #d00000;
    --news-green: #198754;
    --news-gold: #b8860b;
    --news-text: var(--global-text-color);
    --news-muted: #4f5965;
    --news-line: rgba(23, 23, 23, 0.12);
    margin-top: 0.5rem;
  }

  html[data-theme='dark'] .news-page-shell {
    --news-blue: #7fa2ff;
    --news-red: #ff6f6f;
    --news-green: #4ade80;
    --news-gold: #ffd166;
    --news-muted: #cbd3dc;
    --news-line: rgba(255, 255, 255, 0.14);
  }

  .news-hero {
    position: relative;
    min-height: 280px;
    overflow: hidden;
    margin-bottom: 2.5rem;
    padding: 2rem;
    border-radius: 8px;
    background: url(/assets/img/gallery/lab-equipment-6.jpg) center / cover;
    color: #ffffff;
    animation: news-hero-drift 18s ease-in-out infinite alternate;
  }

  .news-hero::before {
    content: "";
    position: absolute;
    inset: 0;
    background: linear-gradient(90deg, rgba(0, 0, 0, 0.78), rgba(0, 0, 0, 0.24));
  }

  .news-hero-content {
    position: relative;
    z-index: 1;
    max-width: 650px;
  }

  .news-hero h2 {
    margin: 0 0 0.65rem;
    color: #ffffff;
    font-size: clamp(1.8rem, 4vw, 2.7rem);
    font-weight: 800;
  }

  .news-hero p {
    margin: 0;
    color: rgba(255, 255, 255, 0.92);
    font-size: 1.05rem;
    line-height: 1.55;
  }

  .news-archive {
    border-top: 1px solid var(--news-line);
  }

  .news-year {
    display: grid;
    grid-template-columns: 90px minmax(0, 1fr);
    gap: 1.4rem;
    margin: 0;
    padding: 1.6rem 0;
    border-bottom: 1px solid var(--news-line);
    animation: news-rise 0.65s ease both;
  }

  .news-year:nth-of-type(2) {
    animation-delay: 0.08s;
  }

  .news-year:nth-of-type(3) {
    animation-delay: 0.16s;
  }

  .news-year:nth-of-type(n + 4) {
    animation-delay: 0.24s;
  }

  .news-year h2 {
    margin: 0;
    color: var(--news-blue);
    font-size: 1.35rem;
    font-weight: 800;
    line-height: 1.2;
  }

  .news-year ul {
    margin: 0;
    padding-left: 1.8rem;
  }

  .news-year li {
    margin-bottom: 0.35rem;
    color: var(--news-text);
    font-size: 0.95rem;
    line-height: 1.28;
    transition: transform 180ms ease;
  }

  .news-year li:hover {
    transform: translateX(5px);
  }

  .news-label {
    color: var(--news-red);
    font-weight: 800;
  }

  .news-label-award {
    color: var(--news-green);
  }

  .news-label-service {
    color: var(--news-gold);
  }

  .news-date-inline {
    color: var(--news-muted);
    white-space: nowrap;
  }

  @keyframes news-hero-drift {
    from {
      background-position: 48% 50%;
    }
    to {
      background-position: 56% 50%;
    }
  }

  @keyframes news-rise {
    from {
      opacity: 0;
      transform: translateY(18px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @media (max-width: 640px) {
    .news-hero {
      min-height: 240px;
      padding: 1.5rem;
    }

    .news-year {
      grid-template-columns: 1fr;
      gap: 0.75rem;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    .news-hero,
    .news-year {
      animation: none;
    }

    .news-year li {
      transition: none;
    }
  }
</style>

<div class='news-page-shell'>
  <section class='news-hero'>
    <div class='news-hero-content'>
      <h2>Lab Momentum</h2>
      <p>Awards, grants, papers, and milestones from the MERIT Lab research community.</p>
    </div>
  </section>

  <div class='news-archive'>
  <section class='news-year'>
    <h2>2026</h2>
    <ul>
      <li><span class='news-label'>[Event]</span> MERIT Lab conducted a summer camp. <span class='news-date-inline'>(2026/07)</span></li>
      <li><span class='news-label'>[Media]</span> The Autoinspector robotic-inspection framework was accepted to ASME MSEC 2026. <span class='news-date-inline'>(2026/05)</span></li>
      <li><span class='news-label news-label-award'>[Award]</span> The team received a $600K NSF CICI grant for a manufacturing-security living lab. <span class='news-date-inline'>(2026/05)</span></li>
      <li><span class='news-label news-label-award'>[Award]</span> PhD student Wuyang Chen was named a Finalist for the IISE M&amp;D Best Student Paper Award. <span class='news-date-inline'>(2026/05)</span></li>
    </ul>
  </section>

  <section class='news-year'>
    <h2>2025</h2>
    <ul>
      <li><span class='news-label news-label-award'>[Award]</span> MERIT received a Honda climate-smart manufacturing project. <span class='news-date-inline'>(2025/09)</span></li>
      <li><span class='news-label news-label-service'>[Service]</span> Dr. Sun began service as Associate Editor of ASME JCISE. <span class='news-date-inline'>(2025/09)</span></li>
      <li><span class='news-label news-label-service'>[Service]</span> MERIT organized the 2nd Convergent Safety Symposium. <span class='news-date-inline'>(2025/09)</span></li>
      <li><span class='news-label news-label-service'>[Service]</span> Dr. Sun served as Chair of the INFORMS QSR Section. <span class='news-date-inline'>(2025/09)</span></li>
    </ul>
  </section>

  <section class='news-year'>
    <h2>2024</h2>
    <ul>
      <li><span class='news-label news-label-service'>[Service]</span> Dr. Sun began service as Associate Editor of IISE Transactions. <span class='news-date-inline'>(2024/10)</span></li>
      <li><span class='news-label news-label-service'>[Service]</span> MERIT organized the 1st Convergent Safety Symposium with experts across UGA, UC San Diego, and UT Austin. <span class='news-date-inline'>(2024/10)</span></li>
      <li><span class='news-label'>[Media]</span> The lab celebrated two IISE Transactions Feature Papers. <span class='news-date-inline'>(2024/10)</span></li>
    </ul>
  </section>

  <section class='news-year'>
    <h2>2023</h2>
    <ul>
      <li><span class='news-label'>[Event]</span> Dr. Sun moved to the University of Georgia and launched the MERIT Lab. <span class='news-date-inline'>(2023/08)</span></li>
      <li><span class='news-label news-label-award'>[Award]</span> Dr. Sun received the SME Outstanding Young Manufacturing Engineer Award. <span class='news-date-inline'>(2023/08)</span></li>
      <li><span class='news-label news-label-award'>[Award]</span> Dr. Sun received the University at Buffalo Exceptional Scholar - Young Investigator Award. <span class='news-date-inline'>(2023/08)</span></li>
      <li><span class='news-label news-label-award'>[Award]</span> The team was awarded the $566K NSF Ethical Industry 4.0 project. <span class='news-date-inline'>(2023/08)</span></li>
    </ul>
  </section>

  <section class='news-year'>
    <h2>2022</h2>
    <ul>
      <li><span class='news-label news-label-award'>[Award]</span> The team won 1st place and $6,000 at the University at Buffalo Agrusa Innovation Competition for an interactive digital twin in cyber manufacturing, with work published at ACM SenSys. <span class='news-date-inline'>(2022/04)</span></li>
    </ul>
  </section>

  <section class='news-year'>
    <h2>2021</h2>
    <ul>
      <li><span class='news-label news-label-award'>[Award]</span> MERIT launched the STREAM platform under a $2.33M NSF Future Manufacturing Research Grant for multi-stage distributed future manufacturing. <span class='news-date-inline'>(2021/09)</span></li>
    </ul>
  </section>

  <section class='news-year'>
    <h2>2018</h2>
    <ul>
      <li><span class='news-label'>[Media]</span> The team published a foundational cyber-coordinated simulation framework for multi-stage additive manufacturing at IEEE CASE, where the paper was selected as a Prominent Paper. <span class='news-date-inline'>(2018/08)</span></li>
    </ul>
  </section>

  <section class='news-year'>
    <h2>2017</h2>
    <ul>
      <li><span class='news-label'>[Event]</span> Dr. Sun joined the University at Buffalo as an Assistant Professor, launching the research program that became the MERIT Lab. <span class='news-date-inline'>(2017/08)</span></li>
    </ul>
  </section>
  </div>
</div>
