---
layout: page
permalink: /awards/
title: Awards & Services
nav: true
nav_order: 3
_styles: |
  .awards-services-page {
    --awards-border: color-mix(in srgb, var(--global-divider-color) 86%, transparent);
    --awards-soft: color-mix(in srgb, var(--global-theme-color) 7%, transparent);
    --awards-soft-strong: color-mix(in srgb, var(--global-theme-color) 14%, transparent);
    --awards-muted: color-mix(in srgb, var(--global-text-color) 68%, var(--global-bg-color));
    --awards-text-soft: color-mix(in srgb, var(--global-text-color) 82%, var(--global-bg-color));
  }

  .awards-services-page .section-block + .section-block {
    margin-top: 2.7rem;
  }

  .awards-services-page .section-head {
    border-bottom: 1px solid var(--awards-border);
    margin-bottom: 1.1rem;
    padding-bottom: 0.75rem;
  }

  .awards-services-page .section-head h2 {
    font-size: 1.45rem;
    margin: 0;
  }

  .awards-services-page .award-list {
    display: grid;
    gap: 0.9rem;
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .awards-services-page .award-item {
    background:
      radial-gradient(circle at top right, var(--awards-soft-strong) 0, transparent 32%),
      linear-gradient(180deg, var(--awards-soft) 0%, transparent 100%);
    border: 1px solid var(--awards-border);
    border-radius: 1rem;
    min-height: 8.6rem;
    padding: 1rem 1rem 0.95rem;
    position: relative;
  }

  .awards-services-page .award-title {
    color: var(--global-text-color);
    font-size: 1rem;
    font-weight: 700;
    line-height: 1.4;
    margin: 0 4.8rem 0 0;
  }

  .awards-services-page .award-date {
    background: color-mix(in srgb, var(--global-theme-color) 12%, transparent);
    border: 1px solid color-mix(in srgb, var(--global-theme-color) 18%, transparent);
    border-radius: 999px;
    color: var(--awards-text-soft);
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0.04em;
    line-height: 1;
    padding: 0.38rem 0.62rem;
    position: absolute;
    right: 0.9rem;
    top: 0.9rem;
  }

  .awards-services-page .award-org {
    color: var(--awards-muted);
    font-size: 0.92rem;
    line-height: 1.55;
    margin: 0.58rem 0 0;
  }

  .awards-services-page .award-note {
    color: var(--awards-text-soft);
    font-size: 0.88rem;
    line-height: 1.55;
    margin: 0.28rem 0 0;
  }

  .awards-services-page .service-grid {
    display: grid;
    gap: 0.8rem;
  }

  .awards-services-page .service-item {
    align-items: start;
    background: linear-gradient(180deg, var(--awards-soft) 0%, transparent 100%);
    border: 1px solid var(--awards-border);
    border-radius: 1rem;
    display: grid;
    gap: 0.2rem 0.9rem;
    grid-template-columns: minmax(7rem, 8rem) minmax(0, 1fr);
    padding: 0.92rem 1rem;
  }

  .awards-services-page .service-title {
    color: var(--awards-muted);
    font-size: 0.84rem;
    font-weight: 700;
    letter-spacing: 0.05em;
    line-height: 1.3;
    margin: 0;
    text-transform: uppercase;
  }

  .awards-services-page .service-meta {
    color: var(--global-text-color);
    font-size: 0.96rem;
    line-height: 1.55;
    margin: 0;
  }

  .awards-services-page .service-meta small {
    color: var(--awards-muted);
    display: block;
    font-size: 0.88rem;
    margin-top: 0.12rem;
  }

  @media (max-width: 860px) {
    .awards-services-page .award-item {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 700px) {
    .awards-services-page .award-list {
      grid-template-columns: 1fr;
    }

    .awards-services-page .service-item {
      grid-template-columns: 1fr;
      gap: 0.28rem;
    }
  }
---

<div class="awards-services-page">
  <section class="section-block">
    <div class="section-head">
      <h2>Awards</h2>
    </div>

    <div class="award-list">
      <article class="award-item">
        <div class="award-date">05/2025</div>
        <p class="award-title">PLMW Scholarship</p>
        <p class="award-org">PLDI 2025</p>
      </article>

      <article class="award-item">
        <div class="award-date">04/2025</div>
        <p class="award-title">AsiaLLVM Student Travel Grant</p>
        <p class="award-org">LLVM</p>
      </article>

      <article class="award-item">
        <div class="award-date">10/2024</div>
        <p class="award-title">Outstanding Master's Thesis Award</p>
        <p class="award-note">信息工程大学优秀硕士论文奖</p>
        <p class="award-org">Information Engineering University</p>
      </article>

      <article class="award-item">
        <div class="award-date">12/2023</div>
        <p class="award-title">National Scholarship</p>
        <p class="award-note">国家奖学金</p>
        <p class="award-org">Ministry of Education of the People's Republic of China</p>
      </article>

      <article class="award-item">
        <div class="award-date">11/2023</div>
        <p class="award-title">First Class Academic Scholarship</p>
        <p class="award-org">Information Engineering University</p>
      </article>

      <article class="award-item">
        <div class="award-date">11/2022</div>
        <p class="award-title">Second Class Academic Scholarship</p>
        <p class="award-org">Information Engineering University</p>
      </article>

      <article class="award-item">
        <div class="award-date">11/2021</div>
        <p class="award-title">First Class Academic Scholarship</p>
        <p class="award-org">Information Engineering University</p>
      </article>
    </div>
  </section>

  <section class="section-block">
    <div class="section-head">
      <h2>Services</h2>
    </div>

    <div class="service-grid">
      <article class="service-item">
        <p class="service-title">Committee</p>
        <p class="service-meta"><a href="https://pact2025.github.io/">PACT 2025</a> Artifact Evaluation Committee</p>
      </article>

      <article class="service-item">
        <p class="service-title">Service</p>
        <p class="service-meta">Executive Committee Member<small>CCF Hunan University Student Chapter</small></p>
      </article>

      <article class="service-item">
        <p class="service-title">Teaching</p>
        <p class="service-meta">Teaching Assistant for Compiler Principles<small>School of Information Science and Engineering, Hunan University, 2024</small></p>
      </article>
    </div>
  </section>
</div>
