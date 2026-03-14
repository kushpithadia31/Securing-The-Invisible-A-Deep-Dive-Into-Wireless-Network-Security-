# Securing-The-Invisible-A-Deep-Dive-Into-Wireless-Network-Security-
# 🌐 Cisco Cybersecurity: Enterprise Wireless Security Framework
> **Module:** Wireless Network Communication | **Course:** Cisco Cybersecurity Essentials

[![Cisco Certified](https://img.shields.io/badge/Certification-Cisco%20Networking%20Academy-005A70?style=for-the-badge&logo=cisco)](https://www.netacad.com/)
[![Security Level](https://img.shields.io/badge/Security-Hardened-success?style=for-the-badge&logo=polkadot)](https://github.com/)
[![Lab Environment](https://img.shields.io/badge/Environment-Packet%20Tracer%208.2-orange?style=for-the-badge&logo=cisco)](https://www.netacad.com/courses/packet-tracer)

---

## 📑 Table of Contents
- [Executive Summary](#-executive-summary)
- [Project Architecture](#-project-architecture)
- [The CIA Triad in Wireless](#-the-cia-triad-in-wireless)
- [Encryption Deep-Dive](#-encryption-deep-dive)
- [Attack Simulation & Mitigation](#-attack-simulation--mitigation)
- [Enterprise Hardening Guide](#-enterprise-hardening-guide)


---

## 📖 Executive Summary
Wireless networks are the most vulnerable entry points in the modern enterprise perimeter. This project, based on the **Cisco Cybersecurity Essentials** curriculum, explores the protocols, vulnerabilities, and defense mechanisms required to secure **IEEE 802.11** communications. 

We transition from basic **PSK (Pre-Shared Key)** setups to **Enterprise-grade 802.1X/EAP** authentication models to ensure robust data privacy.

---

## 🏗️ Project Architecture
The project simulates a corporate environment featuring:
* **WLC (Wireless LAN Controller):** Centralized management for Access Points.
* **RADIUS Server:** For per-user AAA (Authentication, Authorization, and Accounting).
* **VLAN Segmentation:** Separating `Management`, `Corporate`, and `Guest` traffic.

---

## 🛡️ The CIA Triad in Wireless
How we apply the core pillars of Cybersecurity:

| Pillar | Wireless Application |
| :--- | :--- |
| **Confidentiality** | Enforcing **AES-CCMP** encryption to prevent eavesdropping. |
| **Integrity** | Using **MIC (Message Integrity Check)** to prevent packet tampering. |
| **Availability** | Mitigating **Deauthentication Attacks** and RF interference. |

---

## 🔐 Encryption Deep-Dive
A comparative analysis of the evolution of wireless security protocols:

### 1. The Legacy Era (WEP & WPA)
* **WEP:** Critical vulnerability in the 24-bit Initialization Vector (IV). Cracked in < 60 seconds.
* **WPA (TKIP):** A temporary patch for WEP hardware. Vulnerable to chop-chop attacks.

### 2. The Modern Era (WPA2 & WPA3)
* **WPA2-AES:** The current industry standard. Uses **Counter Mode Cipher Block Chaining Message Authentication Code Protocol**.
* **WPA3-SAE:** Implements **Simultaneous Authentication of Equals**, eliminating the risk of offline dictionary attacks and providing **Forward Secrecy**.

---

## ⚔️ Attack Simulation & Mitigation
| Threat Model | Description | Defense Implementation |
| :--- | :--- | :--- |
| **Evil Twin** | Attacker mimics a legitimate SSID. | Deploy **Mutual Authentication** (Certificates). |
| **Rogue AP** | Unauthorized AP plugged into the LAN. | Enable **Port Security** and **WIPS** on WLC. |
| **Wardriving** | Discovery of weak APs via high-gain antennas. | Disable SSID Broadcast & adjust Tx Power. |
| **MITM** | Intercepting data between Client and AP. | Enforce **HTTPS/VPN** and WPA3. |

---

## 🛠️ Enterprise Hardening Guide
Steps followed in this project to secure the environment:

1.  **Management Plane:** Changed default credentials and enabled SSH/HTTPS only.
2.  **Data Plane:** Implemented **WPA2-Enterprise (802.1X)** using PEAP.
3.  **Control Plane:** Enabled **Management Frame Protection (802.11w)**.
4.  **Network Segmentation:**
    * `VLAN 10`: Management (Restricted)
    * `VLAN 20`: Employee (Internal Access)
    * `VLAN 30`: Guest (Internet Only / Captive Portal)

---


## 👤 Author 
**Kush Pithadia**
* College Project: Cybersecurity Essentials
* Connect with me on [LinkedIn](https://www.linkedin.com/in/kush-pithadia-966b662bb?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

---
*Disclaimer: This project is for educational purposes only. Unauthorized access to networks is illegal.*
