---
layout: project
title: 'Wi-Fi QR Generator'
date: 2024-05-15 13:01:12 -0400
categories: project
image: /images/wifi_qr_cover.svg
---

[![Wi-Fi QR Generator](/images/wifi_qr_cover.svg)](https://dandanilyuk.github.io/wifi_qr_generator/)

**Description**: Wi-Fi QR Generator creates QR codes that join a Wi-Fi network the moment they are scanned. Type a network into the static web app by hand, or run the companion shell helper to autodetect the network you are already connected to and open the app with everything prefilled. Finished codes can be copied, downloaded as PNG, or exported as a printable PDF card.

**Features**:

- Form-based QR generation for WPA/WPA2/WPA3, WEP, and open networks, including hidden SSIDs
- Cross-platform shell helper that autodetects the current network on macOS, Linux (NetworkManager), and Windows
- Reads the password from the macOS Keychain when available, with a hidden prompt as the fallback
- "Copy Setup Link" produces a shareable URL that prefills the form on the recipient's end
- Copy to clipboard, PNG download, and printable PDF card export
- Dark and light theme that follows the system preference
- Works offline once loaded, with no analytics and no backend
- Warns when an enterprise 802.1X network is detected, since Wi-Fi QR codes cannot join those

**Motivation**: Sharing Wi-Fi usually means dictating a long password character by character. A QR code lets any modern phone join through its camera in one gesture. The shell helper removes the last bit of typing by pulling the SSID, security type, and password straight from the operating system.

**Technologies Used**:

- HTML, CSS, and vanilla JavaScript, fully client-side
- QRCode.js for QR generation and jsPDF for the printable card
- Bash helper using `networksetup`, `ipconfig`, and the Keychain on macOS, `nmcli` on Linux, and `netsh` via PowerShell on Windows
- URL parameters as the handoff between the shell helper and the web app

**Impact**: Wi-Fi QR Generator removes the friction of getting guests online in homes, offices, and rentals. Nothing about the network ever leaves the browser, so sharing access does not mean surrendering the password to a third-party service.

**Website**: [dandanilyuk.github.io/wifi_qr_generator](https://dandanilyuk.github.io/wifi_qr_generator/)

**GitHub**: [DanDanilyuk/wifi_qr_generator](https://github.com/DanDanilyuk/wifi_qr_generator)
