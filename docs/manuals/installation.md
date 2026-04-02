# Installation Guide

## Recommended Install Order

1. Install the VS Code extension.
2. Install the Workbench desktop app.
3. Use the packaged runtime components provided with the release.

## VS Code Extension

### Marketplace Or VSIX

You can install the extension through the VS Code extension flow or by direct `.vsix` file:

1. Open VS Code.
2. Go to `Extensions`.
3. Choose `Install from VSIX...` if you are using the packaged file.
4. Select the AI Smart Scaffold `.vsix` release asset.

## Workbench Desktop App

### Windows Review Candidate Flow

For the current `0.1.0` review line, the packaged Workbench assets prepared in the parent repo are Windows installers:

- `.msi`
- setup `.exe`

Install one of them, then launch Workbench and use the dashboard to connect supported AI tools.

## Runtime Package

Use the packaged runtime exactly as distributed with the release assets. Do not mix review assets from different release lines.

## First Launch Checklist

1. Open Workbench.
2. Confirm runtime state is visible.
3. Connect one supported AI tool first.
4. Restart that tool if prompted.
5. Open your project in VS Code and confirm the extension sidebar loads.

## If You Prefer Manual MCP Setup

Workbench is the default setup path. Manual MCP JSON editing remains a fallback for constrained environments, not the primary install flow.
