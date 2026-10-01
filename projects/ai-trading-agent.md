---
layout: default
title: AI Trading Agent
permalink: /projects/ai-trading-agent/
---
<p class="eyebrow">01 · AI / FINANCE / AGENT SYSTEMS</p>
<h1>AI Trading Agent</h1>
<p class="lead">A quantitative trading agent designed around forecasting, strategy construction, portfolio management, execution controls, and adversarial validation.</p>

<div class="status-banner">
  <div><small>RELEASE OUTCOME</small><strong>PRE-ALPHA</strong></div>
  <p>Strong internal research result. The system has not traded real capital, and investor-facing legal, compliance, and operational work remains outside the technical validation.</p>
</div>

<div class="evidence-image">
  <img src="{{ '/trading-agent-robustness-score.png' | relative_url }}" alt="AI trading robustness score chart">
</div>

<div class="metric-grid">
  <div><small>CERTIFICATION SCORE</small><strong>87.0<span>/100</span></strong><p>rule-based signal, corrected</p></div>
  <div><small>CERTIFIED SIGNAL</small><strong>Rule-based</strong><p>market-timing decisions</p></div>
  <div><small>REAL CAPITAL</small><strong>$0</strong><p>paper & historical only</p></div>
  <div><small>BREACH PROBABILITY</small><strong>10.2%<span>/yr</span></strong><p>15% drawdown guardrail</p></div>
  <div><small>OPEN DECISIONS</small><strong>3</strong><p>weights, f3, f7</p></div>
  <div><small>EFFECTIVE BREADTH</small><strong>7.2<span>/12</span></strong><p>independent breadth</p></div>
</div>

<section class="case-section">
  <div class="section-label">THE SYSTEM</div>
  <div>
    <h2>From model to agent.</h2>
    <p>Rather than treating trading as a single prediction model, this system connects forecasting, strategy logic, portfolio decisions, execution behavior, and safety limits into one research pipeline. The goal is not only to forecast returns, but to build a system that can be inspected and stress-tested under different conditions.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">VALIDATION</div>
  <div>
    <h2>12 phases. Multiple adversarial passes.</h2>
    <div class="phase-table">
      <div><b>02</b><strong>Robust Testing</strong><span>Mixed · 70/100 composite</span></div>
      <div><b>03</b><strong>Walk-Forward Validation</strong><span>Split verdict</span></div>
      <div><b>04</b><strong>Monte Carlo Certification</strong><span>Certified · 87.0/100</span></div>
      <div><b>05</b><strong>Execution Strengthening</strong><span>Pass bar met</span></div>
      <div><b>06</b><strong>Portfolio Management</strong><span>Built · unreviewed</span></div>
      <div><b>07</b><strong>Guardrail Strengthening</strong><span>Zero critical open</span></div>
      <div><b>08</b><strong>Explainability</strong><span>3/3 criteria met</span></div>
      <div><b>09</b><strong>Reliability Engineering</strong><span>Fails closed</span></div>
      <div><b>11</b><strong>Production Ready</strong><span>Pass bar met</span></div>
    </div>
  </div>
</section>

<section class="case-section">
  <div class="section-label">WHAT HELD UP</div>
  <div class="callout success">
    <h2>Guardrails were the strongest part of the system.</h2>
    <p>The validation framework reports six numeric rules plus a kill switch, adversarially tested across multiple market regimes. That makes the system more resilient in the face of extreme and unstable conditions.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">WHAT DIDN'T</div>
  <div class="callout warning">
    <h2>The ML edge is not certified.</h2>
    <p>The validation report explicitly does not support an "AI-driven edge" claim. The rule-based signal is the certified signal. Machine-learning forecasts are included but not independently validated for live trading.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">LIMITATIONS</div>
  <div class="limitation-list">
    <article><b>Never traded real capital</b><p>All reported results are backtests or simulations.</p></article>
    <article><b>Tail risk is higher than early estimates suggested</b><p>Under corrected daily compounding, Sharpe was 1.48 rather than 3.70 and breach probability 10.2%/yr rather than 1.1%.</p></article>
    <article><b>Three configuration decisions remain open</b><p>Target weights, f3 sector cap, and f7 daily-loss cap require explicit sign-off.</p></article>
    <article><b>Concentration remains structural</b><p>Effective breadth is 7.2 of 12 nominal positions; semiconductors represented 33.32% against a proposed 30% cap.</p></article>
    <article><b>Legal review is separate from technical validation</b><p>Any third-party offering requires qualified legal and compliance review. Technical certification does not establish regulatory readiness.</p></article>
  </div>
</section>

<section class="case-section">
  <div class="section-label">AI USAGE & DISCLOSURE</div>
  <div>
    <h2>How this project was built.</h2>
    <p><strong>Code Development:</strong> Large language models (LLMs) were used to assist with code structure, algorithm research, and documentation. All code was reviewed and validated for correctness and appropriateness before deployment.</p>
    <p><strong>Analysis & Strategy:</strong> All strategic decisions, validation logic, and risk frameworks were developed through independent research and domain expertise. AI tools supported exploration but did not drive core conclusions.</p>
    <p><strong>Sources:</strong> Research draws on quantitative finance literature, Monte Carlo simulation methodology, and portfolio optimization frameworks.</p>
  </div>
</section>

<div class="case-footer">
  <a class="button" href="https://github.com/ENMAXXMACHIINE">View GitHub →</a>
  <a class="link" href="{{ '/projects/' | relative_url }}">Back to projects</a>
</div>
