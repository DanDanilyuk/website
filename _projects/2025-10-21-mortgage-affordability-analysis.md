---
layout: project
title: 'Mortgage Affordability Analysis'
date: 2025-10-21 14:30:00 -0400
categories: project
image: /images/mortgage_affordability_cover.svg
---

[![Mortgage Affordability Analysis](/images/mortgage_affordability_cover.svg)](https://homeaffordabilitytracker.com/)

**Description**: Mortgage Affordability Analysis, live as the Home Affordability Tracker, is a dashboard that charts US home affordability by comparing the full cost of a 30-year mortgage against income. It computes a price-to-income ratio: total principal plus interest divided by annual earnings, where a higher number means housing is further out of reach. The data refreshes weekly from federal sources and covers the nation, all 50 states, and Washington, D.C.

**Features**:

- Price-to-income ratio combining home prices, 30-year mortgage rates, and average earnings in one number
- Single-earner and dual-income (1.4x) household views
- State-level breakdowns using state-specific income multipliers and home prices
- Interactive chart with zoom, pan, date range selection, and per-point inspection
- Dark mode with system preference detection
- Data regenerated automatically every Thursday by a GitHub Actions workflow

**Motivation**: "Is housing getting less affordable?" is a simple question buried under three separate datasets: prices, rates, and wages. Each one alone tells a partial story. Combining them into a single ratio, tracked weekly across decades and broken down by state, makes the trend plain enough to see at a glance.

**Technologies Used**:

- Vanilla JavaScript (ES6+), HTML, and CSS custom properties for theming
- Chart.js 4 with chartjs-plugin-zoom for the interactive chart
- Ruby data pipeline pulling BLS Average Weekly Earnings, Zillow Home Value Index via FRED, and Freddie Mac 30-year rates (MORTGAGE30US)
- BLS Quarterly Census of Employment and Wages for state income multipliers
- GitHub Actions for the weekly refresh; GitHub Pages hosting with no build step

**Impact**: The tracker condenses decades of economic data into one legible affordability trend, at both the national and state level. Because the pipeline runs itself every week, the picture stays current without anyone touching it.

**Website**: [homeaffordabilitytracker.com](https://homeaffordabilitytracker.com/)

**GitHub**: [DanDanilyuk/mortgage_affordability_analysis](https://github.com/DanDanilyuk/mortgage_affordability_analysis)
