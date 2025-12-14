# Known Limitations

EmbryoLock has significant, intentional limitations.

---

## Security Limitations

- Unlimited offline cloning defeats self-destruct
- Password/KDF strength is the final defense
- Does not protect against live compromise
- Does not prevent restore-and-bruteforce with unlimited access

---

## Usability Risks

- Users may destroy their own data
- No recovery options exist
- Misconfiguration can cause permanent loss

---

## Scope Limitations

If your threat model includes:
- Determined attackers
- Long-term access
- Forensic analysis
- Malware

This tool is not appropriate.

---

## Why These Limitations Exist

The project explores a narrow tradeoff:
reducing risk in constrained scenarios at the cost of recoverability.

That tradeoff is intentional.
