# Post-Quantum Cryptography Readiness for Payments

An interactive readiness map for the quantum threat to a payments cryptographic
estate — what a quantum computer breaks, what survives, and the order to fix it.

**🔗 Live dashboard:** https://[your-username].github.io/pqc-payments-readiness/

---

## What this is

A self-directed framework that connects two things most people treat separately:
the **quantum threat** (which cryptographic algorithms fall) and the **payments
estate** (where those algorithms actually live — SWIFT PKI, TLS, code-signing,
HSM keys). The interactive dashboard lets you toggle between the two quantum
algorithms and see the estate respond.

- **Shor's algorithm** breaks asymmetric cryptography (RSA, ECC) — the layer that
  authenticates and secures payments. This is the existential threat.
- **Grover's algorithm** only weakens symmetric cryptography (AES, hashing), which
  larger key sizes already defeat. This is manageable.

## What's inside

- **Threat model** — what breaks (Shor) vs. what survives (Grover)
- **Cryptographic dependency map** — where crypto lives across a payments estate
- **Phased migration roadmap** — inventory & crypto-agility → hybrid pilots →
  production migration → legacy decommission, against the NIST 2030/2035 horizon
- **Target-state standards** — NIST FIPS 203 (ML-KEM), 204 (ML-DSA), 205 (SLH-DSA),
  with CNSA 2.0 Category-5 parameters

## Why it matters now

Harvest-now-decrypt-later: long-lived payment traffic recorded today under RSA/ECC
can be decrypted once a cryptographically-relevant quantum computer exists. The
capture is the attack — so the inventory and crypto-agility work starts now, even
though the quantum computer does not yet exist.

## Scope & honesty

This is a **readiness framework and reference**, not a deployed migration. A quantum
computer capable of breaking RSA-2048 does not exist today — this is a timeline
problem, not a today problem. Standards facts are dated and verified to 2026-06;
re-verify against primary sources (NIST CSRC, NSA CNSA 2.0) before any formal use.

---

*Built as a self-directed project exploring the intersection of post-quantum
cryptography and payments infrastructure.*
