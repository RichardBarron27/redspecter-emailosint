# 📧 Red Specter Email OSINT
[![Stars](https://img.shields.io/github/stars/RichardBarron27/redspecter-emailosint?style=flat&logo=github)](https://github.com/RichardBarron27/redspecter-emailosint/stargazers)
![Last Commit](https://img.shields.io/github/last-commit/RichardBarron27/redspecter-emailosint)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)
![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20Kali%20-purple)
![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/github/license/RichardBarron27/redspecter-emailosint)


> Part of the **Red Specter** ethical cybersecurity tool suite: Offensive Framework • ScriptMap • Email OSINT


**Passive, safe, domain-based email discovery tool for ethical security analysis.**  
Version: **v0.1 (skeleton)**  
Author: **Richard B (Red Specter)**

---

## Overview

`redspecter-emailosint` is a standalone OSINT tool designed to:

- Discover email addresses related to a domain  
- Classify first-party vs third-party addresses  
- Collect data from:
  - Website crawl  
  - Certificate Transparency logs  
  - Optional theHarvester  
- Produce clean Markdown or JSON reports  

The tool is **non-intrusive, passive, safe**, and intended for:

- Ethical hacking labs  
- OSINT workflows  
- Reconnaissance during authorized penetration tests  

---

## Usage

```bash
redspecter-emailosint [OPTIONS]

-d, --domain <domain>
-m, --mode <safe|normal|aggressive>
--no-ct
--no-crawl
--no-harvester
-o, --output <folder>
-h, --help


redspecter-emailosint -d example.com
redspecter-emailosint -d example.com -m safe
redspecter-emailosint -d example.com --no-ct --no-harvester


Roadmap
v0.1

✓ CLI skeleton
✓ Argument parser
✓ Help menu
✓ Output structure
✓ Safety warnings

v0.2

Implement Certificate Transparency lookup

Implement crawler

Implement harvester integration

Email extraction engine

v0.3

Markdown + JSON report generator

Output formatting polish

Error handling

v1.0

Fully packaged Debian tool

Ready for public release

Potential future submission to Kali Linux

Legal / Ethical Notice

This tool performs passive OSINT only.
No exploitation, no intrusive scanning.

You must have explicit authorization when conducting security testing.
The author assumes no liability for misuse.

License

Released under the MIT License.



---

### 🔗 Explore the Red Specter tool suite

- 🗺 **ScriptMap** – Map, group, and document your security/automation scripts in seconds.  
  https://github.com/RichardBarron27/redspecter-scriptmap

- 🧨 **Red Specter Offensive Framework** – Modular bash framework for recon, web enum, vuln scanning, and more (Kali-friendly).  
  https://github.com/RichardBarron27/red-specter-offensive-framework

- 📧 **Red Specter Email OSINT** – Email-focused OSINT helper for investigators and defenders.  
  https://github.com/RichardBarron27/redspecter-emailosint

Follow the Red Specter project for more ethical cybersecurity tools and playbooks.

