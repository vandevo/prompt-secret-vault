# Prompt Lab

## Directory Structure

- `prompts/`
  - `roles/`: Identities and personas (e.g., Operator, Strategist).
  - `tasks/`: Specific actionable workflows (e.g., Blog Engine, Audit).
  - `knowledge/`: Context, style guides, and static data (e.g., Tech Stack, Brand Voice).
  - `tools/`: Utility prompts (e.g., Summarizers, Formatters).
- `labs/`: Experimental prompts not yet production-ready.

## Universal Prompt Format (Schema)

All prompts must use Markdown with YAML Frontmatter.

```markdown
---
title: "Prompt Title"
version: "1.0"
tags: ["tag1", "tag2"]
author: "Van"
description: "Brief description of what this prompt does."
model: "gemini-2.0" # Optional: preferred model
---

# Identity
...

# Rules
...
```

## Workflow

1. **Draft**: Create new prompts in `labs/`.
2. **Test**: Use Cursor to test the prompt against real inputs.
3. **Promote**: Move to `prompts/` when stable.
4. **Commit**: `git add . && git commit -m "feat: add new prompt"`
