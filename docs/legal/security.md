# Security Policy

**Product:** AI Smart Scaffold
**Operator:** H&S Nexus Ventures
**Version:** 1.0 (2026-04-01)

---

## Supported Versions

| Version | Supported |
|---------|-----------|
| 0.1.x   | Yes       |
| < 0.1   | No        |

---

## Reporting a Vulnerability

If you discover a security vulnerability in AI Smart Scaffold, we appreciate responsible disclosure. Please do **not** open a public issue.

### How to Report

Email: **inquiry@hsnexus.com**

Include:
- A description of the vulnerability and its potential impact
- Steps to reproduce the issue
- Affected version(s)
- Any suggested mitigation or fix (optional)

### What to Expect

| Step | Timeline |
|------|----------|
| Acknowledgment of report | Within 3 business days |
| Initial assessment | Within 7 business days |
| Status update with remediation plan | Within 14 business days |
| Fix release (critical severity) | As soon as practical, targeting 30 days |
| Fix release (non-critical) | Next scheduled release |

HSNV will keep you informed throughout the process and credit you in the fix release unless you prefer anonymity.

---

## Scope

### In Scope

- The `ai_project_guard` Python package (runtime core, broker, state, CLI)
- The AI Smart Scaffold VS Code extension (`vscode-gov-sidebar`)
- The HTTP broker server (`python -m gov serve`)
- State persistence files (`.ai-project-guard/`)
- Optional license or entitlement services, where offered, and encrypted content delivery

### Out of Scope

- Your own project workspace files and source code
- Third-party AI models, providers, or IDE platforms
- The VibeCoder_Pack development repository infrastructure (CI, GitHub Actions)
- The HSNV website and payment processing (separate security scope)

---

## Security Design Principles

AI Smart Scaffold is built on these security principles:

1. **Local-first** — The runtime is designed to remain on the machine where it is installed. It is not a continuously connected service, and it does not collect repository-specific work as part of normal product use.
2. **Shared scaffold, not shared repository content** — HSNV distributes the scaffold and runtime. Repository-specific code, files, prompts, and outputs remain local unless the user deliberately sends material for support.
3. **No secrets in code** — License key hashes use one-way SHA-256. Machine fingerprints are hashed before any transmission.
4. **Machine-bound introductory access** — The first-install Tier1 promotional window is anchored to machine-local activation markers mirrored across multiple local app-data locations so the earliest valid start date survives partial local marker loss.
5. **Least privilege** — Tool profiles enforce role-based path and command access. Destructive commands are blocked at the execution gate.
6. **Encrypted IP** — Protected scaffold payloads use AES-256-GCM encryption at rest with decryption keys derived from license + salt + machine fingerprint. Decrypted governance payloads used for prompt injection stay in memory, while entitled runtime flows may materialize or refresh HSNV-managed scaffold assets on disk inside the user's existing workspace.
7. **Localhost-only HTTP** — The broker server binds to `127.0.0.1` only. No external network exposure.
8. **Append-only audit** — Broker decisions, tool calls, and bypasses are written to an immutable JSONL audit trail.
9. **Minimized support data** — If troubleshooting requires logs or diagnostic bundles, users should submit only what is necessary. HSNV targets pruning or deletion of that material when the support work is complete, subject to legal or security retention requirements.

---

## Operational Reality

The product includes substantial guardrails, but those guardrails do not eliminate operational uncertainty.

Unexpected behavior can still occur in AI systems, local tooling, or third-party integrations. For that reason, HSNV recommends the following:

- Review important AI-proposed actions before accepting them.
- Avoid sharing more project data than is needed for support.
- Keep sensitive material out of troubleshooting bundles unless it is strictly required.
- Treat updates as deliberate maintenance events rather than continuous remote control of the software on the installed machine.

---

## Responsible Disclosure Policy

- We ask that you give HSNV reasonable time to investigate and address the issue before public disclosure.
- We will not take legal action against researchers who follow responsible disclosure in good faith.
- If a vulnerability affects users, we will notify affected users in accordance with applicable data protection laws.

---

## Contact

H&S Nexus Ventures
Email: inquiry@hsnexus.com
