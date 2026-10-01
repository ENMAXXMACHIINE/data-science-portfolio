---
layout: default
title: Credit Card Default Prediction
permalink: /projects/credit-card-default/
---
<p class="eyebrow">02 · CLASSIFICATION · RISK</p>
<h1>Credit Card Default Prediction</h1>
<p class="lead">Logistic regression and ensemble methods for predicting credit card default risk using financial and behavioral data.</p>

<section class="case-section">
  <div class="section-label">RESEARCH QUESTION</div>
  <div>
    <h2>Who is at risk of defaulting?</h2>
    <p>Using historical credit card account data, can we build a predictive model to identify customers at risk of default, allowing proactive risk mitigation?</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">METHODOLOGY</div>
  <div>
    <h2>Classification with ensemble methods</h2>
    <p>We compared logistic regression, random forest, and gradient boosting models. Feature engineering included payment-to-balance ratios, delinquency patterns, and credit utilization metrics.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">KEY FINDINGS</div>
  <div>
    <ul>
      <li>Recent payment status is the strongest predictor</li>
      <li>Age and credit limit show non-linear relationships with default risk</li>
      <li>Ensemble methods outperformed logistic regression by 5–8 percentage points in AUC</li>
    </ul>
  </div>
</section>

<section class="case-section">
  <div class="section-label">LIMITATIONS</div>
  <div>
    <p>Class imbalance (default rate ~22%) required careful threshold tuning. Economic conditions, policy changes, and temporal drift could shift model performance in production.</p>
  </div>
</section>

<div class="case-footer">
  <a class="button" href="https://github.com/ENMAXXMACHIINE">View Code →</a>
  <a class="link" href="{{ '/projects/' | relative_url }}">Back to projects</a>
</div>
