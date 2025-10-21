---
layout: project
title: 'Mortgage Affordability Analysis'
date: 2025-10-21 14:30:00 -0400
categories: project
image: /images/mortgage_affordability_cover.svg
---

[![Mortgage Affordability Analysis](/images/mortgage_affordability_cover.svg)](https://dandanilyuk.github.io/mortgage_affordability_analysis/)

**Description**: The Mortgage Affordability Analysis visualizes the relationship between housing costs and income over time using a cost-to-income multiplier. It combines Case-Shiller Home Price Index data, 30-year mortgage rates, and average weekly earnings to calculate how many years of income it would take to pay off a typical 30-year mortgage. The tool provides both single-income and household-income perspectives on housing affordability.

**Features**:

- Interactive Chart.js visualization with zoom and pan functionality
- Weekly data points aligned to mortgage rate release dates (Thursdays)
- Dual perspective: single income vs. household income (1.4x multiplier)
- Estimated future values using daily seasonal adjustment factors
- Visual distinction between actual and estimated data (solid vs. dashed lines)
- Date range selection for focused analysis
- Real-time calculations combining multiple economic data sources

**Motivation**: Understanding housing affordability requires analyzing multiple economic factors simultaneously. This project addresses the challenge of tracking how accessible homeownership is relative to income over time. By automating data collection from BLS and FRED APIs and calculating a comprehensive affordability metric, it provides valuable insights into housing market trends that affect millions of potential homebuyers.

**Technologies Used**:

- Ruby (data fetching and processing)
- BLS API (Bureau of Labor Statistics - Average Weekly Earnings)
- FRED API (Federal Reserve Economic Data - Case-Shiller Index and Mortgage Rates)
- HTML/CSS/JavaScript
- Chart.js (interactive data visualization)
- JSON (data serialization)
- Date interpolation and seasonal adjustment algorithms

**Impact**: The Mortgage Affordability Analysis democratizes access to complex economic analysis by presenting multiple data sources in a single, easy-to-understand visualization. It helps users understand long-term housing market trends and make informed decisions about homeownership. The tool's ability to project future values using seasonal patterns provides additional forecasting capabilities beyond raw data availability.

**Website**: [Mortgage Affordability Analysis](https://dandanilyuk.github.io/mortgage_affordability_analysis/)

**Github**: [Source Code](https://github.com/DanDanilyuk/mortgage_affordability_analysis)
