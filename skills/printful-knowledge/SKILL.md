---
name: printful-knowledge
description: >
  Printful knowledge and workflow guidance for products, catalog items, variants,
  printing techniques, placements, branding, print files, mockups, pricing,
  shipping, fulfillment, stores, product synchronization, orders, and Printful
  API concepts. Use whenever a user asks a Printful-specific question or needs
  help deciding how a Printful workflow works. This is a knowledge-first skill:
  it does not require a Printful API key for general guidance. Treat current
  prices, availability, shipping, endpoint behavior, and account-specific facts
  as dynamic and verify them when the task depends on them.
---

# Printful Knowledge

Use this skill as the default domain guide for Printful questions.

## Operating rules

1. Start with knowledge, not authentication.
2. Do not ask for or require a Printful API key for general Printful guidance.
3. Read only the reference file(s) needed for the user's question.
4. Preserve Printful distinctions such as Catalog Product vs Catalog Variant and Product ID vs Variant ID.
5. Treat current prices, availability, shipping, fulfillment, supported techniques, placements, and API behavior as dynamic.
6. For dynamic public facts, verify current official Printful information when tools allow it.
7. For private account facts or account actions, use a separately configured authenticated integration if one is actually available.
8. Never ask the user to paste an API token into ordinary chat.
9. Never claim live account access unless an authenticated integration was actually used.
10. Keep knowledge guidance separate from actions that can change an account, publish content, place orders, or spend money.

## Reference routing

Read the smallest relevant reference set:

- `references/core-concepts.md` — object model and terminology.
- `references/catalog-and-variants.md` — products, variants, regions, and availability.
- `references/printing-branding-files.md` — print methods, placements, branding, and artwork files.
- `references/mockups.md` — mockup concepts and workflow.
- `references/pricing-shipping-fulfillment.md` — cost, shipping, and fulfillment concepts.
- `references/stores-products-orders.md` — stores, sync products, product configuration, and orders.
- `references/live-data-boundary.md` — when public knowledge is enough and when authenticated live data is required.
- `references/source-policy.md` — source priority, freshness, and how to handle changing facts.

## Response discipline

When useful, distinguish:

- **Stable knowledge** — conceptual guidance supported by the references.
- **Current public fact** — a current fact verified from an official public source.
- **Live account fact** — a fact obtained from an authenticated account integration.
- **Dated snapshot** — historical or project data tied to an explicit date.
- **Unknown** — not established by the available source.

Do not turn an unknown or stale fact into a confident current claim.
