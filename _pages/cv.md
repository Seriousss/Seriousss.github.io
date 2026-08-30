---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 3
cv_pdf: /assets/pdf/CV_tianran.pdf
description: Curriculum vitae.
---

<style>
  .cv-actions {
    margin: 0 0 1.25rem;
  }
  .cv-actions a {
    display: inline-block;
    padding: 0.4rem 0.9rem;
    border: 1px solid var(--global-theme-color, #4c96b7);
    border-radius: 4px;
    color: var(--global-theme-color, #4c96b7);
    text-decoration: none;
    font-size: 0.95rem;
  }
  .cv-actions a:hover {
    background-color: var(--global-theme-color, #4c96b7);
    color: #fff;
  }
  .cv-embed {
    width: 100%;
    aspect-ratio: 1 / 1.35;
    min-height: 480px;
    border: 1px solid var(--global-divider-color, rgba(0, 0, 0, 0.1));
    border-radius: 4px;
  }
  .cv-fallback {
    padding: 2rem;
    text-align: center;
  }
  @media (max-width: 576px) {
    .cv-embed {
      aspect-ratio: 1 / 1.1;
    }
  }
</style>

<div class="cv-actions">
  <a href="{{ page.cv_pdf | relative_url }}" target="_blank" rel="noopener">Download PDF</a>
</div>

<object class="cv-embed" data="{{ page.cv_pdf | relative_url }}" type="application/pdf">
  <div class="cv-fallback">
    <p>Your browser cannot display the PDF inline.</p>
    <a href="{{ page.cv_pdf | relative_url }}" target="_blank" rel="noopener">Open the CV in a new tab</a>
  </div>
</object>
