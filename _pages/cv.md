---
layout: default
title: CV
permalink: /cv/
---

<div
  class="cv-pdf-viewer"
  data-english-pdf="{{ '/assets/pdf/cv.pdf' | relative_url }}"
  data-chinese-pdf="{{ '/assets/pdf/resume_chinese.pdf' | relative_url }}"
>
  <div class="cv-pdf-viewer__header">
    <h1 class="cv-pdf-viewer__title">Curriculum Vitae</h1>
    <button class="cv-pdf-viewer__language" type="button" aria-label="Switch to Chinese CV">中文版</button>
  </div>

  <iframe
    class="cv-pdf-viewer__frame"
    src="{{ '/assets/pdf/cv.pdf' | relative_url }}#view=FitH"
    title="English CV"
  ></iframe>

  <p class="cv-pdf-viewer__fallback">
    If the PDF does not appear, open the
    <a class="cv-pdf-viewer__direct-link" href="{{ '/assets/pdf/cv.pdf' | relative_url }}">English CV</a>
    directly.
  </p>
</div>

<script>
  (() => {
    const viewer = document.querySelector('.cv-pdf-viewer');
    if (!viewer) return;

    const frame = viewer.querySelector('.cv-pdf-viewer__frame');
    const languageButton = viewer.querySelector('.cv-pdf-viewer__language');
    const directLink = viewer.querySelector('.cv-pdf-viewer__direct-link');
    const englishPdf = viewer.dataset.englishPdf;
    const chinesePdf = viewer.dataset.chinesePdf;
    let currentLanguage = 'en';

    languageButton.addEventListener('click', () => {
      const showChinese = currentLanguage === 'en';
      currentLanguage = showChinese ? 'zh' : 'en';

      const pdf = showChinese ? chinesePdf : englishPdf;
      const label = showChinese ? '中文简历' : 'English CV';

      frame.src = `${pdf}#view=FitH`;
      frame.title = label;
      directLink.href = pdf;
      directLink.textContent = label;
      languageButton.textContent = showChinese ? 'English Version' : '中文版';
      languageButton.setAttribute('aria-label', showChinese ? 'Switch to English CV' : 'Switch to Chinese CV');
    });
  })();
</script>
