# A/B Test Simulation 

## Overview
A concise, Colab-ready notebook that simulates an A/B experiment for a recommendation change and demonstrates standard analysis steps: data simulation, aggregation, inference (two-sample proportions z-test), confidence intervals (Wilson), and visualization. This is a self-contained educational/prototyping asset — no external dataset required.

## Key Features
- Synthetic user-level binary outcome generation (Bernoulli trials).
- Per-arm metrics: sample size, conversions, conversion rates.
- Absolute and relative lift calculation.
- Two-sample proportions z-test (via `statsmodels`) with two-sided p-value.
- Wilson confidence intervals for each arm (more robust than Wald in many cases).
- Clean, Colab-oriented layout with separate Markdown and code cells, plus a horizontal bar plot of rates with CIs.

## Requirements
- Python 3.8+
- Packages:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `statsmodels`


## Ethical Considerations

When moving from simulated demos to real-world experiments, consider the ethical and user-impact dimensions of experimentation. This project is intended for learning and prototyping; apply the following principles when working with real user data or production experiments:

Privacy & Data Protection

Avoid collecting or storing personally identifiable information (PII) unless strictly necessary and approved.

Anonymize or pseudonymize user identifiers before analysis.

Follow applicable data-protection laws and organizational policies (e.g., GDPR, CCPA). Ensure appropriate data retention and deletion policies.
