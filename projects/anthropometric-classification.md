---
layout: default
title: Anthropometric Classification
permalink: /projects/anthropometric-classification/
---
<p class="eyebrow">04 · CLASSIFICATION · MODEL EVALUATION</p>
<h1>Anthropometric Classification</h1>
<p class="lead">Multi-class classification model for body composition categories using physical measurements and machine learning evaluation techniques.</p>

<section class="case-section">
  <div class="section-label">RESEARCH QUESTION</div>
  <div>
    <h2>Can we accurately classify body type from measurements?</h2>
    <p>Using anthropometric data (height, weight, and body measurements), can we reliably predict body composition categories?</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">METHODOLOGY</div>
  <div>
    <h2>Multi-class classification with rigorous evaluation</h2>
    <p>Data was split using stratified cross-validation. Multiple classifiers were trained and evaluated using precision, recall, F1-score, and confusion matrices.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">MODEL PERFORMANCE</div>
  <div>
    <ul>
      <li>Best model achieved 87% weighted F1-score across 3 classes</li>
      <li>Random forest showed stronger generalization in cross-validation</li>
      <li>Class-specific analysis revealed more difficulty distinguishing borderline cases</li>
    </ul>
  </div>
</section>

<div class="case-footer">
  <a class="button" href="https://github.com/ENMAXXMACHIINE">View Code →</a>
  <a class="link" href="{{ '/projects/' | relative_url }}">Back to projects</a>
</div>
