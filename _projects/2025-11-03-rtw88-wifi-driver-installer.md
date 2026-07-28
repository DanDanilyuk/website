---
layout: project
title: 'RTW88 WiFi Driver Installer'
date: 2025-11-03 17:02:00 -0500
categories: project
image: /images/rtw88_driver_installer_cover.svg
---

[![RTW88 WiFi Driver Installer](/images/rtw88_driver_installer_cover.svg)](https://dandanilyuk.github.io/rtw88_driver_installer/)

**Description**: RTW88 WiFi Driver Installer is a script that automates setting up Realtek WiFi 5 drivers on Linux. One command handles dependency resolution, kernel module compilation, Secure Boot MOK enrollment, and post-install verification, turning a notoriously fiddly driver installation into a single step.

**Features**:

- One-line install command for the Realtek RTW88 driver family
- Support for multiple Realtek chipsets (RTL8723DE, RTL8814AE, RTL8821CE, RTL8822BE, RTL8822CE, and USB variants)
- PCIe, USB, and SDIO adapter support
- DKMS integration so drivers rebuild automatically on every kernel update
- Secure Boot support through MOK (Machine Owner Key) enrollment
- Pre-built firmware bundling and modprobe configuration
- Works on Ubuntu 20.04+, Debian, Arch Linux, Manjaro, EndeavourOS, and Raspberry Pi OS, on both 32-bit and 64-bit systems
- Automated post-installation verification

**Motivation**: Realtek WiFi adapters are everywhere in budget laptops, and Linux support for them regularly means compiling a kernel module by hand and fighting Secure Boot. Each step is a place for a newcomer to get stuck with no working internet to search for answers. The installer collapses all of it into one command that ends with working WiFi.

**Technologies Used**:

- Bash shell scripting
- DKMS (Dynamic Kernel Module Support)
- The Linux kernel module compilation toolchain
- Multi-distro package management (apt, pacman)

**Impact**: The installer gives owners of Realtek hardware a reliable, reproducible path to working WiFi across major distributions. What used to cost an afternoon of forum threads now takes the time of one command.

**Website**: [dandanilyuk.github.io/rtw88_driver_installer](https://dandanilyuk.github.io/rtw88_driver_installer/)

**GitHub**: [DanDanilyuk/rtw88_driver_installer](https://github.com/DanDanilyuk/rtw88_driver_installer)
