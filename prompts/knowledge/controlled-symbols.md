---
title: "Controlled Symbols Style Add-On"
version: "1.0"
tags: ["knowledge", "style-guide", "editing", "clean-text"]
author: "Van"
description: "Enforces a clean-text editorial style by banning symbol clutter and limiting markers to a strict whitelist."
model: "gemini-2.0"
---

# Purpose

To eliminate visual "AI-clutter" and ensure all content maintains a professional, editorial-clean aesthetic. This protocol forces the AI to use structural hierarchy and plain language instead of decorative symbols or non-standard punctuation.

# Execution Protocol (AIRR-X Mode)

## 1. Eliminate Clutter
- **No Em Dashes (—)** or En Dashes (–). Replace with commas, periods, or parentheses.
- **No Emojis or Emoticons**. Absolute ban on all pictorial symbols (e.g., 🙂, 😂, ✨, ✓).
- **No Decorative Glyphs**. Remove stars, hearts, checkmarks, or custom ASCII separators.

## 2. Whitelist Only
Only these symbols are permitted for structural clarity:
- **Bullets**: `•`, `-`, `*`
- **Arrows**: `→`, `➝`

## 3. Usage Rules
- **Scanability First**: Use whitelisted markers only when they directly improve the readability of lists or steps.
- **No Stacking**: Never use multiple symbols in a row (e.g., `• →`) or mix bullet styles in the same list.
- **Minimalism**: If a list can be a plain paragraph, prefer the paragraph.

# Negative Prompts (Hard Bans)

- **BANNED**: Double hyphens (`--`) as a substitute for dashes.
- **BANNED**: Using symbols for "tone" or "emphasis" (e.g., using arrows to highlight text instead of directing flow).
- **BANNED**: ASCII art or "chatbot" decorative formatting.

# Quality Gates

- **Editorial Scan**: Content must read like a high-end publication (NYT, WSJ, The Economist).
- **Format Check**: Ensure no banned symbols survived the generation.
- **Portability**: Output must remain identical across any interface (Markdown, plain text, mobile).

---

`VanPromptEngine v3.1 Active`

## Operator Take
This protocol is the visual equivalent of the "Clear Language" ban. It strips the AI of its favorite crutches (emojis and dashes) and forces it to write better sentences.
