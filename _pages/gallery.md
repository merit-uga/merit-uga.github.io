---
layout: page
title: Gallery
permalink: /gallery/
description: Photos and images from the MERIT Lab
nav: true
nav_order: 5
images:
  venobox: true
---

<div class="gallery-shell">
  <nav class="gallery-index" aria-label="Gallery collections">
    {% for group in site.data.gallery %}
      <a class="gallery-index-link" href="#{{ group.id }}">
        <span>{{ group.title }}</span>
      </a>
    {% endfor %}
  </nav>

{% for group in site.data.gallery %}

<section class="gallery-group" id="{{ group.id }}" aria-labelledby="{{ group.id }}-title">
<header class="gallery-group-header">
<div>
<p class="gallery-group-number">Collection 0{{ forloop.index }}</p>
<h2 id="{{ group.id }}-title">{{ group.title }}</h2>
</div>
</header>

      <div class="gallery-grid">
        {% for image in group.images %}
          <figure class="gallery-item{% if image.featured %} gallery-item--featured{% endif %}">
            <a
              class="venobox"
              data-gall="{{ group.id }}"
              data-title="{{ image.caption | escape }}"
              href="{{ image.src | relative_url }}"
              aria-label="Open image: {{ image.caption | escape }}"
            >
              <img src="{{ image.src | relative_url }}" alt="{{ image.alt | escape }}" loading="lazy">
            </a>
            <figcaption>{{ image.caption }}</figcaption>
          </figure>
        {% endfor %}
      </div>
    </section>

{% endfor %}

</div>

<style>
  .gallery-shell {
    width: min(1180px, 100%);
    margin: 0 auto;
  }

  .gallery-index {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 0.75rem;
    margin-bottom: 3.5rem;
  }

  .gallery-index-link {
    display: flex;
    min-height: 76px;
    padding: 1rem 1.1rem;
    border: 1px solid var(--global-divider-color);
    border-left: 4px solid var(--global-theme-color);
    border-radius: 6px;
    color: var(--global-text-color);
    justify-content: center;
    text-decoration: none;
    transition:
      border-color 180ms ease,
      transform 180ms ease,
      box-shadow 180ms ease;
  }

  .gallery-index-link:hover,
  .gallery-index-link:focus-visible {
    border-color: var(--global-theme-color);
    color: var(--global-theme-color);
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
    transform: translateY(-2px);
  }

  .gallery-index-link span {
    font-weight: 700;
    line-height: 1.25;
  }

  .gallery-group {
    margin: 0 0 4.5rem;
    scroll-margin-top: 90px;
  }

  .gallery-group-header {
    margin-bottom: 1.35rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid var(--global-divider-color);
  }

  .gallery-group-header h2 {
    margin: 0;
    font-size: clamp(1.55rem, 2.4vw, 2.2rem);
    letter-spacing: 0;
  }

  .gallery-group-number {
    margin: 0 0 0.35rem;
    color: var(--global-theme-color);
    font-size: 0.76rem;
    font-weight: 800;
    letter-spacing: 0;
    text-transform: uppercase;
  }

  .gallery-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
  }

  .gallery-item {
    display: flex;
    min-width: 0;
    margin: 0;
    overflow: hidden;
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    background: var(--global-card-bg-color);
    flex-direction: column;
  }

  .gallery-item--featured {
    grid-column: span 2;
  }

  .gallery-item a {
    display: block;
    overflow: hidden;
    background: var(--global-bg-color);
  }

  .gallery-item img {
    display: block;
    width: 100%;
    aspect-ratio: 4 / 3;
    margin: 0;
    object-fit: cover;
    transition: transform 320ms ease;
  }

  .gallery-item--featured img {
    aspect-ratio: 2 / 1;
  }

  .gallery-item a:hover img,
  .gallery-item a:focus-visible img {
    transform: scale(1.025);
  }

  .gallery-item figcaption {
    display: flex;
    min-height: 52px;
    padding: 0.75rem 0.9rem;
    color: var(--global-text-color);
    font-size: 0.9rem;
    line-height: 1.45;
    align-items: center;
  }

  @media (max-width: 820px) {
    .gallery-grid {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }

  }

  @media (max-width: 540px) {
    .gallery-index,
    .gallery-grid {
      grid-template-columns: 1fr;
    }

    .gallery-item--featured {
      grid-column: auto;
    }

    .gallery-item--featured img {
      aspect-ratio: 4 / 3;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    .gallery-index-link,
    .gallery-item img {
      transition: none;
    }
  }
</style>
