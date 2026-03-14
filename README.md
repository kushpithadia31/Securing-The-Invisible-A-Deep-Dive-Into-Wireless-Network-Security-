# Securing-The-Invisible-A-Deep-Dive-Into-Wireless-Network-Security-
# 🛡️ Cisco Cybersecurity Essentials: Wireless Network Security
[![Cisco Certified](https://img.shields.io/badge/Certification-Cisco%20Cybersecurity-blue?style=for-the-badge&logo=cisco)](https://www.netacad.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Security Level](https://img.shields.io/badge/Security-Advanced-red?style=for-the-badge)](https://github.com/)

A comprehensive research project and technical guide based on the **Wireless Network Communication** module of the Cisco Networking Academy. This project analyzes the vulnerabilities of RF signals and implements defense-in-depth strategies for modern WLANs.

---

## 📖 Table of Contents
* [Executive Summary](#-executive-summary)
* [Wireless Attack Vectors](#-wireless-attack-vectors)
* [Encryption Evolution](#-encryption-evolution)
* [Lab Simulations](#-lab-simulations)
* [Hardening Checklist](#-hardening-checklist)
* [Technologies Used](#-technologies-used)

---

## 📝 Executive Summary
In a perimeter-less world, wireless signals are the most vulnerable entry point for threat actors. This project explores how to secure the **802.11** standard, transitioning from legacy protocols (WEP) to modern, robust standards like **WPA3**. 

> **Core Objective:** To mitigate unauthorized access and protect Data Confidentiality and Integrity over the airwaves.

---

## 🚨 Wireless Attack Vectors
This module identifies critical threats analyzed during the course:

| Attack Name | Mechanism | Mitigation Strategy |
| :--- | :--- | :--- |
| **Evil Twin** | Spoofed SSID to capture credentials | Use of Digital Certificates/802.1X |
| **WPS Brute Force** | Exploiting the 8-digit PIN vulnerability | Disable WPS on all Access Points |
| **Deauthentication** | Forcing clients off the network | Implement 802.11w (Protected Management Frames) |
| **Wardriving** | Geographic mapping of vulnerable APs | Disable SSID Broadcast & use WPA3 |

---

## 🔐 Encryption Evolution
Security is a moving target. We analyze the cryptographic shift:

1.  **WEP:** ❌ Insecure (24-bit IV is easily cracked).
2.  **WPA/TKIP:** ⚠️ Legacy (Temporary fix for WEP hardware).
3.  **WPA2/AES:** ✅ Current Standard (Uses Counter Mode Cipher Block Chaining Message Authentication Code Protocol).
4.  **WPA3:** 🛡️ Future Proof (Uses **Simultaneous Authentication of Equals (SAE)** to prevent offline dictionary attacks).

---

## 🧪 Lab Simulations
This repository includes a **Cisco Packet Tracer** simulation featuring:
* **WLC (Wireless LAN Controller)** configuration.
* **RADIUS Server** integration for Enterprise authentication.
* **VLAN Segmentation** to isolate guest traffic from corporate data.

`Check the /simulations folder for the .pkt files.`

---

## ✅ Hardening Checklist
A 5-step guide to securing any wireless deployment:
- [ ] **Change Admin Defaults:** Eliminate factory-set passwords.
- [ ] **Firmware Patching:** Regular updates to close zero-day exploits.
- [ ] **Power Level Tuning:** Reduce signal bleed outside the physical building.
- [ ] **Enable WPA3:** If hardware supports it, enforce SAE.
- [ ] **Network Monitoring:** Use IPS/IDS to detect rogue access points.

---

## 🛠️ Technologies Used
* **Networking:** Cisco Packet Tracer, GNS3.
* **Security Tools:** Aircrack-ng (for educational testing), Wireshark.
* **Documentation:** Markdown, LaTeX (for crypto-analysis).

---

## 👤 Author
**Kush Pithadia**
* College Project: Cybersecurity Essentials
* Connect with me on [LinkedIn](https://www.linkedin.com/in/kush-pithadia-966b662bb?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

---
*Disclaimer: This project is for educational purposes only. Unauthorized access to networks is illegal.*
