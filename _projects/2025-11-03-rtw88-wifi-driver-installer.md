---
layout: project
title: 'RTW88 WiFi Driver Installer'
date: 2025-11-03 17:02:00 -0500
categories: project
image: /images/rtw88_driver_installer_cover.svg
---

[![RTW88 WiFi Driver Installer](/images/rtw88_driver_installer_cover.svg)](https://dandanilyuk.github.io/rtw88_driver_installer/)

**Description**: The RTW88 WiFi Driver Installer is an automated installation tool that streamlines the setup of Realtek WiFi 5 drivers on Linux systems. This script handles dependency resolution, kernel module compilation, and secure boot enrollment to enable seamless WiFi adapter support without manual configuration.

**Features**:

- Automated installation of RTW88 Realtek WiFi 5 drivers
- Support for multiple Realtek chipsets (RTL8723DE, RTL8814AE, RTL8821CE, RTL8822BE, RTL8822CE, and USB variants)
- DKMS (Dynamic Kernel Module Support) for automatic rebuilds on kernel updates
- Secure Boot MOK (Machine Owner Key) enrollment support
- Pre-built firmware bundling and modprobe configuration
- Compatibility with Ubuntu 20.04+, Arch Linux, Manjaro, and EndeavourOS
- Support for both 32-bit and 64-bit systems
- Automated post-installation verification

**Motivation**: Linux users often struggle with driver installation for Realtek WiFi adapters, particularly with secure boot configurations and kernel module compilation. This project eliminates the complexity by automating the entire installation process, making it accessible to users of all technical levels.

**Technologies Used**:

- Shell scripting (Bash)
- DKMS (Dynamic Kernel Module Support)
- Kernel module compilation
- Linux package management

**Impact**: The RTW88 WiFi Driver Installer reduces installation friction and empowers Linux users to quickly enable WiFi functionality on their systems without navigating complex compilation and configuration steps. It provides a reliable, reproducible installation method across multiple Linux distributions.

**Website**: [RTW88 WiFi Driver Installer](https://dandanilyuk.github.io/rtw88_driver_installer/)

**GitHub**: [DanDanilyuk/rtw88_driver_installer](https://github.com/DanDanilyuk/rtw88_driver_installer)
