# Security Policy

## Reporting a Vulnerability

If you believe you have found a security vulnerability in EmbryoLock, please report it responsibly.

**Do not** open public issues for active vulnerabilities.

### How to Report
- Email: **security@embryolock.dev**  
  (or replace with a monitored address)
- Include:
  - A clear description of the issue
  - Steps to reproduce, if applicable
  - Any relevant logs or proof-of-concept
  - The version or commit hash tested

Reports will be acknowledged when received.

---

## Scope

This project has a deliberately **narrow threat model**.  
Only vulnerabilities that violate the documented design intent are considered in scope.

### In Scope
- Implementation errors that undermine the stated threat model
- Cryptographic misuse (incorrect modes, unsafe parameters)
- Logic flaws that bypass intended destruction behavior
- Vulnerabilities that allow unintended recovery or silent failure

### Out of Scope
- Attacks requiring unlimited offline cloning
- Brute-force attacks limited only by password strength
- Live malware, keyloggers, or compromised operating systems
- Physical access attacks with unrestricted time
- Social engineering or user error

---

## No Bug Bounty

This is an independent project and does not offer a paid bug bounty.
Responsible disclosure is appreciated.

---

## Response Policy

Valid reports will be evaluated based on:
- Severity
- Reproducibility
- Alignment with documented scope

Fixes may be released, documented, or declined depending on impact and design intent.

---

## Disclaimer

This software is provided **as-is**, without warranty of any kind.  
Users are responsible for understanding and accepting the risks outlined in the documentation.
