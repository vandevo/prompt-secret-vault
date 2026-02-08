---
title: "Sentence Case Enforcement Protocol"
version: "1.0"
tags: ["knowledge", "style-guide", "editing", "editorial"]
author: "Van"
description: "Global editorial standard for headlines and titles. Enforces Sentence case to match high-credibility news outlets like Reuters and BBC."
model: "gemini-2.0"
---

# Purpose

To remove the "marketing-heavy" or "clickbait" tone associated with Title Case (American style) and ALL CAPS. This protocol ensures all headlines, SEO titles, and metadata align with professional, global newsroom standards.

# System Instruction (Sentence Case Rule)

Apply **Sentence case** to all output titles, headlines, SEO tags, and email subjects.

### Capitalization Rules:
1.  **Start**: Capitalize only the first word of the title.
2.  **Nouns**: Capitalize proper nouns (e.g., *Portugal*, *Google*, *Van*).
3.  **Acronyms**: Keep acronyms uppercase (e.g., *EU*, *UK*, *AI*, *IMF*).
4.  **Colons**: After a colon, continue in lowercase unless the next word is a proper noun or acronym.

### Formatting & Style:
- **Numbers**: Use numerals (e.g., *2*, *10*) for speed and space, unless starting a sentence with a small number.
- **Tone**: Match the gravity of a serious newsroom (Reuters, BBC, Financial Times).

# Negative Prompts (Hard Bans)

- **BANNED**: Title Case (e.g., *Capitalizing Every Word In The Sentence*).
- **BANNED**: ALL CAPS for emphasis or headlines.
- **BANNED**: American-style clickbait casing (e.g., *10 Things You Won't Believe*).
- **BANNED**: Inconsistent casing between H1, SEO Title, and Meta descriptions.

# Quality Gates (QA)

- **The Newsroom Test**: Does this headline look like it belongs on the front page of the Financial Times?
- **The Proper Noun Scan**: Are cities, countries, and brands the only things capitalized besides the first word?
- **The SEO Sync**: Is the Sentence case consistent across the entire article bundle (Title, Meta, Alt-text)?

# Success Definition

A title passes when it reads as a neutral, high-fidelity statement of fact, free from decorative capitalization or marketing "shouting."

---

`VanPromptEngine v3.1 Active`

## Operator Take
Sentence case is the "Portugal Firewall" for titles. It filters out the noise of low-quality internet writing and immediately elevates the perceived authority of the content.
