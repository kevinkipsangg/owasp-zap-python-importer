# OWASP ZAP Python Report Importer

A Python cybersecurity tool for importing OWASP ZAP HTML security reports, extracting vulnerability findings, classifying security risks and exporting results into CSV format.

## Project Overview

This project automates the collection and organisation of security findings from OWASP ZAP reports. It helps cybersecurity learners and security professionals maintain structured records of authorised security assessments.

## Features

- OWASP ZAP HTML report parsing
- Vulnerability extraction
- Risk classification
- Target URL validation
- CSV report generation
- UTC timestamps
- Duplicate finding detection
- CSV formula injection protection
- Error handling
- Remote target authorisation option

## Technologies

- Python 3
- HTMLParser
- CSV
- Regular Expressions
- Argparse
- IP Address Validation

## Installation

Clone the repository:

```bash
git clone https://github.com/kevinkipsangg/owasp-zap-python-importer.git
cd owasp-zap-python-importer
```

## Usage

Import a report from an authorised local testing environment:

```bash
python import_zap.py zap-report.html
```

Specify an output file:

```bash
python import_zap.py zap-report.html --output findings.csv
```

For explicitly authorised remote assessments:

```bash
python import_zap.py zap-report.html --authorize-remote
```

## Output

The application exports findings into a CSV file containing:

- Timestamp
- Finding name
- Target URL
- Risk level
- Confidence
- Evidence
- Description

## Security Notice

This application processes existing OWASP ZAP HTML reports. It does not perform vulnerability scanning itself.

Only assess systems you own or have explicit permission to test. Treat exported vulnerability reports as confidential.

## Future Improvements

- Security findings dashboard
- HTML and JSON report support
- Advanced vulnerability analytics
- More automated tests
- Improved report compatibility

## Author

**Kevin Kipsang**

GitHub: https://github.com/kevinkipsangg

## Licence

MIT License
