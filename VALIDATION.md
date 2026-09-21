# Validation report

Created by HM  
Release candidate: 1.0.0  
Validated: 2026-09-21

## Static validation

- **OpenAI quick validator: PASS** — Skill is valid!
- **Frontmatter only name+description: PASS**
- **openai.yaml parses: PASS**
- **short_description length check: PASS**
- **default_prompt mentions $printful-knowledge: PASS**
- **implicit invocation explicitly true: PASS**
- **small icon exists: PASS** — `assets/icon-small.svg`
- **large icon exists: PASS** — `assets/icon-large.png`
- **all linked references exist: PASS**
- **credential/secret scan: PASS**
- **no .env files: PASS**
- **no unresolved placeholder markers: PASS**

## Package integrity

- Standalone ZIP root: `printful-knowledge/`
- Standalone ZIP corruption check: PASS

## SHA-256

- `printful-knowledge.zip`: `a567fab7b15fb3a4dcf8ca2a636638b34f4507c30ce0e42414acbbf36f6c1992`

## Runtime status

- **ChatGPT Work implicit invocation: PASS** — confirmed during pre-release testing on 2026-09-21.
- **ChatGPT web Chat implicit invocation: did not trigger in the tested conversation.** This is recorded as a surface-specific runtime result, not as a skill validation failure.
- Other surfaces remain untested unless separately recorded.

## Validation basis

The OpenAI quick validator used for this build mirrors the official `quick_validate.py` source reviewed on 2026-09-21.
