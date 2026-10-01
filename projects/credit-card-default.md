---
layout: default
title: Credit Card Default Prediction
permalink: /projects/credit-card-default/
---
<p class="eyebrow">02 · CLASSIFICATION · RISK</p>
<h1>Credit Card Default Prediction</h1>
<p class="lead">A classification modeling project designed to identify likely loan and credit default risk using financial behavior and repayment patterns.</p>

<section class="case-section">
  <div class="section-label">RESEARCH QUESTION</div>
  <div>
    <h2>Who is at risk of defaulting?</h2>
    <p>Using historical consumer credit data, can we build a predictive model that separates customers at high risk of default from those who are more likely to stay current? This question matters because the model supports early intervention and risk management decisions.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">METHODOLOGY</div>
  <div>
    <h2>Classification with careful feature engineering</h2>
    <p>I compared logistic regression, random forest, and boosting approaches using credit, payment, and delinquency features. Feature engineering focused on repayment behavior, utilization, and account history to improve signal and interpretability.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">KEY FINDINGS</div>
  <div>
    <ul>
      <li>Recent payment status and delinquency history were the strongest drivers of default risk.</li>
      <li>Utilization and account age created nonlinear patterns that improved model performance.</li>
      <li>Ensemble methods materially improved discrimination over a baseline logistic model.</li>
    </ul>
  </div>
</section>

<section class="case-section">
  <div class="section-label">LIMITATIONS</div>
  <div>
    <p>Class imbalance required careful threshold tuning and recall/precision trade-offs. Real-world performance may shift over time as borrower behavior and macroeconomic conditions change.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">AI USAGE & DISCLOSURE</div>
  <div>
    <h2>How this project was built.</h2>
    <p><strong>Code & Analysis:</strong> LLMs were used to assist with model implementation, feature engineering techniques, and documentation. All modeling decisions and interpretations are based on independent analysis and validation.</p>
    <p><strong>Sources:</strong> Draws on classification metrics literature, imbalanced learning strategies, and credit risk modeling principles.</p>
  </div>
</section>

<div class="case-footer">
  <a class="button" href="https://github.com/ENMAXXMACHIINE">View Code →</a>
  <a class="link" href="{{ '/projects/' | relative_url }}">Back to projects</a>
</div>
