---
layout: default
title: Football Match Intelligence
permalink: /projects/football-match-intelligence/
---
<p class="eyebrow">05 · SPORTS ANALYTICS · HOME ADVANTAGE</p>
<h1>Football Match Intelligence</h1>
<p class="lead">A reproducible match-analysis project using a realistic synthetic football dataset to study which teams and match conditions are associated with the strongest home performance.</p>

<div class="status-banner">
  <div><small>RESEARCH QUESTION</small><strong>Which teams and conditions drive home advantage?</strong></div>
  <p>Using structured match-level data, this project asks whether home performance is strongest for certain teams, in particular seasons, and under particular conditions such as weather and attendance.</p>
</div>

<section class="case-section">
  <div class="section-label">DATASET</div>
  <div>
    <h2>6,000 matches across six seasons.</h2>
    <p>The project uses a synthetic but realistic football match dataset generated for analysis. It contains 6,000 matches, 12 teams, and 16 columns. The unit of analysis is a single match, with each row representing one team matchup in a specific season. The dataset includes team identity, season, weather, attendance, expected goals, goals, shots, possession, fouls, referee, and result.</p>
    <ul>
      <li><strong>Source:</strong> Synthetic dataset generated for educational analysis; designed to reflect realistic football match patterns.</li>
      <li><strong>Unit of analysis:</strong> One match.</li>
      <li><strong>Sample size:</strong> 6,000 matches.</li>
      <li><strong>Features:</strong> match_id, season, home_team, away_team, weather, attendance, home_xg, away_xg, home_goals, away_goals, home_shots, away_shots, home_possession_pct, fouls, referee, result.</li>
      <li><strong>Missing data:</strong> No material missing values were introduced in the synthetic data generation stage.</li>
    </ul>
  </div>
</section>

<section class="case-section">
  <div class="section-label">VARIABLES</div>
  <div>
    <h2>Key variables and operationalization.</h2>
    <p><strong>Home performance</strong> is operationalized as whether the home team wins, the margin of victory, and the difference in expected goals between home and away teams. Home advantage is then explored across team identity, weather, and attendance context.</p>
    <p><strong>Primary explanatory variables:</strong> home_team, away_team, weather, attendance, home_xg, away_xg, home_possession_pct, and referee. These variables help explain whether match context or team quality is more strongly associated with home success.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">DATA CLEANING</div>
  <div>
    <h2>Pandas-based cleaning logic.</h2>
    <p>Because this project is designed to be reproducible and teachable, the workflow starts by checking data integrity, normalizing values, and identifying edge cases before modeling. A pandas version would convert the synthetic CSV into a dataframe, standardize weather labels, convert attendance to numeric, and clean team labels or referee inconsistencies.</p>
    <pre><code>import pandas as pd

df = pd.read_csv('football_matches.csv')
df['weather'] = df['weather'].str.strip().str.title()
df['attendance'] = pd.to_numeric(df['attendance'], errors='coerce')
df['result'] = df['result'].astype(str)

# handle missing values
for col in ['attendance', 'home_xg', 'away_xg']:
    df[col] = df[col].fillna(df[col].median())

df = df.drop_duplicates(subset=['match_id'])</code></pre>
    <p>These steps matter because team names, weather labels, and attendance can vary in ways that distort comparisons. Standardizing categories helps reduce noise and improves model interpretability before assessing home advantage patterns.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">VISUALIZATIONS</div>
  <div>
    <h2>Two visuals directly tied to the research question.</h2>
    <div class="image-grid">
      <figure>
        <img src="{{ '/assets/images/football-home-advantage.svg' | relative_url }}" alt="Bar chart of home win rate by team">
        <figcaption>Figure 1. Home win rate by team. This chart shows which clubs are most strongly associated with home success.</figcaption>
      </figure>
      <figure>
        <img src="{{ '/assets/images/football-weather-home.svg' | relative_url }}" alt="Bar chart of home win rate by weather condition">
        <figcaption>Figure 2. Home win rate by weather condition. Weather can affect home-team performance through field conditions and tactical adjustments.</figcaption>
      </figure>
    </div>
  </div>
</section>

<section class="case-section">
  <div class="section-label">LIMITATIONS</div>
  <div>
    <h2>Important caveats.</h2>
    <p>Because the dataset is synthetic, it is designed for teaching and reproducibility rather than empirical inference. It does not capture true tactical changes, injuries, travel burdens, or long-run club-specific effects. It also omits real-world metrics such as xG under pressure, tactical formations, referee bias, and player availability, which may matter in actual match analysis.</p>
    <p>Unanswered questions include whether home advantage changes with crowd size, whether certain weather conditions systematically amplify or reduce home performance, and whether stronger teams maintain a consistent edge regardless of venue.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">CODE</div>
  <div>
    <h2>Underlying notebook.</h2>
    <p>The full reproducible notebook is linked below.</p>
    <div class="case-footer">
      <a class="button" href="https://github.com/ENMAXXMACHIINE/data-science-portfolio/blob/main/Project%20Phase%202%20DTSC.ipynb">Open Notebook →</a>
      <a class="link" href="{{ '/projects/' | relative_url }}">Back to projects</a>
    </div>
  </div>
</section>

<section class="case-section">
  <div class="section-label">AI USAGE & DISCLOSURE</div>
  <div>
    <h2>How this project was built.</h2>
    <p><strong>Code and workflow:</strong> Large language models were used to assist with notebook structure, generation logic, and documentation. All analysis decisions, modeling choices, and interpretation were reviewed and validated independently.</p>
    <p><strong>Research basis:</strong> This project builds on common sports analytics concepts around home advantage, expected goals, and contextual match performance.</p>
  </div>
</section>

<section class="case-section">
  <div class="section-label">REFERENCES</div>
  <div>
    <p>Pollard, R. (1986). Home advantage in soccer: A review of its existence and causes. <em>Journal of Sports Sciences</em>, 4(3), 237–244.</p>
    <p>Reilly, T., &amp; Thomas, V. (1976). A motion analysis of work-rate in different positional roles in professional football match-play. <em>Journal of Human Movement Studies</em>, 2(2), 87–97.</p>
    <p>Ruiz, H., et al. (2013). Analysis of football performance indicators. <em>International Journal of Performance Analysis in Sport</em>, 13(3), 731–748.</p>
  </div>
</section>
