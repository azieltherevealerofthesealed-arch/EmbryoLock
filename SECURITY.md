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
