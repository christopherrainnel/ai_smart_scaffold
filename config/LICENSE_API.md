# License Validation API — Integration Spec

> **For AI Smart Scaffold runtime engineers.**
> This document describes how this product calls the H&S Nexus license
> validation API to check the user's entitlement tier on startup and on demand.

---

## Endpoint

```
POST https://www.hsnexus.com/api/license/validate
Content-Type: application/json
```

## Authentication

Include the user's **Supabase access token** in the Authorization header.
This is obtained from the Supabase session after the user signs in via
`hsnexus.com/auth`.

```
Authorization: Bearer <supabase_access_token>
```

The API uses the Supabase Admin SDK server-side to verify the token —
it never asks for the service role key from the client.

---

## Request Body

```json
{
  "sku": "ai-smart-scaffold-tier1"
}
```

| Field | Type   | Required | Description |
|-------|--------|----------|-------------|
| `sku` | string | yes      | The product SKU to check. Use `"ai-smart-scaffold-tier1"` for Tier1. |

---

## Response — Success (200)

```json
{
  "tier": "tier1",
  "status": "active",
  "expires_at": "2026-05-10T00:00:00Z",
  "product": "AI Smart Scaffold",
  "sku": "ai-smart-scaffold-tier1",
  "features": [
    "Unlimited governed sessions",
    "Full Tier1 instruction depth",
    "Priority support",
    "All connected product surfaces"
  ]
}
```

| Field        | Type     | Description |
|--------------|----------|-------------|
| `tier`       | string   | `"free"`, `"tier1"`, or `"enterprise"` |
| `status`     | string   | `"active"`, `"expired"`, `"cancelled"`, `"trial"` |
| `expires_at` | ISO 8601 | When the current period ends. `null` for free. |
| `product`    | string   | Human-readable product name. |
| `sku`        | string   | The validated SKU. |
| `features`   | string[] | Displayable feature list for the active tier. |

## Response — No Active Paid Tier (200)

When the user has an account but no paid entitlement for the requested SKU,
the API returns free baseline:

```json
{
  "tier": "free",
  "status": "active",
  "expires_at": null,
  "product": "AI Smart Scaffold",
  "sku": "ai-smart-scaffold-free"
}
```

## Response — Unauthorized (401)

Token missing, invalid, or expired.

```json
{ "error": "Unauthorized", "message": "Invalid or expired access token." }
```

## Response — Server Error (500)

```json
{ "error": "Internal", "message": "License check failed. Try again later." }
```

---

## How to Call This From the Product

### 1. On startup (extension / Workbench activate)
- Read the stored Supabase session from local storage (if `persistSession: true`).
- If a session exists and `expires_at` is in the future, call the validate API.
- Cache the result locally for up to **5 minutes** to avoid hammering on every prompt.
- If the token is expired, attempt silent refresh via Supabase `refreshSession()`.

### 2. On user-initiated sign-in
- After `signInWithGoogle` / `signInWithGithub` / `signInWithEmail` completes,
  call validate immediately and update the in-app tier display.

### 3. On `hsnexus://auth-callback` URI event (VS Code future)
- The extension can register a URI handler for
  `vscode://hsnexus.ai-smart-scaffold/auth-callback`.
- When the success page triggers this URI after payment, call validate immediately.

---

## Subscribe Flow — How to Open the Funnel

When a Free user clicks "Upgrade to Tier1" inside the app:

```js
// VS Code extension
const uri = vscode.Uri.parse(
  'https://www.hsnexus.com/subscribe/ai-smart-scaffold?source=vscode'
);
await vscode.env.openExternal(uri);
```

The `?source=vscode` parameter lets the success page know to attempt the
`vscode://` callback after payment.

---

## Supabase Project

| Setting | Value |
|---------|-------|
| Project URL | `SUPABASE_URL` (from .env / secure config) |
| Anon key (client) | `SUPABASE_ANON_KEY` |
| Auth providers | Email, Google, GitHub |
| `licenses` table | Source of entitlement truth |

---

## Adding a New Product (Future)

To add a new digital product:
1. Add its SKU and tier definitions to `SITE_CONFIG.commerce.digitalProducts` in `site-config.js`.
2. Add a product row to the `products` table in Supabase.
3. Create a `subscribe/<product-slug>/index.html` page.
4. The validate API is generic — it accepts any registered SKU from the `licenses` table.
   No API code change needed for new products.

---

_Last updated: April 2026 · H&S Nexus Ventures_
