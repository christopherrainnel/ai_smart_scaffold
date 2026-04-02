# Privacy Policy

**Product:** AI Smart Scaffold
**Operator:** H&S Nexus Ventures
**Version:** 1.0 (2026-04-01)
**Status:** Public product privacy policy

> This is the **shipped product privacy policy** for AI Smart Scaffold. It is always live and reflects the current product. The development SSOT for legal content is `docs/compliance/PRIVACY.md`.

---

## 1. Who We Are

H&S Nexus Ventures ("HSNV", "we", "us", "our") develops and distributes AI Smart Scaffold, a governed runtime for AI-assisted software development, distributed as a VS Code extension and Python CLI.

Contact: inquiry@hsnexus.com

---

## 2. Scope

This Privacy Policy applies to:

- The AI Smart Scaffold VS Code extension ("Extension")
- The AI Smart Scaffold CLI (`python -m gov`, "Runtime")
- Any optional HSNV-operated services you explicitly connect to through the Software, if and when such services are offered (for example, commercial licensing or entitlement APIs)

This Policy does **not** apply to your own project workspace files. Those remain on your machine and are not part of our normal data collection.

AI Smart Scaffold is designed to operate locally on the machine where you install it. It is not a continuously connected service. Outside optional hosted services, updates, or support submissions that you choose to send, your repository-specific work remains local to you.

---

## 3. Data We Collect

### 3.1 Data You Provide

- **Account and License Information** — when you purchase a subscription: name, email address, payment information (processed by our payment provider, not stored by HSNV), and license key details.
- **Support Requests** — content you provide when contacting HSNV for support.
- **Optional Diagnostic Bundles You Choose to Submit** — if you use the Extension's `SEND BUGS / FEEDBACK` flow, you may choose to submit a locally generated diagnostics bundle to HSNV support over HTTPS. The bundle can include runtime state snapshots, audit logs, prompt-journal files, and your written feedback. It is generated on your machine for review before you confirm upload. You should include only what is needed for troubleshooting. If repository-specific or sensitive material is included, HSNV uses it only for troubleshooting or analysis and targets pruning or deletion once it is no longer needed for that support work.

### 3.2 Data Collected Automatically

The Software operates primarily locally. The current runtime does not require telemetry to function. If optional telemetry or hosted product services are introduced, the categories below describe the intended scope of automatically collected product-usage data:

| Data Type | Description | Identifiable? |
|---|---|---|
| Feature activation events | Which governance stages were triggered | No |
| Error codes and stack fragments | Anonymized error class and location | No |
| Extension version and OS platform | For compatibility analysis | No |
| Session count and duration | How frequently the Software is used | No |

**We do not collect by default:**
- Your source code or project files
- File contents, commit messages, or repository names
- Repository-specific scaffold content you keep locally
- AI prompts or model responses
- Personally identifiable information through telemetry

Optional diagnostic bundles are not automatic telemetry. They are only shared if you deliberately confirm submission.

### 3.3 Optional Service and License Validation Data

If HSNV offers hosted license validation, entitlement, or subscription services and you choose to use them:

- License key hash (one-way), machine fingerprint hash, and subscription status are exchanged.
- No source code or workspace content is transmitted as part of normal validation.
- Validation requests are logged for security and fraud prevention for up to 90 days.

---

## 4. How We Use Your Data

| Purpose | Legal Basis (GDPR) | Legal Basis (DPA 2012 PH) |
|---|---|---|
| Deliver the Software and subscription benefits | Contract performance | Contractual obligation |
| Process payments and manage license keys | Contract performance | Contractual obligation |
| Improve Software reliability via anonymized telemetry | Legitimate interest / Consent | Legitimate purpose / Consent |
| Respond to support requests | Legitimate interest | Legitimate purpose |
| Prevent fraud and unauthorized use | Legitimate interest | Legitimate purpose |
| Comply with legal obligations | Legal obligation | Legal obligation |

---

## 5. Data Sharing

HSNV does not sell your personal data.

We share data only with:

- **Payment processors** (e.g., Stripe), where subscriptions or paid services are offered. Their own privacy terms apply.
- **Infrastructure providers**, where HSNV-hosted services are used. Data is processed under data processing agreements.
- **Legal authorities** — when required by applicable law, court order, or to protect the rights and safety of HSNV, users, or the public.

---

## 6. Data Retention

| Data Type | Retention |
|---|---|
| Account and license data | Duration of subscription + 3 years for tax/legal compliance |
| Support correspondence | 2 years from last contact |
| Raw diagnostic bundle attachments you choose to send | Targeted for pruning or deletion within 30 days after troubleshooting or product-improvement handling is complete, unless a longer retention period is required for security, fraud-prevention, or legal obligations |
| Anonymized telemetry | Aggregated indefinitely; raw events deleted after 12 months |
| License validation logs | 90 days |

After the applicable retention period, data is deleted or anonymized.

---

## 7. Your Rights

Depending on your jurisdiction, you may have the following rights:

### 7.1 Rights Under GDPR (EU/EEA Users)
- **Access** — request a copy of personal data HSNV holds about you
- **Rectification** — correct inaccurate personal data
- **Erasure** — request deletion of your personal data ("right to be forgotten")
- **Portability** — receive your data in a structured, machine-readable format
- **Restriction** — restrict processing in certain circumstances
- **Objection** — object to processing based on legitimate interest
- **Withdraw Consent** — where processing is based on consent, you may withdraw at any time

### 7.2 Rights Under Philippine Data Privacy Act (RA 10173)
- Right to be informed, to access, to correct, to erasure/blocking, to damages, and to lodge a complaint with the National Privacy Commission.

### 7.3 Rights Under CCPA (California, USA)
- Right to know, delete, opt out of sale, and non-discrimination.

To exercise any of these rights, contact inquiry@hsnexus.com. HSNV will respond within 30 days (or as required by applicable law).

---

## 8. Telemetry Controls

The current runtime product does not require telemetry to operate. If HSNV later enables optional telemetry, the product will provide documented controls for enabling, disabling, or configuring it.

In jurisdictions where prior consent is required (for example, under GDPR or ePrivacy rules), telemetry is **off by default** until you explicitly opt in.

---

## 9. Security

HSNV implements appropriate technical and organizational measures to protect your data:

- License key hashes are stored using one-way cryptographic hashing (SHA-256)
- Machine fingerprint data is hashed before transmission
- All communication between the Software and HSNV services, when such services are used, uses TLS 1.2 or higher
- Scaffold content IP is AES-256-GCM encrypted at rest (in VSIX)
- Support material is expected to be minimized before submission and is targeted for pruning when no longer needed

Despite these measures and the runtime guardrails, no system is perfectly secure. Unexpected behavior can still occur in AI tools, local environments, or third-party integrations. Review important outputs and avoid sending more data than needed for support. HSNV will notify affected users of material data breaches in accordance with applicable law.

---

## 10. Children's Privacy

AI Smart Scaffold is a developer tool intended for professional and adult use. HSNV does not knowingly collect personal data from individuals under the age of 18. If you become aware that a minor has provided personal data, contact us at inquiry@hsnexus.com.

---

## 11. International Data Transfers

HSNV is based in the Philippines. If you are located in the EU, EEA, or another jurisdiction with data transfer restrictions, your data may be transferred to the Philippines or to infrastructure providers in other countries.

For EU/EEA users, transfers are conducted under the GDPR's Standard Contractual Clauses (SCCs) or other appropriate safeguards as required.

---

## 12. Changes to This Policy

HSNV may update this Privacy Policy when our practices change or when required by law. For material changes:

- We will notify you via in-product notification or email at least 14 days in advance.
- Continued use of the Software after the effective date constitutes acceptance of the updated Policy.

---

## 13. Contact and Data Protection Officer

For privacy inquiries, data subject requests, or to report a concern:

**H&S Nexus Ventures**
Email: inquiry@hsnexus.com

For EU users who believe their rights have not been adequately addressed, you may lodge a complaint with your local Data Protection Authority.
