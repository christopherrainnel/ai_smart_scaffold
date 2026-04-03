# Getting Started with AI Smart Scaffold

AI Smart Scaffold is opinionated by design. You need to keep the folder structure and workflow in place while your project is active. That constraint is intentional because it helps the AI remain consistent across sessions. The common folders most projects need are already included, so you are not starting from zero.

Version `0.1.0` keeps the same workspace on the **Free** baseline until the initial entitlement sync completes. On an eligible first installation, that same workspace then enters **Tier1** immediately and can remain there for up to **20 days**, with all bundled introductory access ending no later than **June 30, 2026**. After that introductory window ends, the workspace returns to the Free baseline unless a separate paid Tier1 entitlement is active.

Runtime protection stays machine-aware while this happens. AI Smart Scaffold works from a 3-session active baseline and can temporarily lift the soft ceiling to 4 when the machine has healthy headroom. Separate context budgets help prevent prompt flooding and overloaded long sessions; they are runtime safety controls, not a paid usage meter.

## Recommended First Steps

Use the **Workbench desktop app** to get connected. It handles the wiring across your AI tools so you do not have to edit configuration files manually.

1. Open the Workbench app.
2. Check the **Dashboard** and review runtime state.
3. If something looks incomplete, run **Doctor**.
4. Open **MCP Connections** and activate the tool you want to use.
5. If Workbench provides an activation prompt, send it inside that AI tool session.
6. Open your project in VS Code and use the extension sidebar to monitor runtime activity.
7. Use **Pause** only when you intentionally want to step outside the governed flow.

Manual MCP JSON editing is still available, but Workbench is the recommended path.

---

## Core Working Model

- Governance is active rather than passive documentation
- Planning, execution, and verification are kept as separate stages
- Workbench connects the tools, the extension shows runtime state, and the runtime enforces the workflow

---

## A Note on Local-First Operation

AI Smart Scaffold runs on your machine.

- Your project files, prompts, and outputs stay local unless you deliberately share them
- If you send material for support or troubleshooting, share only what is needed
- The guardrails materially reduce risk, but they do not eliminate unexpected AI behavior
- Updates come through deliberate installs, not background sync

---

## Read Next

- Installation: `installation.md`
- System requirements: `system-requirements.md`
- Supported tools: `supported-tools.md`
- CLI reference: `cli-reference.md`
