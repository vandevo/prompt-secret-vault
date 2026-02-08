# 🚀 Start Here: Your Prompt Lab

Welcome to your **Cursor-Native Prompt Lab**. This is a dedicated workspace for building, testing, and storing high-quality AI prompts.

## 1. How to Open the Lab
1.  Open **Cursor**.
2.  Go to `File > Open Folder...`
3.  Select `C:\Worktugal apps\prompt-lab`.

> **Tip**: Always open this folder directly. Do not open it as a sub-folder of another project, or the Agent might get confused.

## 2. How to Run the Agent
The Lab is equipped with a **Prompt Engineering Agent**. It lives in Cursor and knows your rules.

**To use it:**
1.  Open the **Cursor Chat** (`Ctrl+L` or `Cmd+L`).
2.  Type a request like:
    *   *"Audit this prompt for clarity."*
    *   *"Refine this draft using the social distribution protocol."*
    *   *"Create a new task prompt for researching competitors."*
3.  The Agent will read your rules in `.cursor/rules/prompt-engineer.mdc` and give you a structured, high-quality response.

## 3. How to Save a New Prompt
1.  Create a **Draft** in the `labs/` folder (e.g., `labs/new-idea.md`).
2.  Write your raw thoughts.
3.  Ask the Agent: *"Refine labs/new-idea.md into a production prompt."*
4.  Save the final result into the correct folder in `prompts/`:
    *   `prompts/roles/`: Identities (Who is the AI?)
    *   `prompts/tasks/`: Jobs (What needs to be done?)
    *   `prompts/knowledge/`: Context (Style guides, facts)

## 4. Coffee Shop Workflow (Laptop Sync)
Since this is a Git repository, you can sync it between your Desktop and Laptop via GitHub.

**On your Desktop (Before leaving):**
1.  Open Terminal (`Ctrl+` `).
2.  Type: `git add . && git commit -m "update prompts" && git push`

**On your Laptop (At the coffee shop):**
1.  Open the `prompt-lab` folder in Cursor.
2.  Open Terminal.
3.  Type: `git pull`
4.  Do your work.
5.  When finished: `git add . && git commit -m "coffee shop edits" && git push`

**On your Desktop (Back home):**
1.  Type: `git pull` to get your coffee shop changes.
