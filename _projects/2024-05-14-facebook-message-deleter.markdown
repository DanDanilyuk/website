---
layout: project
title: 'Facebook Message Deleter'
date: 2024-05-14 13:01:12 -0400
categories: project
image: /images/facebook_message_deleter_cover.svg
---

[![Facebook Message Deleter](/images/facebook_message_deleter_cover.svg)](https://dandanilyuk.github.io/facebook_message_deleter)

**Description**: The Facebook Message Deleter is a browser console script that bulk-deletes Facebook Messenger conversations. Users paste the script into their browser's developer console on the Messenger page, and it automatically removes conversations in batches. No browser extensions or additional software required.

**Features**:

- Bulk deletion of Facebook Messenger conversations via browser console
- Rate-limited to 50 conversations per run to avoid triggering Facebook's abuse detection
- Minified script version available for quick pasting
- HTML-based interface as an alternative to console usage
- Runs entirely in the browser with no external server communication
- No browser extensions or software installations needed

**Motivation**: Facebook does not provide a built-in way to bulk-delete Messenger conversations. Removing them one by one is tedious, especially for users with hundreds or thousands of conversations. This script automates the process, letting users clean up their message history in minutes instead of hours.

**Technologies Used**:

- JavaScript (browser console execution)
- Facebook Messenger DOM interaction
- HTML interface for non-technical users
- Script minification for ease of use

**Impact**: The Facebook Message Deleter saves significant time for users who want to clean up their Messenger history. By automating a process that Facebook intentionally makes difficult, it gives users more control over their own data and privacy.

**Website**: [Facebook Message Deleter](https://dandanilyuk.github.io/facebook_message_deleter/)

**GitHub**: [DanDanilyuk/facebook_message_deleter](https://github.com/DanDanilyuk/facebook_message_deleter)
