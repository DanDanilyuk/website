---
layout: project
title: 'Bill of Sale Builder'
date: 2026-05-07 16:04:00 -0400
categories: project
image: /images/bill_of_sale_builder_cover.svg
---

[![Bill of Sale Builder](/images/bill_of_sale_builder_cover.svg)](https://www.billofsalebuilder.com)

**Description**: Bill of Sale Builder is a static, browser-only wizard that produces a downloadable PDF Vehicle Bill of Sale for any US state plus the District of Columbia. A six-step flow collects the state and role, both parties' details, the vehicle, and the sale terms, then renders a state-aware PDF in the browser. Nothing is sent to a server; all data lives in `localStorage` until the form is cleared.

**Features**:

- Six-step wizard covering setup, your info, the other party, the vehicle, sale terms, and review
- Full coverage for all 50 US states and the District of Columbia
- State-aware PDF output with the correct honorific, DMV reference link, and notary block per jurisdiction
- Federal post-2021 odometer disclosure (49 CFR 580) with automatic 20-year exemption
- Three vehicle types supported: motor vehicle, trailer, and boat, each with the right VIN, serial, or HIN rules
- VIN auto-decode via the NHTSA vPIC API to fill year, make, model, and body
- ZIP-driven city and state autofill via api.zippopotam.us, only filling blank values
- Joint-title support with a co-owner toggle on each party step
- Light and dark theme that follows `prefers-color-scheme` and persists explicit choices
- In-browser PDF preview before download, with form state saved to `localStorage` between sessions

**Motivation**: Selling a used car, trailer, or boat usually means hunting down the right state-specific Bill of Sale form, paying a generator service, or typing one from scratch. Bill of Sale Builder produces a clean, jurisdiction-correct PDF for free without sending personal details to a server. Keeping the form fully client-side matters because it carries names, addresses, ID numbers, and VINs.

**Technologies Used**:

- Vanilla JavaScript (ES2020) with native ES modules, no build step
- jsPDF, vendored locally with no runtime CDN dependency
- NHTSA vPIC API for VIN decoding
- api.zippopotam.us for ZIP to city/state lookup
- `localStorage` for form persistence and theme preference
- HTML and CSS with `[data-theme]` light/dark theming
- Self-hosted Inter woff2 font

**Impact**: Bill of Sale Builder removes a small but persistent friction from private vehicle sales by producing a legally formatted, state-correct document in a few minutes. The fully client-side architecture keeps sensitive personal information on the user's device.

**Website**: [www.billofsalebuilder.com](https://www.billofsalebuilder.com)

**GitHub**: [DanDanilyuk/billofsalebuilder](https://github.com/DanDanilyuk/billofsalebuilder)
