# Account And Tiers

AI Smart Governance official use requires an H&S Nexus account. The server-side account record is the authority for entitlement and usage limits across devices.

## Free

- Price: `$0/month`
- Requires sign-in
- Limited to the first 2 governed repos per account per day
- Limited to up to 2 concurrent governed sessions/agents
- Intended for real personal work, evaluation, and lightweight governed development

## Tier1

- Price: `$3/month`
- Requires sign-in
- Unlimited official-use governed repos per day
- Unlimited official-use governed sessions/agents
- Still subject to safety, abuse, infrastructure, and fair-use controls

## Enforcement Principle

Usage limits must be enforced by the official hosted entitlement service, not by client-side files alone. The local extension, plugin, workbench, CLI, or MCP surface may display state and cache signed snapshots, but the account service remains the commercial source of truth.

## Backend Work Still Needed

Before broad public release, H&S Nexus Ventures should confirm the Supabase-backed account and entitlement tables support:

- Per-account authentication across devices
- A product SKU for AI Smart Governance Tier1
- Server-authoritative daily repo counters
- Server-authoritative concurrent governed session counters
- Paid Tier1 activation, cancellation, expiry, and downgrade handling
- Audit logs for quota decisions and entitlement changes
