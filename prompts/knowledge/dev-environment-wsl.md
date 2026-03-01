---
title: "Dev Environment Contract"
version: "1.0"
tags: ["knowledge", "wsl", "environment", "contract"]
author: "Van"
description: "Single-environment development and Git workflow contract for WSL Ubuntu."
model: "gemini-3-flash"
---

# Dev Environment Contract

**Status**: Active  
**Scope**: All repositories under `/home/vandevo/projects/`

## Purpose
Define the single development environment, Git workflow, and deployment source of truth to prevent dual-environment corruption.

## Environment Rules

1. **WSL Only**: All development occurs inside WSL Ubuntu.
2. **Valid Root**: The only valid working directory root is `/home/vandevo/projects/`.
3. **No Windows Copies**: No active development is allowed in any Windows C drive copy.
4. **Archive/Delete Duplicates**: If a duplicate Windows repo exists, it must be archived or deleted.

## Git Discipline

1. **Inside WSL**: All Git operations must occur inside WSL.
2. **GitHub is Canonical**: GitHub is the source of truth.
3. **Disposable Local**: The local environment is disposable.
4. **Pre-Change Routine**:
   - `git fetch --all`
   - `git status`
5. **Pre-Deploy Check**:
   - Confirm `HEAD` equals `origin/main`.
   - No split-brain repository state allowed.

## Commit Workflow

- **Allowed**:
  - Cursor Source Control panel (inside WSL)
  - WSL terminal git commands
- **Not Allowed**:
  - GitHub Desktop for WSL repositories
  - Windows PowerShell git for Linux repos

## Deployment Model

1. **Source**: Production reads from GitHub `main`.
2. **Automation**: Cloudflare pulls from GitHub.
3. **State**: Supabase is external state, not source code.
4. **Safety**: Local machine failure must not affect GitHub state.

## Risk Controls

- Never maintain two physical working copies of the same repo.
- Never commit without reviewing diffs.
- Never assume folder sync equals Git sync.
- Always verify branch tracking.

---
**Contract active as of migration to WSL Ubuntu.**
