---
layout: page
permalink: /awards/
title: Awards & Services
nav: true
nav_order: 3
_styles: |
  .awards-services-page {
    --awards-border: color-mix(in srgb, var(--global-divider-color) 82%, transparent);
    --awards-soft: color-mix(in srgb, var(--global-theme-color) 8%, transparent);
    --awards-accent: color-mix(in srgb, var(--global-theme-color) 34%, transparent);
    --awards-muted: color-mix(in srgb, var(--global-text-color) 72%, var(--global-bg-color));
  }

  .awards-services-page .section-block + .section-block {
    margin-top: 3rem;
  }

  .awards-services-page .section-head {
    border-bottom: 1px solid var(--awards-border);
    margin-bottom: 1.4rem;
    padding-bottom: 0.8rem;
  }

  .awards-services-page .section-head h2 {
    font-size: 1.45rem;
    margin: 0;
  }

  .awards-services-page .award-list {
    display: grid;
    gap: 0.95rem;
  }

  .awards-services-page .award-item {
    align-items: start;
    column-gap: 1.1rem;
    display: grid;
    grid-template-columns: 6.3rem minmax(0, 1fr);
  }

  .awards-services-page .award-date {
    color: var(--awards-muted);
    font-size: 0.9rem;
    font-weight: 700;
    letter-spacing: 0.02em;
    line-height: 1.5;
    padding-top: 0.3rem;
  }

  .awards-services-page .award-content {
    background: linear-gradient(90deg, var(--awards-soft) 0%, transparent 26%);
    border-left: 2px solid var(--awards-accent);
    padding: 0.3rem 0 0.45rem 1rem;
  }

  .awards-services-page .award-title {
    font-size: 1rem;
    font-weight: 700;
    line-height: 1.45;
    margin: 0;
  }

  .awards-services-page .award-org {
    color: var(--awards-muted);
    font-size: 0.92rem;
    line-height: 1.55;
    margin: 0.18rem 0 0;
  }

  .awards-services-page .service-grid {
    display: grid;
    gap: 0.95rem;
  }

  .awards-services-page .service-item {
    background: linear-gradient(180deg, var(--awards-soft) 0%, transparent 100%);
    border: 1px solid var(--awards-border);
    border-radius: 1rem;
    padding: 1rem 1.05rem;
  }

  .awards-services-page .service-title {
    font-size: 1rem;
    font-weight: 700;
    line-height: 1.45;
    margin: 0;
  }

  .awards-services-page .service-meta {
    color: var(--awards-muted);
    font-size: 0.92rem;
    line-height: 1.55;
    margin: 0.2rem 0 0;
  }

  @media (max-width: 700px) {
    .awards-services-page .award-item {
      gap: 0.4rem;
      grid-template-columns: 1fr;
    }

    .awards-services-page .award-date {
      padding-top: 0;
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
        <div class="award-content">
          <p class="award-title">PLMW Scholarship</p>
          <p class="award-org">PLDI 2025</p>
        </div>
      </article>

      <article class="award-item">
        <div class="award-date">04/2025</div>
        <div class="award-content">
          <p class="award-title">AsiaLLVM Student Travel Grant</p>
          <p class="award-org">LLVM</p>
        </div>
      </article>

      <article class="award-item">
        <div class="award-date">10/2024</div>
        <div class="award-content">
          <p class="award-title">Outstanding Master's Thesis Award / 信息工程大学优秀硕士论文奖</p>
          <p class="award-org">Information Engineering University</p>
        </div>
      </article>

      <article class="award-item">
        <div class="award-date">12/2023</div>
        <div class="award-content">
          <p class="award-title">National Scholarship / 国家奖学金</p>
          <p class="award-org">Ministry of Education of the People's Republic of China</p>
        </div>
      </article>

      <article class="award-item">
        <div class="award-date">11/2023</div>
        <div class="award-content">
          <p class="award-title">First Class Academic Scholarship</p>
          <p class="award-org">Information Engineering University</p>
        </div>
      </article>

      <article class="award-item">
        <div class="award-date">11/2022</div>
        <div class="award-content">
          <p class="award-title">Second Class Academic Scholarship</p>
          <p class="award-org">Information Engineering University</p>
        </div>
      </article>

      <article class="award-item">
        <div class="award-date">11/2021</div>
        <div class="award-content">
          <p class="award-title">First Class Academic Scholarship</p>
          <p class="award-org">Information Engineering University</p>
        </div>
      </article>
    </div>
  </section>

  <section class="section-block">
    <div class="section-head">
      <h2>Services</h2>
    </div>

    <div class="service-grid">
      <article class="service-item">
        <p class="service-title"><a href="https://pact2025.github.io/">PACT 2025</a> Artifact Evaluation Committee</p>
      </article>

      <article class="service-item">
        <p class="service-title">Executive Committee Member</p>
        <p class="service-meta">CCF Hunan University Student Chapter</p>
      </article>

      <article class="service-item">
        <p class="service-title">Teaching Assistant for Compiler Principles</p>
        <p class="service-meta">School of Information Science and Engineering, Hunan University, 2024</p>
      </article>
    </div>
  </section>
</div>
