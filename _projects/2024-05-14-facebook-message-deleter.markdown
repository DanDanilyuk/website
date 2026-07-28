---
layout: project
title: 'Facebook Message Deleter'
date: 2024-05-14 13:01:12 -0400
categories: project
image: /images/facebook_message_deleter_cover.svg
---

[![Facebook Message Deleter](/images/facebook_message_deleter_cover.svg)](https://dandanilyuk.github.io/facebook_message_deleter)

**Description**: Facebook Message Deleter is a browser console script that bulk-deletes Facebook Messenger conversations. Open Messenger, paste the script into the developer console, and it works through the conversation list the same way a person would: open each thread's menu, click Delete, confirm, repeat. No extension, no install, and nothing to hand your login to.

**Features**:

- Runs straight from the browser console; nothing to install or grant permissions to
- On-page status bar with a live deletion count and a STOP button to end the run at any point
- Keeps deleting until the conversation list is empty, pacing itself as Messenger lazy-loads more threads
- Optional `LIMIT` constant to cap deletions per run for anyone worried about rate limiting
- Minified single-line version for quick pasting
- Companion GitHub Pages site for copying the script without cloning the repo
- Entirely client-side; the script touches nothing but the Messenger page it runs on

**Motivation**: Facebook offers no way to bulk-delete Messenger conversations. Clearing years of history means removing threads one at a time, three clicks each. This script automates exactly those clicks, so a cleanup that would take hours runs unattended in minutes.

**Technologies Used**:

- Vanilla JavaScript executed in the browser's developer console
- DOM automation driving the same Messenger menus a person would click
- Timed waits that pace deletions against Messenger's lazy loading
- A minified build alongside the readable source

**Impact**: Facebook Message Deleter gives people a practical way to clear their message history and take back some privacy. Because it is a readable script pasted by hand rather than an extension, there is no third party to trust with account access.

**Website**: [dandanilyuk.github.io/facebook_message_deleter](https://dandanilyuk.github.io/facebook_message_deleter/)

**GitHub**: [DanDanilyuk/facebook_message_deleter](https://github.com/DanDanilyuk/facebook_message_deleter)
