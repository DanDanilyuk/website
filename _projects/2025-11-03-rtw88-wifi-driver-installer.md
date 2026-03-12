---
layout: project
title: 'RTW88 WiFi Driver Installer'
date: 2025-11-03 17:02:00 -0500
categories: project
image: /images/rtw88_driver_installer_cover.svg
---

[![RTW88 WiFi Driver Installer](/images/rtw88_driver_installer_cover.svg)](https://dandanilyuk.github.io/rtw88_driver_installer/)

**Description**: The RTW88 WiFi Driver Installer is an automated installation script that streamlines the setup of Realtek WiFi 5 drivers on Linux systems. It handles dependency resolution, kernel module compilation, and Secure Boot MOK enrollment to enable WiFi adapter support without manual configuration.

**Features**:

- One-line install command for Realtek RTW88 WiFi 5 drivers
- Support for multiple Realtek chipsets (RTL8723DE, RTL8814AE, RTL8821CE, RTL8822BE, RTL8822CE, and USB variants)
- PCIe, USB, and SDIO adapter support
- DKMS integration for automatic driver rebuilds on kernel updates
- Secure Boot MOK (Machine Owner Key) enrollment support
- Pre-built firmware bundling and modprobe configuration
- Compatibility with Ubuntu 20.04+, Debian, Arch Linux, Manjaro, EndeavourOS, and Raspberry Pi OS
- Support for both 32-bit and 64-bit systems
- Automated post-installation verification

**Motivation**: Linux users often struggle with Realtek WiFi adapter installation, particularly around Secure Boot configurations and kernel module compilation. This project eliminates that complexity by automating the entire process into a single command, making reliable WiFi setup accessible regardless of Linux experience.

**Technologies Used**:

- Bash shell scripting
- DKMS (Dynamic Kernel Module Support)
- Linux kernel module compilation toolchain
- Multi-distro package management (apt, pacman)

**Impact**: The RTW88 WiFi Driver Installer removes the most common barrier to Linux adoption for users with Realtek WiFi hardware. It provides a reliable, reproducible installation method across multiple distributions, saving hours of manual troubleshooting.

**Website**: [RTW88 WiFi Driver Installer](https://dandanilyuk.github.io/rtw88_driver_installer/)

**GitHub**: [DanDanilyuk/rtw88_driver_installer](https://github.com/DanDanilyuk/rtw88_driver_installer)
