# AI Smart Scaffold

> Launch note: The VS Code extension ships first in this public release. The Workbench desktop app and broader runtime surfaces follow after the VS Code rollout.

AI Smart Scaffold is a local-first governed runtime for AI-assisted software development. It acts like an orchestrator between you, your AI tools, and your repository so work is less likely to drift across chats, files, and half-finished handoffs. Planning, execution, verification, and runtime state stay reviewable, recoverable, and easier to finish over time.

---

## 0.1.0 Public Release

Version `0.1.0` is the first public release line.

For early users who begin on or before **June 30, 2026**, the product enters bundled **Tier1** mode during the initial entitlement sync in the same workspace and can remain there for up to **20 days** on that machine, with all bundled introductory access ending no later than **June 30, 2026**. After that introductory Tier1 window ends, the product returns to the Free baseline unless a separate paid Tier1 entitlement is active.

This means early users enter the Tier1 workflow in the same project without creating a second working folder.

Runtime protection stays machine-aware across tiers. AI Smart Scaffold works from a **3-session active baseline** and can temporarily lift the soft ceiling to **4** when the machine has healthy headroom. Separate context budgets help prevent prompt flooding and overloaded long sessions; they are runtime safety controls, not a paid usage meter.

Free is not a soft unlimited mode. It includes a bounded Tier1-preview budget:

- up to **5 premium prompts** per rolling 24-hour window
- up to **8 premium entitlement events** per rolling 24-hour window
- optional **20-minute AI-work duration** cap where telemetry is available
- optional **15-minute first-to-second premium-tool gap** fallback where telemetry is not available

On the first cap hit, runtime behavior falls back to the Free-preview state while keeping machine safety protections and the current workspace active.

---

## What It Does

- **AI orchestration that reduces drift** by keeping planning, execution, verification, and tool activity from quietly wandering apart
- **Structured task lifecycle** so important steps are less likely to disappear when the project gets busy
- **Practical scaffold foundation** for governed work in the same repository you already use
- **Multi-session continuity** with state, recovery support, and better visibility when work stretches across chats
- **Shared notification history across connected product surfaces** so guided actions do not disappear after a single toast
- **Repo change awareness outside the active session** so important created, moved, or deleted files are surfaced as repo notices instead of being pinned to the wrong chat
- **Safer governed-file refreshes** so same-name managed files are less likely to collide with your existing work
- **Tier1 guided workflow support** that gives subscribers deeper help finishing the project when AI output starts to sprawl or stall
- **VS Code extension**, **Workbench desktop app**, and the **governed runtime** working as one product line
- **Local-first support flow** that lets you review a diagnostics bundle before you decide to send it

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
2. **Governed runtime**
3. **Workbench desktop app**

These forms work together, but the **VS Code extension is the first shipped surface** in this release sequence and your project remains in the same workspace.

---

## Local-First Operation

- HSNV ships the scaffold and runtime, not your repository-specific work
- Project files, prompts, and outputs stay local unless you deliberately share support material
- Your own project markdowns and docs stay editable in the same workspace. When the runtime needs follow-up on managed areas or repo structure, it surfaces reviewable notices instead of silently assuming intent.
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
