# Red Specter Email OSINT

**Version 0.2.0**

Passive, domain-based email intelligence tool for ethical reconnaissance and defensive security analysis.

## Overview

Red Specter Email OSINT is a comprehensive toolkit for authorized security assessments and infrastructure analysis. It provides DNS enumeration, email validation, certificate transparency lookups, and passive reconnaissance capabilities through publicly available data sources.

## Features

### DNS Infrastructure Analysis
- **MX Record Enumeration** - Mail server discovery and configuration analysis
- **SPF Record Analysis** - Sender Policy Framework validation
- **DKIM Configuration** - DomainKeys Identified Mail detection
- **DMARC Policy Review** - Domain-based Message Authentication reporting

### Email Validation & Verification
- **RFC-Compliant Validation** - Syntax and format verification
- **Confidence Scoring** - High/medium/low confidence ratings based on validation depth
- **Catch-All Detection** - SMTP-based catch-all server identification
- **MX Record Verification** - Active mail server validation

### Passive Reconnaissance
- **Certificate Transparency Lookups** - Domain discovery via CT logs (crt.sh)
- **theHarvester Integration** - Passive email harvesting from multiple public sources
- **Multi-Source Aggregation** - Consolidated results from various OSINT sources

### Reporting & Output
- **CSV Export** - Structured data for analysis and tracking
- **JSON Export** - Machine-readable format for integration
- **Text Reports** - Human-readable summary outputs
- **Comprehensive Logging** - Detailed operation tracking

## Installation

\`\`\`bash
git clone https://github.com/RichardBarron27/redspecter-emailosint.git
cd redspecter-emailosint
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
pip install -e .
\`\`\`

## Usage

### Full Infrastructure Scan
\`\`\`bash
redspecter-emailosint scan -d target.com --json --csv
\`\`\`

### Individual Commands
\`\`\`bash
redspecter-emailosint check-mx -d target.com
redspecter-emailosint validate -e user@target.com
redspecter-emailosint ct-lookup -d target.com
redspecter-emailosint check-catchall -d target.com
redspecter-emailosint harvest -d target.com
\`\`\`

## Ethical Use & Legal Compliance

### Authorized Use Only
This tool is designed for:
- Authorized penetration testing engagements
- Defensive security assessments with proper authorization
- Infrastructure analysis of domains you own or have permission to assess

### Prohibited Uses
- Unauthorized reconnaissance of third-party domains
- Spam or unsolicited bulk email campaigns
- Violation of website terms of service

**Always obtain explicit written authorization before use.**

## Testing

\`\`\`bash
pytest
pytest --cov=redspecter_emailosint --cov-report=html
\`\`\`

## Version History

### v0.2.0 (January 2026)
- Complete Python rewrite with modular architecture
- Added comprehensive DNS analysis (MX, SPF, DKIM, DMARC)
- Implemented RFC-compliant email validation with confidence scoring
- Added SMTP-based catch-all detection
- Integrated Certificate Transparency lookups via crt.sh
- Added theHarvester wrapper for passive reconnaissance
- Multi-format output (CSV, JSON, text)
- 53+ unit tests with pytest
- Click-based CLI with multiple subcommands
- Type hints throughout codebase

## License

MIT License - See LICENSE file for details

## Author

**Red Specter Security Research**
- GitHub: [@RichardBarron27](https://github.com/RichardBarron27)

## Disclaimer

This tool is provided for educational and authorized security assessment purposes only. Users assume all responsibility for lawful and ethical use.

---

*Built for the cybersecurity community. Use responsibly.*
