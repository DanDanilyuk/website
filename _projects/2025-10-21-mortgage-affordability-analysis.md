---
layout: project
title: 'Mortgage Affordability Analysis'
date: 2025-10-21 14:30:00 -0400
categories: project
image: /images/mortgage_affordability_cover.svg
---

[![Mortgage Affordability Analysis](/images/mortgage_affordability_cover.svg)](https://dandanilyuk.github.io/mortgage_affordability_analysis/)

**Description**: The Mortgage Affordability Analysis is an interactive dashboard that visualizes US housing affordability over time using a cost-to-income multiplier. It combines Case-Shiller Home Price Index data, 30-year mortgage rates, and average weekly earnings to calculate how many years of income it would take to pay off a typical 30-year mortgage. The tool provides both single-income and household-income perspectives.

**Features**:

- Interactive Chart.js visualization with zoom and pan controls
- Weekly data points aligned to mortgage rate release dates (Thursdays)
- Dual perspective toggle: single income vs. household income (1.4x multiplier)
- Estimated future values using daily seasonal adjustment factors
- Visual distinction between actual and estimated data using solid vs. dashed lines
- Date range selection for focused analysis of specific time periods
- Automated data fetching from BLS and FRED APIs via Ruby scripts

**Motivation**: Understanding housing affordability requires analyzing multiple economic factors simultaneously. This project addresses the challenge of tracking how accessible homeownership is relative to income over time. By combining data from the Bureau of Labor Statistics and the Federal Reserve, it produces a single affordability metric that reveals long-term housing market trends.

**Technologies Used**:

- Ruby for data fetching and processing
- BLS API (Bureau of Labor Statistics - Average Weekly Earnings)
- FRED API (Federal Reserve Economic Data - Case-Shiller Index and Mortgage Rates)
- HTML/CSS/JavaScript
- Chart.js for interactive data visualization
- Date interpolation and seasonal adjustment algorithms

**Impact**: The Mortgage Affordability Analysis presents complex economic data in an accessible, interactive format. It helps users understand long-term housing market trends and provides forecasting through seasonal pattern projections beyond raw data availability.

**Website**: [Mortgage Affordability Analysis](https://dandanilyuk.github.io/mortgage_affordability_analysis/)

**GitHub**: [DanDanilyuk/mortgage_affordability_analysis](https://github.com/DanDanilyuk/mortgage_affordability_analysis)
