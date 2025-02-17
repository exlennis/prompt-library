---
title: Fix Spelling and Grammar - Editable
version: 1.0
last_updated: 2025-02-13
category: Writing
sub_category: Proofreading
description: Correct grammatical errors and convert to Australian English spelling, preserving formatting.
keywords:
  - grammar
  - Australian English spelling
  - correction
  - editing
source: [https://ray.so/prompts]
models:
  - GPT-4o
  - Claude 3.5
recommended_presets:
  creativity: 1/5
variables:
  {{selection}}:
    type: string
    description: The text that needs to be corrected
    example: "This is a text with speling and grammer errors."
  {{maintainOriginalLanguage}}:
    type: boolean
    description: Flag to preserve the original language of the text
    example: true
  {{replyWithRewrittenText}}:
    type: boolean
    description: Flag to indicate if the response should only contain the rewritten text
    example: true
  {{maintainURLs}}:
    type: boolean
    description: Flag to preserve any URLs in the text unchanged
    example: true
---

# Fix Spelling and Grammar - Editable

Correct grammatical errors and convert to Australian English spelling, preserving formatting.

---

## Structured Prompt

```markdown
Act as a spelling corrector and improver. {{replyWithRewrittenText}}

Strictly follow these rules:
- Correct spelling, grammar and punctuation
- Enforce Australian English spelling and YYYY-MM-DD date format
- {{maintainOriginalLanguage}}
- NEVER surround the rewritten text with quotes
- {{maintainURLs}}
- Don't change emojis

Text: {{selection}}

Fixed Text:
```

### Example Input

```markdown
Text: This is a text with speling and grammer errors that need's fixing! http://example.com 👍
```

### Example Output
```markdown
Fixed Text: This is a text with spelling and grammar errors that needs fixing! http://example.com 👍
```

---


### Notes:
- Boolean type variables

### Metadata:
- **Category**: Writing — Proofreading
- **Model**: GPT-4o, Claude 3.5;
- **Creativity**: 1/5 (low)
- **Source:** [Raycast Prompt Library](https://ray.so/prompts)

---

**v1.0** — Updated **2025-02-13**
