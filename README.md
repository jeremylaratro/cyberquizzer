# Cyberquizzer

Interactive cybersecurity knowledge assessment and interview preparation platform.

## Overview

Cyberquizzer provides comprehensive quiz modules for cybersecurity education, certification prep, and interview preparation. Features 300+ questions across 6 study modules with progress tracking, multiple quiz formats, and detailed explanations.

## Features

### Core Features
- **300+ Multiple-Choice Questions** across 6 study modules
- **Self-Assessment Quizzes** with detailed explanations
- **Progress Tracking** with persistent local storage
- **Difficulty-Based Filtering** (Beginner to Expert)
- **Category-Based Organization** for focused study
- **Timed Quiz Support** for exam simulation
- **Random Question Selection** for varied practice

### Quiz Formats
- **Multiple-Choice Mode**: Immediate feedback with explanations
- **Self-Assessment Mode**: Free-response with key learning points
- **Timed Mode**: Exam simulation with configurable time limits

## Study Modules

| Module | Questions | Description |
|--------|-----------|-------------|
| **Pentesting** | 53+ | Active Directory, Web Apps, Network, Linux, Windows, Mobile, Cloud |
| **Security Engineering** | 50+ | Secure Coding, Architecture, DevSecOps, IAM, Infrastructure |
| **Blue Team / SOC** | 40+ | Incident Response, Threat Detection, SIEM, Forensics |
| **Threat Intelligence** | 35+ | IOCs, Threat Actors, Analysis, Attribution |
| **Threat Hunting** | 30+ | Techniques, Tools, MITRE ATT&CK, Hypothesis-Driven |
| **Cryptography** | 40+ | Algorithms, Protocols, Key Management, PKI |

## Categories

### Pentesting Module
- Active Directory
- Web Application Security
- Network Security
- Linux Security
- Windows Security
- Mobile Security
- Cloud Security (AWS, Azure, GCP)

### Security Engineering Module
- Secure Coding Practices
- Security Architecture
- DevSecOps
- Identity & Access Management (IAM)
- Infrastructure Security
- GRC (Governance, Risk, Compliance)

### Blue Team Module
- SOC Operations
- SIEM Analysis
- Incident Response
- Threat Hunting
- Digital Forensics
- Threat Intelligence Integration

### Hardware/IoT Security
- UART/JTAG/SPI
- Firmware Analysis
- RF/SDR
- RFID/NFC
- Bluetooth Security
- Embedded Systems
- Physical Security

## Question Format

### Multiple-Choice Questions
```
Question: Which type of account is primarily targeted in a Kerberoasting attack?

A) Computer accounts with SPNs
B) User accounts with SPNs (Service Principal Names)  [CORRECT]
C) Domain Controllers only
D) Guest accounts

Explanation: Kerberoasting targets user accounts with SPNs because their
service tickets are encrypted with a password-derived key that can be
cracked offline.
```

### Self-Assessment Questions
```
Question: Explain unconstrained delegation and why it's a security risk.
How would you identify and exploit it?

Key Points:
- Service can impersonate users to any service
- TrustedForDelegation flag in userAccountControl
- Exploitation with printer bug or forced authentication
- Extract TGTs from LSASS memory
- Mitigation: Use constrained or resource-based delegation

[Detailed Answer with commands and techniques]
```

## Difficulty Levels

| Level | Description |
|-------|-------------|
| **Beginner** | Entry-level concepts and fundamentals |
| **Easy** | Basic understanding and terminology |
| **Intermediate** | Practical application and common scenarios |
| **Advanced** | Expert knowledge and complex techniques |
| **Expert** | Advanced techniques and edge cases |

## Interview Preparation

Modules are designed for cybersecurity job interviews:

- **Penetration Tester / Red Team** - Pentesting module
- **Security Engineer** - Security Engineering module
- **SOC Analyst / Blue Team** - Blue Team module
- **Threat Intelligence Analyst** - Threat Intelligence module
- **Threat Hunter** - Threat Hunting module
- **Hardware Security Researcher** - Hardware/IoT module

Each question includes:
- Detailed technical explanations
- Key talking points for interviews
- Commands and tools references
- Real-world scenarios

## Usage

### Web Version
Visit the [Cyberquizzer website](https://jlaratro.us/pages/cyberquizzer.html) for the interactive web interface.

### Local Usage
Clone this repository and open `pentest.html` in a browser for offline access.

```bash
git clone https://github.com/jeremylaratro/Cyberquizzer.git
cd Cyberquizzer
open pentest.html  # or use your browser
```

## Certification Prep

Questions align with common cybersecurity certifications:
- OSCP / OSEP / OSWE
- CEH (Certified Ethical Hacker)
- PNPT (Practical Network Penetration Tester)
- CompTIA Security+ / CySA+ / PenTest+
- GCIH / GPEN / GWAPT
- AWS Security Specialty
- Azure Security Engineer

## Contributing

Contributions welcome! To add questions:

1. Fork the repository
2. Add questions following the existing format
3. Include detailed explanations
4. Submit a pull request

### Question Guidelines
- Use clear, unambiguous wording
- Provide accurate technical explanations
- Include relevant commands and tools
- Match difficulty to expected knowledge level
- Make incorrect options plausible but clearly wrong

## Related Projects

- [iCTF](https://apps.apple.com/app/ictf) - Mobile CTF training app (iOS)
- [jlaratro.us](https://jlaratro.us) - Personal portfolio with additional resources

## License

MIT License - See LICENSE file for details.

## Acknowledgments

- OWASP for security guidelines
- MITRE ATT&CK framework
- Cybersecurity community for challenge inspiration
