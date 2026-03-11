# 🛡️ Repository Guide: Scans, Remediations & Case Studies

Welcome to my cybersecurity repository. This repository serves as a practical, hands-on archive of cybersecurity practice that I accumulated and this guide will help you navigate the resources I have compiled.


## 📂 What You Will Find Here

This repository is divided into three core pillars:

### 1. 🔍 Vulnerability Scans & Assessments

This section contains raw and sanitized output from Nessus security assessment tools. It demonstrates my methodology for identifying vulnerabilities across different environments (including cloud infrastructure and enterprise networks).

* **Network & Port Scans:** Nmap scan outputs detailing open ports, service versions, and OS fingerprinting.
* **Vulnerability Assessments:** Reports generated from tools like Nessus or OpenVAS, categorized by CVSS (Common Vulnerability Scoring System) severity.
* **Cloud Configurations:** Scans of Azure environments demonstrating misconfigurations in identity and access management (IAM) or storage accounts.

### 2. 🛠️ Remediations & Hardening Strategies

This directory contains the practical steps and documentation used to close the vulnerabilities found in the scans.

* **Step-by-Step Patching Guides:** Documentation on how to mitigate specific CVEs.
* **Architecture Adjustments:** Explanations for editing the networks to implement Zero Trust principles or network segmentation.

### 3. 📜 Famous Cybersecurity Reports & Case Studies

To understand the current threat landscape, we must study the past. This folder contains my personal analyses and summaries of landmark cybersecurity breaches and industry reports.

* **Incident Post-Mortems:** Deep dives into famous breaches.
* **Threat Actor Tactics:** Breakdowns of how advanced persistent threats (APTs) mapped to the MITRE ATT&CK framework during these historical events.
* **Lessons Learned:** Strategic takeaways on how modern security frameworks (like NIST or CMMC) could have prevented these disasters.

---

## 🧭 How to Navigate the Repository

1. **Start with the Scans:** Navigate to the `/Scans` directory to view the initial assessment of a system. Each scan file includes a brief markdown summary of the target environment.
2. **Review the Fix:** For every scan, there is a corresponding markdown file or script in the `/Remediations` folder linked via the CVE number or system name.
3. **Explore the Case Studies:** Browse the `/Reports` directory for standalone reading on major industry events.
