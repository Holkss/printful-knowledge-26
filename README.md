# Printful Knowledge

<p align="center">
  <img src="assets/logo-github.svg" alt="Printful Knowledge logo" width="520">
</p>

**Created by HM**  
Created: **2026-09-21**  
Current version: **1.0.0**

A knowledge-first Printful skill for ChatGPT/Codex-compatible skill hosts.

It helps with Printful products, catalog variants, production methods, branding, print files, mockups, pricing concepts, shipping, fulfillment, stores, orders, and API concepts **without requiring an API key for general knowledge use**.

## Design principles

- Knowledge first; authentication only when a task truly requires private/live account data.
- Dynamic facts are verified instead of frozen as permanent truth.
- No API token belongs in the skill or repository.
- `SKILL.md` stays concise; detailed domain material lives in `references/`.
- Automatic invocation is enabled in `agents/openai.yaml`.

## Repository layout

```text
printful-knowledge-26/
├── assets/
│   └── logo-github.svg
├── skills/
│   └── printful-knowledge/
│       ├── SKILL.md
│       ├── agents/openai.yaml
│       ├── assets/
│       │   └── icon-small.svg
│       └── references/
├── docs/
│   ├── BUILD-BASIS.md
│   ├── BRANDING.md
│   └── TESTING.md
├── CHANGELOG.md
├── LICENSE
├── VALIDATION.md
└── README.md
```

## Installation package

The installable standalone skill is the `printful-knowledge/` folder from `skills/`, packaged as a ZIP with that folder at the archive root.

## API credentials

General use requires **no Printful API key**.

Private account/store/order data and account actions require a separately configured authenticated integration. Do not paste API tokens into ordinary chat.

## Compatibility record

Built against the OpenAI skill format and Printful documentation reviewed on **2026-09-21**. See `docs/BUILD-BASIS.md`.

## Trademark note

Printful is a trademark of its respective owner. This is an independent, unofficial knowledge project and is not affiliated with or endorsed by Printful.

No official Printful logo asset is bundled in this repository.

## License

MIT for repository material to the extent the author has rights to license it. See `LICENSE`.
