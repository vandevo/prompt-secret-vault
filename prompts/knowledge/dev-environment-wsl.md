---
title: "Dev Environment Contract"
version: "1.1"
tags: ["knowledge", "wsl", "environment", "contract"]
author: "Van"
description: "Operational infrastructure documentation for WSL Ubuntu development."
model: "gemini-3-flash"
---

# Dev Environment Contract

**Status**: Active  
**Scope**: All repositories under `/home/vandevo/projects/`

## 1. Environment Rules

- **Host**: All development must occur inside WSL Ubuntu.
- **Path**: Valid root is `/home/vandevo/projects/`.
- **C-Drive Restriction**: No active development allowed in Windows-native directories.
- **De-duplication**: Duplicate repositories on Windows partitions must be deleted or archived.

## 2. Git Discipline

- **Context**: Execute all Git operations within the WSL terminal or Cursor WSL instance.
- **Canonical Source**: GitHub is the singular source of truth.
- **State Verification**:
  - Run `git fetch --all` before starting work.
  - Run `git status` to verify working tree state.
  - Run `git branch` to confirm active branch before commit.
- **Pre-Deploy**: Confirm local `HEAD` matches `origin/main`.

## 3. Commit Workflow

- **Requirements**:
  - Use meaningful commit messages.
  - Generic messages ("update", "fix", "changes") are prohibited.
- **Authorized Tools**:
  - Cursor Source Control (WSL)
  - WSL terminal Git CLI
- **Prohibited Tools**:
  - GitHub Desktop (Windows)
  - PowerShell/CMD Git CLI

## 4. Deployment & State

- **Source**: Production deployment reads from GitHub `main`.
- **Sync**: Cloudflare Pages syncs directly with GitHub.
- **State**: Supabase serves as external state; code remains in Git.
- **Redundancy**: Local machine failure must result in zero data loss on GitHub.

## 5. Risk Controls

- **Diff Review**: Review `git diff` before every commit.
- **Target Verification**: Verify target branch name before every push.
- **HEAD State**: Never work on a detached `HEAD`.
- **Isolation**: Never maintain two active physical copies of the same repository.

---
**Contract active as of migration to WSL Ubuntu.**
