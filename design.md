# Design Overview

EmbryoLock follows a simple principle:

> The only copy that matters is the one that exists right now.

---

## High-Level Architecture

- Files are encrypted locally using a user-supplied password and KDF
- Authentication attempts are counted
- Exceeding the allowed attempts irreversibly destroys the encrypted data
- No recovery mechanism exists by design

---

## Self-Destruct Model

- Destruction occurs locally
- No network dependency
- No remote kill switch
- No backups generated or stored

The goal is to ensure that **failed access attempts eliminate future access**, not
to harden against unlimited offline analysis.

---

## Design Tradeoffs

Chosen deliberately:
- Simplicity over completeness
- Destruction over recovery
- Clarity over flexibility

Rejected deliberately:
- Automatic backups
- Silent failure modes
- Claims of comprehensive protection
