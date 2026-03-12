---
layout: project
title: 'Wi-Fi QR Generator'
date: 2024-05-15 13:01:12 -0400
categories: project
image: /images/wifi_qr_cover.svg
---

[![Wi-Fi QR Generator](/images/wifi_qr_cover.svg)](https://dandanilyuk.github.io/wifi_qr_generator/)

**Description**: The Wi-Fi QR Generator creates scannable QR codes that let devices connect to a WiFi network without manually entering credentials. It supports two modes: automatic detection of the current wireless network or manual entry of SSID, password, and security type. Generated QR codes can be exported as PDF or image files.

**Features**:

- Auto-detect mode that reads the current wireless network's SSID and security type
- Manual entry mode for SSID, password, and encryption type (WEP, WPA/WPA2)
- Support for hidden network configurations
- Export QR codes as downloadable PDF files via jsPDF
- Export QR codes as downloadable image files
- Shell script component (wifi_gen.sh) for command-line network detection

**Motivation**: Sharing WiFi credentials with guests typically means dictating a long password or writing it down. This tool generates a QR code that any modern smartphone can scan to connect instantly. The auto-detect feature makes it even faster by pulling the current network's details automatically.

**Technologies Used**:

- HTML/CSS/JavaScript
- QRCode.js library for QR code generation
- jsPDF library for PDF export
- Shell scripting (Bash) for wireless network detection

**Impact**: The Wi-Fi QR Generator eliminates the friction of sharing WiFi credentials in homes, offices, and public spaces. Guests can connect by scanning a single QR code instead of typing a complex password.

**Website**: [Wi-Fi QR Generator](https://dandanilyuk.github.io/wifi_qr_generator/)

**GitHub**: [DanDanilyuk/wifi_qr_generator](https://github.com/DanDanilyuk/wifi_qr_generator)
