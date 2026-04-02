# Supported Tools

AI Smart Scaffold uses the Model Context Protocol (MCP) and dedicated hooks to provide a single governance brain across multiple different AI tools and editors.

## Currently Supported Integrations

The Workbench can automatically detect and wire up the following tools:

- **Cursor**
- **Windsurf**
- **VS Code Copilot** (via our native extension)
- **Claude Desktop**
- **Cline**
- **Roo Code**
- **Gemini CLI**
- **Claude Code CLI**

## Installation Scopes

When activating a tool via the Workbench, you may be presented with different installation scopes:

- **Project Scope (Recommended):** Wires the tool to the specific `.venv_run` located inside your current project. This ensures complete isolation.
- **Machine Scope:** Wires the tool to a broader machine-level Python path. Useful for tools like Claude Desktop that operate globally rather than per-folder.

## Tool Safety Profiles

Different tools have different capabilities. AI Smart Scaffold limits what AI agents can do based on matching **Tool Safety Profiles**. For example, an agent using Cline may be trusted to edit front-end files, while a background script may be blocked from running destructive terminal commands.

If you don't see your tool listed here, you may still be able to integrate it via manual MCP JSON configuration or the local HTTP Proxy mode—see the developer docs for more details.
