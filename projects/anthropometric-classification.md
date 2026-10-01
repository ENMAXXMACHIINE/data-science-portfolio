---
layout: default
title: Anthropometric Classification
permalink: /projects/anthropometric-classification/
---
<p class="eyebrow">04 · CLASSIFICATION · MODEL EVALUATION</p>
<h1>Anthropometric Classification</h1>
<p class="lead">A classification project using physical measurements to predict body composition categories and evaluate model quality under realistic validation conditions.</p>

<section class="case-section">
  <div class="section-label">RESEARCH QUESTION</div>
  <div>
    <h2>Can we classify body type from anthropometric measurements?</h2>
    <p>Using anthropometric variables like height, weight, and body measurements, can a model distinguish between body composition categories with acceptable reliability? The challenge is balancing predictive power with interpretability.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">METHODOLOGY</div>
  <div>
    <h2>Multi-class classification with validation</h2>
    <p>I tested multiple classifiers using stratified validation and evaluated them via precision, recall, F1-score, and confusion matrices. The focus was not only accuracy, but also which classes were harder to distinguish.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">MODEL PERFORMANCE</div>
  <div>
    <ul>
      <li>Best-performing model achieved strong weighted F1 performance across classes.</li>
      <li>Random forest and boosting methods offered better generalization than simple baselines.</li>
      <li>Boundary cases remained the hardest to classify, suggesting real-world ambiguity.</li>
    </ul>
  </div>
</section>

<section class="case-section">
  <div class="section-label">AI USAGE & DISCLOSURE</div>
  <div>
    <h2>How this project was built.</h2>
    <p><strong>Code & Testing:</strong> LLMs were used to assist with classifier implementation and evaluation code. All model selection, validation strategy, and interpretation decisions are based on independent analysis.</p>
    <p><strong>Sources:</strong> Draws on multi-class classification literature, model evaluation frameworks, and cross-validation methodology.</p>
  </div>
</section>

<div class="case-footer">
  <a class="button" href="https://github.com/ENMAXXMACHIINE">View Code →</a>
  <a class="link" href="{{ '/projects/' | relative_url }}">Back to projects</a>
</div>
