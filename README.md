# AI Smart Scaffold

> Launch note: The VS Code extension ships first in this public release. The Workbench desktop app and broader runtime surfaces follow after the VS Code rollout.

AI Smart Scaffold is a local-first governed runtime for AI-assisted software development. It keeps planning, execution, verification, and runtime state disciplined across sessions so AI work stays reviewable, recoverable, and easier to manage over time.

---

## 0.1.0 Public Release

Version `0.1.0` is the first public release line.

For early users who begin on or before **June 30, 2026**, the product enters bundled **Tier1** mode during the initial entitlement sync in the same workspace and can remain there for up to **20 days** on that machine, with all bundled introductory access ending no later than **June 30, 2026**. After that introductory Tier1 window ends, the product returns to the Free baseline unless a separate paid Tier1 entitlement is active.

Runtime protection stays machine-aware across tiers. AI Smart Scaffold works from a 3-session active baseline and can temporarily lift the soft ceiling to 4 when the machine has healthy headroom. Separate context budgets help prevent prompt flooding and overloaded long sessions; they are safety controls, not a paid usage meter.

---

## What It Does

- Governs planning, execution, and verification instead of leaving those steps to memory
- Keeps runtime state visible across sessions and tools
- Provides a practical scaffold foundation for new or existing software projects
- Works through the VS Code extension, the Workbench desktop app, and the governed runtime
- Stays local-first unless you deliberately use optional support or commercial services

---

## Foundational Project Structure

AI Smart Scaffold uses the five folders most software teams already recognize as a practical baseline:

| Folder | Purpose |
| --- | --- |
| `src/` | Functional application logic |
| `tests/` | Validation and regression coverage |
| `docs/` | Technical notes, user guidance, and architecture decisions |
| `scripts/` | Build, setup, and automation helpers |
| `config/` | Centralized project settings and policy |

---

## Product Forms

AI Smart Scaffold is available as:

1. **VS Code extension**
2. **Workbench desktop app**
3. **Governed runtime**

These forms work together, but the **VS Code extension is the first shipped surface** in this release sequence and your project remains in the same workspace.

---

## Local-First Operation

- HSNV shares the scaffold and runtime, not your repository-specific work
- Project files, prompts, and outputs stay local unless you deliberately share support material
- If you send troubleshooting material, keep it minimal and relevant
- Guardrails materially reduce risk, but unexpected AI behavior can still occur and should be reviewed

---

## Getting Started

- `docs/manuals/main-instructions.md`
- `docs/manuals/installation.md`
- `docs/manuals/system-requirements.md`
- `docs/manuals/supported-tools.md`

---

## Release and Legal

- `CHANGELOG.md` and `docs/release-notes/`
- `LICENSE`, `SECURITY.md`, `SUPPORT.md`
- `docs/legal/`
