# Prompt OS / Secret Vault v2.1

## Overview
This is a **High-Fidelity Prompt Operating System** designed for a sovereign solopreneur. It transforms Cursor from a generic AI editor into a specialized execution engine (CEO, COO, Senior Engineer, and Marketing Director).

## The Master Switch: Core Router
The system is governed by the **`prompts/core-router.md`**. 
To initialize a session with maximum efficiency and zero cognitive drag, always start by loading the router:
`@prompts/core-router.md activate`

## Directory Structure

- `prompts/`
  - `roles/`: Core identities (e.g., `ai-cofounder v3.2`, `unified-operator v3.0`).
  - `tasks/`: Actionable engines (e.g., `solopreneur-engine v1.0`, `email-engine v1.1`).
  - `knowledge/`: Grounding data (e.g., `stack-audit-2026`, `operator-truth v1.0`).
  - `tools/`: Workflow automation (e.g., `session-wrapup v1.1`, `thread-launcher v3.1`).
- `archives/`: Versioned session handovers for context continuity.
- `resources/`: Raw research, logs, and deep-dive materials.

## Technical Stack (Feb 2026)
- **Fast Model**: Gemini 3 Flash (Daily execution).
- **Smart Model**: Gemini 3 Pro (Architecture/Logic).
- **Senior Model**: Claude Opus 4.6 (Agentic coding/Refactors).
- **Primary Stack**: Cloudflare Pages + Supabase (New) / WordPress + FluentCRM (Legacy).

## Maintenance & Update Protocol
Whenever the system undergoes a structural change (new prompt, retired tech, model update), follow this protocol:

1. **Update Knowledge**: Ensure `prompts/knowledge/stack-audit-2026.md` reflects the change.
2. **Update Router**: Adjust `prompts/core-router.md` if modules or modes change.
3. **Sync README**: Update this file to maintain a high-level overview.
4. **Wrap Up**: Run `@prompts/tools/session-wrapup.md` to secure the new state.

### "Update README" Command
When the user says **"Update README"**, the Agent must:
1. Scan the `prompts/` directory for new/deleted files.
2. Verify version numbers in YAML frontmatter.
3. Cross-reference the current `stack-audit-2026.md`.
4. Rewrite the README to match the absolute current state of the ecosystem.

---

`VanOS v2.1 Ready`
*Clarity. Control. Freedom.*
