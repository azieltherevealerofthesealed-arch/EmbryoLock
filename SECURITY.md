# Security Policy

## Supported Versions
Only the latest release and the `main` branch are actively supported.

Older versions may contain known or unknown vulnerabilities and should
not be relied upon for secure deployments.

## Reporting a Vulnerability

If you believe you have found a security vulnerability in EmbryoLock:

- **Do NOT open a public issue**
- Do NOT disclose details publicly before coordination

Instead, use one of the following:
- GitHub Security Advisories (preferred)
- Or contact the repository owner privately via GitHub

Please include:
- A clear description of the issue
- Steps to reproduce (if applicable)
- Potential impact assessment

## Disclosure Process

- Reports will be acknowledged as reasonably possible
- Valid issues will be investigated and addressed
- Fixes may be released silently or with minimal disclosure
  when appropriate to reduce exploit risk

## Automation and CI Security

- GitHub Actions are restricted by allowlist
- All actions are pinned to full-length commit SHAs
- Forked pull requests require explicit approval before workflows run
- Automation cannot bypass branch protection or human review

## Project Security Model

EmbryoLock is designed around:
- Open-source transparency
- Constrained execution
- Immutable release artifacts
- Human-controlled trust boundaries

Security is treated as a property of structure, not secrecy.

Thank you for helping keep this project safe.





updated 1/17/26
____________________________________________________________________________________
# Security Policy

## Scope and Intent

EmbryoLock is a **local file vault** designed around a specific threat model:

**Primary goal:**  
Prevent *post-unlock*, *delayed*, or *casual* access to sensitive data by ensuring failed authentication attempts permanently destroy the encrypted payload.

This tool intentionally prioritizes **data destruction over recovery** in certain threat scenarios.

## Threats Considered In Scope

- Theft of a device *after* a vault has been created
- Delayed access attempts where the unlock window has passed
- Casual forensic inspection
- Opportunistic attackers without unlimited offline resources

## Threats Explicitly Out of Scope

EmbryoLock is **not designed** to protect against:

- Unlimited offline cloning of the vault
- Offline brute-force attacks at scale
- Attackers who can freely duplicate the vault and retry indefinitely
- Live malware, keyloggers, or compromised operating systems
- Advanced surveillance or memory inspection attacks

If an attacker can repeatedly clone the vault and attempt passwords offline, security reduces to the strength of the password and KDF alone. In such cases, this tool is **not appropriate**.

## Design Trade-offs

This project intentionally accepts the following trade-off:

> **Loss of data is preferable to unauthorized access.**

Users should assume:
- Failed authentication attempts may irreversibly destroy data
- Accidental lockout is possible
- Strong passwords are critical

## Responsible Disclosure

If you discover a security issue, design flaw, or implementation bug:

- Please open a GitHub issue **or**
- Contact: **security@azieltherevealerofthesealed@gmail.com
No bug bounty program is offered at this time.

## Disclaimer

This project is provided **as-is**, without warranty.  
It should not be used as a general-purpose secure storage solution or a replacement for established, audited encryption tools.
