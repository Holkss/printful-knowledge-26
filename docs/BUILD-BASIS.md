# Build basis

Created by HM  
Created: 2026-09-21  
Version: 1.0.0

## OpenAI basis

The skill was built against the OpenAI skill-creator guidance reviewed on 2026-09-21:

- `SKILL.md` is required.
- YAML frontmatter uses `name` and `description` only.
- `name` + `description` are the primary trigger metadata.
- `agents/openai.yaml` is used for UI metadata.
- `icon_small`, `icon_large`, `brand_color`, and `default_prompt` are supported UI fields.
- `policy.allow_implicit_invocation` defaults to true; this skill sets it explicitly to true.
- Detailed material belongs in `references/` and should not be duplicated unnecessarily in `SKILL.md`.
- Final structure should be validated with the current OpenAI `quick_validate.py`.

Primary OpenAI sources:
- https://github.com/openai/skills/blob/main/skills/.system/skill-creator/SKILL.md
- https://github.com/openai/codex/blob/main/codex-rs/skills/src/assets/samples/skill-creator/references/openai_yaml.md
- https://help.openai.com/en/articles/20001066

## Printful basis

Primary Printful source entry points:
- https://developers.printful.com/docs/
- https://developers.printful.com/docs/v2-preview/
- https://developers.printful.com/docs/v2-beta/
- https://help.printful.com/

The skill intentionally avoids freezing volatile catalog prices, availability, shipping rates, endpoint schemas, or account state as permanent knowledge.

## Compatibility statement

Correct claim:

> Built and validated against documentation current on 2026-09-21.

Do not claim permanent future compatibility.
