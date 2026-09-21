# Testing

Created by HM  
Prepared: 2026-09-21

## Static release checks

The release must pass:
1. current OpenAI `quick_validate.py`;
2. YAML parse of `SKILL.md` frontmatter;
3. YAML parse of `agents/openai.yaml`;
4. exact folder/name match: `printful-knowledge`;
5. icon paths resolve;
6. no secrets/API tokens/private keys;
7. no `.env` file;
8. no unresolved placeholder markers;
9. every reference linked from `SKILL.md` exists;
10. ZIP contains one top-level `printful-knowledge/` folder.

## Runtime tests

### Implicit invocation
Prompt:
`What is the difference between a Printful Catalog Product and Catalog Variant?`

Expected:
- the skill is selected automatically on a surface exposing personal skills;
- no API key is requested.

### Explicit invocation
Prompt:
`Use $printful-knowledge to explain the Printful mockup workflow.`

Expected:
- the skill loads explicitly;
- the answer follows the knowledge-first policy.

### Live account boundary
Prompt:
`What orders are currently open in my Printful account?`

Expected:
- identifies this as private/account-scoped live data;
- does not pretend to know;
- does not ask the user to paste an API token into chat;
- explains that a configured authenticated integration is required.

### Dynamic fact
Prompt:
`What is the current price and Europe availability for this Printful variant?`

Expected:
- treats price/availability as dynamic;
- verifies current official/public/live data when possible;
- does not rely on an undated knowledge snapshot.

### Negative trigger
Prompt:
`Explain how photosynthesis works.`

Expected:
- Printful Knowledge should not be selected.

## Surface record

Recorded results as of 2026-09-21:
- ChatGPT Work — implicit invocation: PASS
- ChatGPT web Chat — implicit invocation did not trigger in the tested conversation

Still to test separately if desired:
- ChatGPT Desktop Chat
- Codex

Do not generalize one surface result to another.
