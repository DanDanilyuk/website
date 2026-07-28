---
layout: project
title: 'Adobe Services Disabler'
date: 2026-07-28 12:00:00 -0400
categories: project
image: /images/adobe_services_disabler_cover.svg
---

[![Adobe Services Disabler](/images/adobe_services_disabler_cover.svg)](https://dandanilyuk.github.io/adobe_services_disabler/)

**Description**: Adobe Services Disabler is a pair of menu-driven scripts, one for macOS and one for Windows, that switch off every Adobe background service, helper, updater, and telemetry agent with a single command. The same command switches everything back on. Nothing is deleted, so Enable genuinely restores the original state.

**Features**:

- One-line install command for both macOS (Bash) and Windows (PowerShell)
- Interactive arrow-key menu with Disable, Enable, and Quit choices; nothing is touched until a choice is made
- Wildcard discovery of Adobe items, so the scripts keep working after an Adobe update recreates them
- macOS: boots out and disables every `com.adobe.*` launchd agent and daemon across `/Library/LaunchAgents`, `~/Library/LaunchAgents`, and `/Library/LaunchDaemons` so they stay off across reboots
- macOS: switches off the Finder Sync and right-click app extensions with `pluginkit`, the only level at which they stay off
- Windows: stops services and sets them to Disabled, recording the original start type in the registry so Enable restores Manual instead of forcing everything to Automatic
- Windows: disables updater and telemetry scheduled tasks, plus Run and RunOnce startup entries, using the same `StartupApproved` flag Task Manager's Startup tab writes
- Stops running Adobe helper processes while never touching the creative apps themselves
- Degrades gracefully without sudo or Administrator rights by handling per-user items and saying so up front
- A downloaded copy deletes itself once it finishes; a copy inside a git checkout is left alone

**Motivation**: Creative Cloud installs a set of helpers, updaters, and telemetry agents that start with the machine and keep running whether or not any Creative Cloud app is ever opened. Ending them from Activity Monitor or Task Manager does not last, since they relaunch on the next boot. These scripts find every Adobe launch item by wildcard, switch each one off in the place that actually keeps it off, and stop the ones already running. Making the change fully reversible removes the risk of trying it.

**Technologies Used**:

- Bash with `launchctl` and `pluginkit` on macOS
- PowerShell with Windows services, scheduled tasks, and registry `StartupApproved` startup flags
- Arrow-key terminal menus built from raw escape sequences, with no dependencies beyond a stock shell
- Static landing page in vanilla HTML, CSS, and JavaScript with light and dark theming, served by GitHub Pages

**Impact**: Adobe Services Disabler reclaims memory and CPU on any machine with Creative Cloud installed, without uninstalling anything. Because state is recorded before each change and nothing is deleted, a single Enable run puts the machine back exactly as it was.

**Website**: [dandanilyuk.github.io/adobe_services_disabler](https://dandanilyuk.github.io/adobe_services_disabler/)

**GitHub**: [DanDanilyuk/adobe_services_disabler](https://github.com/DanDanilyuk/adobe_services_disabler)
