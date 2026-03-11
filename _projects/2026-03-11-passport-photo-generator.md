---
layout: project
title: 'Passport Photo Generator'
date: 2026-03-11 16:04:00 -0500
categories: project
image: /images/passport_photo_generator_cover.svg
---

[![Passport Photo Generator](/images/passport_photo_generator_cover.svg)](https://dandanilyuk.github.io/passport_photo_generator/)

**Description**:
The Passport Photo Generator is a client-side web application that arranges passport photos onto standard print sizes for convenient home or pharmacy printing. Users simply crop their photo using the State Department's online tool, upload the cropped image, select a print size, and download a print-ready file. All image processing happens entirely in the browser with no server uploads required.

**Features**:

- Simple 4-step workflow: crop, upload, select print size, download
- Support for standard print sizes (4x6" and 5x7")
- 300 DPI output for high-quality prints
- 2x2" passport photo arrangement optimized for each print size
- Fully client-side processing with no server uploads or data collection
- Output as ready-to-print JPEG files
- Precise pixel dimensions (600x600px per photo, 1200x1800px for 4x6", 1500x2100px for 5x7")
- Clean, minimal interface with guided steps

**Motivation**: Getting passport photos printed can be surprisingly expensive for what amounts to a simple image arrangement task. This project provides a free, privacy-respecting alternative that lets anyone generate print-ready passport photo sheets at home or at a local pharmacy. By keeping all processing in the browser, it ensures that sensitive identity photos are never uploaded to a third-party server.

**Technologies Used**:

- HTML/CSS
- JavaScript
- Client-side image processing
- Canvas API for photo arrangement and export
- Responsive design

**Impact**: The Passport Photo Generator saves users time and money by eliminating the need for professional passport photo services. It prioritizes privacy by processing everything locally in the browser, making it a trustworthy option for handling sensitive identity photos. The straightforward workflow makes it accessible to users of all technical skill levels.

**Website**: [Passport Photo Generator](https://dandanilyuk.github.io/passport_photo_generator/)

**GitHub**: [DanDanilyuk/passport_photo_generator](https://github.com/DanDanilyuk/passport_photo_generator)
