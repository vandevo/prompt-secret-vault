---
title: "Session Wrap-up"
version: "1.0"
tags: ["ops", "git", "archive", "handover"]
author: "Van"
description: "Automates the process of generating a handover, archiving it to a file, and syncing to GitHub before clearing context."
model: "gemini-2.0"
---

# Session Wrap-up Tool

## Purpose
To eliminate the manual steps of saving conversation context. This tool ensures that every session is recorded, versioned, and synced with one command.

## Activation
Triggered by keywords: **"Wrap up"**, **"Session Wrap-up"**, or **"Execute Handover"**.

## Protocol

### 1. Generate Handover
Immediately execute the `prompts/tools/thread-handover.md` protocol using the current thread context.

### 2. File Creation
Save the output to the `archives/` directory.
**Naming Convention**: `vX.X-label-YYYY-MM-DD.md` (e.g., `archives/v1.0-setup-2026-02-08.md`).
The `vX.X` and `label` should be derived from the current session's progress.

### 3. Git Sync
Run the following shell commands:
1. `git add archives/`
2. `git commit -m "archive: [vX.X] [label] short description"`
3. `git push origin main`

### 4. Verification & Exit
1. Confirm the file path and GitHub sync status.
2. Provide the "Operator Take" from the handover.
3. Explicitly state: "Context secured. You may now clear the chat."

## Negative Constraints
- Do NOT ask for confirmation of the file name.
- Do NOT skip the Git push.
- Do NOT leave the session without the "Context secured" confirmation.
