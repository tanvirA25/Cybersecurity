# 🔐 Artemis Penetration Testing Report

This repository contains the detailed technical report of a comprehensive penetration test conducted for **Artemis**, a natural gas company serving over **1.7 million customers**. The goal was to assess the network's security posture, identify vulnerabilities, and provide actionable remediation strategies.

---

## 📌 Project Overview

- **Client**: Artemis (Natural Gas Provider)
- **Scope**: Internal & external network, web apps, and cloud infrastructure
- **Testing Type**: Grey-box
- **Standards Used**: OSSTMM, OWASP Testing Guide, NIST SP 800-115

---

## 🧭 Methodology

The penetration test followed a four-phase methodology:

| Phase | Description |
|-------|-------------|
| **1. Reconnaissance** | Collected open-source intelligence (OSINT) from social media, DNS records, leaked credentials, and network traffic. |
| **2. Target Scanning** | Identified live hosts, open ports, and services using Nmap, Zenmap, Armitage, and Telnet. |
| **3. Vulnerability Scanning** | Used OpenVAS, Burp Suite, Wapiti, and Metasploit to identify exploitable weaknesses and CVEs. |
| **4. Threat Assessment** | Assessed the risks using OWASP and CVSS scoring; mapped vulnerabilities to real-world attack vectors. |

---

## 🔎 Key Findings

- ✅ **5 Critical** and **4 High-Risk** vulnerabilities identified
- 🛠️ Major issues included:
  - Unpatched **RDP** services
  - **SQL Injection** flaws in web apps
  - **Default credentials** on Cisco devices
  - **Apache CVE-2019-0211** root privilege risk
  - **AWS misconfigurations** exposing sensitive data
  - **Microsoft Exchange** RCE vulnerability

---

## ✅ Recommendations

- Patch and upgrade vulnerable services
- Apply **network segmentation** to limit lateral movement
- Restrict **public cloud access** and enforce **IAM policies**
- Enable **multi-factor authentication (MFA)**
- Separate critical systems (e.g., Exchange) from external exposure
- Train developers in **secure coding practices**
- Implement regular **vulnerability assessments** and **logging/monitoring**

---

## 📄 Report Contents

- 📘 Scope of Work  
- 🎯 Project Objectives  
- 🧠 Assumptions  
- 📅 Timeline & Phase Breakdown  
- 📊 Summary of Findings  
- 🛡️ Detailed Remediation Plan  

---

## 📁 Files

- `Artemis_PenTest_Report.pdf` – Full report  
- `Penetration_Methodology.png` – Diagram of 4-phase testing strategy  

---
