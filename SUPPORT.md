# Support

> Launch note: The VS Code extension is the first shipped surface. Early users who begin on or before **June 30, 2026** enter **Tier1** during the initial entitlement sync in the same workspace and can remain there for up to **20 days**, with all bundled introductory access ending no later than **June 30, 2026**.

For product questions, installation issues, or support requests:

- Email: `inquiry@hsnexus.com`

Recommended first references:

- `README.md`
- `docs/manuals/main-instructions.md`
- `docs/manuals/installation.md`
- `docs/manuals/system-requirements.md`
- `docs/manuals/supported-tools.md`
- [Current pricing](https://www.hsnexus.com/pricing)

## Runtime Protection and Capacity

- AI Smart Scaffold keeps runtime concurrency machine-safe. The current runtime starts from a 3-session active baseline and can temporarily lift the soft ceiling to 4 when the machine has healthy headroom.
- Separate context budgets help prevent prompt flooding, oversized governance payloads, and overloaded long sessions. These budgets are runtime safety controls, not a paid-usage meter.
- Tier1 adds deeper guidance and workflow value designed to help you finish real projects, but it does not disable machine-safety protections.
- Free users have bounded preview access to selected Tier1-depth features:
  - up to **5 premium prompts** per rolling 24-hour window
  - up to **8 premium entitlement events** per rolling 24-hour window
  - optional **20-minute AI-work duration** cap where trusted telemetry is available
  - optional **15-minute first-to-second premium-tool gap** fallback where duration telemetry is not available
- Main status surfaces show entitlement state as `free`, `free-preview`, `tier1`, or `tier1-expired` so users can always tell current effective capability at a glance.

## Notifications and Drift Reduction

- As connected product surfaces are used together, AI Smart Scaffold keeps the same product-only notification history visible so runtime alerts and guided actions do not disappear after one dismissed toast.
- If important repo files are created, moved, or deleted outside the active governed session, AI Smart Scaffold raises a repo-scoped notice instead of blaming the current chat box for work it did not do.
- Supported notifications can be resolved in one product surface and reflected in another on refresh.
- Your own project markdowns remain editable. AI Smart Scaffold is there to guide and surface follow-up, not to freeze your docs.

## Common Issues

### I saw a repo change or FILE_MAP alert even though this chat did not edit files

**Cause:** The runtime detected a FILE_MAP-relevant file create, move, or delete outside the active governed session, such as another tool, a pull, a scaffold refresh, or a manual file operation.

**Fix:** Open the notification center, review the notice, and choose the matching action. If the change is important project structure, update the relevant repo docs so the runtime and the repo stay aligned.

## Frequently Asked Questions

**Q: Why do notifications show up in more than one product surface?**
A: When you use connected product surfaces together, AI Smart Scaffold keeps a shared product-only notification feed in local runtime state so important alerts, repo notices, and guided actions stay visible instead of disappearing with one dismissed toast.

**Q: What happens if files change outside the active chat session?**
A: AI Smart Scaffold raises a repo-scoped notice instead of pinning that obligation to the wrong chat. That helps you catch important created, moved, or deleted files without turning every repo change into the wrong closeout debt.

**Q: Can I still edit my own markdown docs?**
A: Yes. Your project-authored markdowns remain yours to edit in the same workspace. AI Smart Scaffold surfaces follow-up when managed areas or repo structure need review, but it does not require you to move into a second working folder just to keep writing docs.
