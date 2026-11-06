---
layout: project
title: 'Passport Photo Generator'
date: 2026-03-11 16:04:00 -0500
categories: project
description: 'Print your own passport photos for under a dollar, with every pixel processed in your browser.'
website: https://dandanilyuk.github.io/passport_photo_generator/
github: https://github.com/DanDanilyuk/passport_photo_generator
image: /images/projects/passport_photo_generator.jpg
logo: /images/passport_photo_generator_cover.svg
caption: 'A 4x6" print sheet of six 2x2" photos, shown here with my headshot.'
---

## Description

Passport Photo Generator is a client-side web app that arranges passport photos onto standard print sizes, ready to print at home or at a pharmacy kiosk. Crop your photo with the State Department's free tool, upload it, pick a print size, and download a print-ready JPEG. Every pixel is processed in the browser; nothing is uploaded anywhere.

## Features

- Four-step workflow: crop with the State Department's tool, upload, pick a size, download
- 4x6" and 5x7" print layouts filled with 2x2" passport photos
- 300 DPI output with exact pixel dimensions: 600x600 per photo, 1200x1800 for 4x6", 1500x2100 for 5x7"
- Fully client-side processing with no server uploads and no data collection
- No build tools or dependencies; the whole app is a single page

## Motivation

Pharmacies charge upwards of fifteen dollars for passport photos, and the actual work is arranging a government-cropped image onto a 4x6 sheet. That is a job for a canvas, not a service counter. Printing the sheet as a regular photo costs under a dollar.

## Technologies Used

- HTML, CSS, and vanilla JavaScript
- Canvas API for photo arrangement, resizing, and JPEG export
- The State Department's photo crop tool as the upstream compliance step

## Impact

Passport Photo Generator turns a fifteen-dollar errand into a one-dollar print. Keeping identity photos entirely on the user's own device makes it an easy tool to trust with a sensitive document.
