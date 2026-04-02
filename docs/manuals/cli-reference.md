# CLI Reference

While the Workbench app provides a visual interface for managing AI Smart Scaffold, the entire engine is powered by the `gov` CLI. You can use these commands manually in your terminal for deep control, integration into CI/CD pipelines, or scripting.

> Note: Always run these via the bundled Python environment (`python -m gov`) or the compiled broker executable.

## Core Commands

| Command | Purpose |
|---------|---------|
| `gov scaffold` | Materializes the governed folder structure and starter files into a fresh project repository. |
| `gov session` | Refreshes the active session, handles prompt cadence tracking, and records tool activity. |
| `gov check` | Performs deterministic baseline checks on your project to ensure structural adherence. |
| `gov plan` | Validates an upcoming task plan against your project's active rules and policy packs. |
| `gov verify` | Enforces verification gates before an AI agent is allowed to mark a task as complete. |
| `gov resume` | Recovers context and runtime state snapshots after an interruption or workstation switch. |
| `gov status` | Emits a high-signal JSON summary of the current runtime state, blocking warnings, and the next required action. |

## Operations & Diagnostics

| Command | Purpose |
|---------|---------|
| `gov doctor` | Runs health diagnostics across the workspace, checking paths, MCP wiring, and runtime reachability. |
| `gov repair` | Attempts to self-heal missing configuration, update stale schemas, and fix broken wire-ups. |
| `gov broker` | The always-on background hook (used by extensions and MCP) to evaluate rule pre-checks and post-checks. |
| `gov migrate` | Handles trusted automatic migration of data locations (e.g., migrating from legacy local state to shared app data). |
| `gov gc` | Garbage collects stale runtime snapshots, old logs, and safely purges legacy state after migration. |
| `gov serve` | Starts the local HTTP broker server (localhost-only) for tools that cannot use the MCP protocol. |
