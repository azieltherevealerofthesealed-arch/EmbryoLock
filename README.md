# EmbryoLock

EmbryoLock is a **local file vault** designed around a narrow security tradeoff:
in certain situations, **irreversible destruction is preferable to delayed access**.

This project is not a general-purpose encryption tool.

---

## Threat Model

### In scope
- Post-unlock device theft
- Delayed or opportunistic access
- Casual or non-expert forensic inspection
- Scenarios where **loss is preferable to later compromise**

### Out of scope
- Unlimited offline cloning
- Live malware, keyloggers, or memory inspection
- Attackers with long-term interactive access
- Nation-state or forensic-lab adversaries

> If an attacker can freely clone the vault and attempt passwords indefinitely,
> security reduces to the strength of the password/KDF alone.

---

## What This Is
- A **destructive-by-design** vault
- A risk-reduction tool for **specific scenarios**
- A learning and exploration project

## What This Is Not
- A replacement for standard encryption tools
- Protection against determined offline brute-force
- Safe against user error

---

## Documentation
- [DESIGN.md](DESIGN.md)
- [LIMITATIONS.md](LIMITATIONS.md)
- [USAGE.md](USAGE.md)
- [FAQ.md](FAQ.md)
- [SECURITY.md](SECURITY.md)

---

## Warning

This tool can permanently destroy data.
Use only if you understand and accept that risk.
