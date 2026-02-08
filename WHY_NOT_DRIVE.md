# Why Not Google Drive?

This Lab is intentionally stored in `C:\Worktugal apps\prompt-lab` (Local SSD) instead of Google Drive. Here is why.

## 1. Speed & Performance
*   **Cursor Indexing**: AI agents need to read thousands of lines of code/text instantly to give smart answers.
*   **Local SSD**: Reading from `C:\` is instant.
*   **Google Drive**: Reading from `Y:\` (virtual drive) requires downloading/streaming files on demand. This makes Cursor slow, buggy, and likely to time out when "reading" your prompt library.

## 2. Data Safety (Sync Conflicts)
*   **Git vs. Drive**: You cannot use Git inside a Google Drive synced folder safely.
    *   Git creates thousands of tiny files in `.git/`.
    *   Google Drive tries to sync them while Git is writing them.
    *   **Result**: Corrupted repository, lost history, and broken files.
*   **The Fix**: We use **GitHub** for syncing. It is designed for code/text projects and handles versions perfectly.

## 3. "Codebase" Mentality
*   Prompts are **code**. They have versions (`v1.0`, `v1.1`), bugs, and dependencies.
*   Google Drive treats files as "Documents" (flat, separate).
*   Git treats files as a "System" (interconnected, history-tracked).

## How to Backup?
Your backup is **GitHub**. It is safer than Drive because it tracks *every single change you ever made*, not just the latest version.
