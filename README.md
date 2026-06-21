# AI Smart Governance

AI Smart Governance is an account-required governance layer for AI-assisted software development. It helps teams keep AI agents, chat boxes, editor extensions, and repositories aligned so work stays reviewable, recoverable, and safer to finish.

This repository is the public documentation, support, update, and issue-intake surface for the product. It is not the private runtime source repository.

## Product Truth

- Product name: **AI Smart Governance**
- Operator: **H&S Nexus Ventures**
- Website: [hsnexus.com](https://www.hsnexus.com)
- Main product forms: official VS Code extension, plugin/workbench surfaces, CLI/MCP runtime integrations, and hosted account/entitlement services
- Official governance requires sign-in with an H&S Nexus account
- The main governance brain, runtime implementation, entitlement enforcement, backend code, and packaged product builds remain private unless the owners later approve a narrower safe-code release

## Current Public Repo Boundary

This repo is for:

- Product updates and public release notes
- Installation and usage guidance when the official product is available
- Public support, feature requests, and bug reports
- Security reporting instructions
- Commercial and account-tier explanations

This repo is not for:

- Releasing the private governance brain
- Publishing extension, workbench, CLI, MCP, or backend source code
- Publishing entitlement, quota, payment, or license-enforcement internals
- Accepting code contributions that attempt to replace the official product

Selected compatibility layers, schemas, examples, or policy formats may be opened later for inspection if the owners decide they are safe to publish. There is no promise or schedule for that. Monetization and user trust both matter, so public code release decisions will stay deliberate.

## Tiers

| Tier | Price | Account requirement | Daily repo scope | Governed sessions / agents |
| --- | ---: | --- | --- | --- |
| Free | $0/month | Required | First 2 governed repos per account per day | Up to 2 concurrent governed sessions/agents |
| Tier1 | $3/month | Required | Unlimited official-use repo scope | Unlimited official-use governed sessions/agents, subject to safety and abuse controls |

The official product must enforce these limits server-side per user account across devices. Local files or client settings are not the source of truth for commercial access.

## Start Here

- [Account and Tiers](docs/account-and-tiers.md)
- [Product Forms](docs/product-forms.md)
- [Public Roadmap](docs/public-roadmap.md)
- [Support](SUPPORT.md)
- [Security](SECURITY.md)
- [Changelog](CHANGELOG.md)

## Repository Name Note

This repository was previously published under the historical GitHub slug `ai_smart_scaffold`. The public product and repository name are now **AI Smart Governance**.
