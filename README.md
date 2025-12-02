# Red Specter Email OSINT (redspecter-emailosint)

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


