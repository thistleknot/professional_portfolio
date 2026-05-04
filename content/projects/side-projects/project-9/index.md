---
title: "Algorithmic Investment Research: Markowitz, Factor Models & Business Cycles"
date: 2024-08-15
external_link: ""
summary: "Systematic quantitative investment research combining Modern Portfolio Theory (Markowitz optimization), multi-factor models, and macroeconomic cycle analysis. FRED API data integration for regime detection and dynamic portfolio rebalancing. Published research on systematic risk-return optimization."
tags:
  - portfolio-optimization
  - factor-models
  - macroeconomics
  - quantitative-finance
  - fred-api
  - systematic-research
---

## Algorithmic Investment Research: Markowitz, Factor Models & Business Cycles

Rigorous quantitative framework for portfolio optimization integrating Modern Portfolio Theory, multi-factor risk models, and macroeconomic regime detection.

### Components

**Markowitz Portfolio Optimization:**
- Efficient frontier computation
- Mean-variance optimization with constraints (transaction costs, leverage limits)
- Covariance matrix estimation and regularization
- Risk-adjusted return maximization

**Multi-Factor Models:**
- Fama-French factors (market, size, value, profitability, investment)
- Momentum and quality factors
- Factor exposure analysis and risk decomposition
- Alpha vs. beta attribution

**Business Cycle Integration:**
- FRED API data: employment, consumer confidence, ISM indices, yield curves
- Regime detection: expansion, contraction, inflection points
- Dynamic factor weights based on macroeconomic state
- Cycle-aware portfolio rebalancing

### Technical Stack

- Python: NumPy, SciPy optimization, Pandas
- FRED API: Federal Reserve economic data
- PostgreSQL: Time series storage and queries
- Statistical methods: Cointegration, regime-switching models, Kalman filtering

### Methodology

Beyond naive Markowitz (which assumes constant correlations), this system adapts to market regimes:
- Bull markets: higher equity exposure, factor tilts toward value
- Downturns: rebalance toward defensive factors, quality, lower volatility
- Inflection points: pre-position for regime transition

### Results

Systematic approach outperforms static allocation through regime-aware rebalancing and factor timing. Real-time deployment validates theoretical research.

