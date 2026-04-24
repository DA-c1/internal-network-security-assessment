# Internal Network Security Assessment Lab

## Overview

This project documents a lab-based internal network security assessment performed within an authorised educational environment. The scenario simulated a corporate Research & Development (R&D) network segment requiring security review before handling sensitive business operations.

The objective was to identify security weaknesses, validate potential attack paths in a controlled setting, and provide remediation recommendations aligned with industry best practice.

This project demonstrates practical exposure to offensive security concepts, Windows environments, networking fundamentals, and professional reporting.

---

## Scope

Assessment scope was limited to:

- Simulated internal R&D subnet
- Windows client and server hosts
- Internal services exposed within test range
- Publicly available reconnaissance sources (OSINT)

Out of scope:

- Social engineering
- Production systems
- Destructive actions
- Data exfiltration
- Unauthorised persistence

---

## Skills Demonstrated

### Security

- Reconnaissance (OSINT)
- Host discovery
- Port scanning
- SMB enumeration
- Vulnerability validation
- Risk assessment
- Security remediation planning

### IT / Infrastructure

- Windows environments
- Domain / workgroup awareness
- Networking fundamentals
- Service identification
- Firewall posture review
- User privilege review
- Documentation

---

## Tools Used

- Nmap
- Legion
- Metasploit (lab environment only)
- WHOIS
- Netcraft
- Nslookup
- Kali Linux
- Windows Command Line

---

## Methodology

### 1. Reconnaissance

Performed passive information gathering using publicly available sources to identify:

- Domain information
- IP ownership ranges
- Public DNS records
- Technology exposure indicators

### 2. Scanning & Enumeration

Internal subnet analysis conducted to identify:

- Live hosts
- Open ports
- Running services
- Hostnames
- Operating systems
- SMB exposure

### 3. Vulnerability Validation

Legacy SMB services were reviewed and tested in a controlled lab environment to validate patching and configuration weaknesses.

### 4. Security Review

Privilege levels, password hygiene, host protections, and firewall posture were reviewed.

### 5. Reporting

Findings were prioritised by risk and mapped to remediation actions.

---

## Key Findings

| Severity | Finding | Impact |
|---------|---------|--------|
| High | Legacy SMB service exposure | Increased risk of remote compromise |
| High | Missing critical patch management | Exploitable known vulnerabilities |
| Medium | Weak password controls | Increased credential attack risk |
| Medium | Excessive administrative privileges | Lateral movement risk |
| Medium | Firewall disabled / misconfigured | Reduced host protection |
| Low | Limited monitoring visibility | Delayed detection capability |

---

## Remediation Recommendations

### Immediate

- Disable SMBv1 / legacy protocols
- Apply security patches
- Re-enable and harden host firewalls
- Remove unnecessary administrator rights

### Short Term

- Enforce strong password policy
- Implement MFA where possible
- Centralise logging
- Regular vulnerability scanning

### Long Term

- Network segmentation
- SIEM monitoring
- Endpoint detection tooling
- Patch management lifecycle

---

## What I Learned

This project strengthened practical understanding of:

- Internal attack surface assessment
- Vulnerability prioritisation
- Windows network enumeration
- Common enterprise weaknesses
- Translating technical findings into business risk
- Writing professional security reports

---

## Screenshots



- ### Network Discovery
Host discovery across internal lab subnet using Nmap.

- <img width="908" height="1081" alt="image" src="https://github.com/user-attachments/assets/1dd9ec3b-ba0b-4dac-8e06-508654cfeeab" />

### Service Enumeration
Open ports and exposed services identified using Legion.

- <img width="940" height="877" alt="image" src="https://github.com/user-attachments/assets/0281d270-a15f-4f8c-be06-8655a2b41e7c" />

### Vulnerability Validation
- A controlled lab simulation validated susceptibility to MS17-010 (EternalBlue), demonstrating risk of unpatched SMB services.
- <img width="940" height="928" alt="image" src="https://github.com/user-attachments/assets/c437727a-937c-49d6-a7bf-43ded1250a5f" />

### Proof of Concept Access
-Successful controlled access achieved within authorised lab scope.
- <img width="940" height="1068" alt="image" src="https://github.com/user-attachments/assets/09f25e60-9552-4e43-86b9-b858a88eb11f" />

### Post-Exploitation Visibility Review Demonstrated potential impact of host compromise in test environment.
- Reviewed accessible internal directories to assess potential business impact and data exposure risk. 
<img width="940" height="1046" alt="image" src="https://github.com/user-attachments/assets/112f237d-5c82-4d9a-be0f-347130a58e8b" />











- Service enumeration
- SMB findings
- Risk summary table



---

## Disclaimer

Completed in an isolated educational lab environment with authorised scope for learning purposes only.

