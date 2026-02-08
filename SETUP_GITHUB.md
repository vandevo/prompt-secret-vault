# Setup GitHub (One-Time)

Since I cannot access your browser to create the repository for you, please follow these steps to publish your Lab to the cloud.

## Step 1: Create Repo
1.  Go to [GitHub.com/new](https://github.com/new).
2.  Repository name: `prompt-lab`.
3.  Visibility: **Private** (Recommended).
4.  **Do NOT** initialize with README, .gitignore, or License (we already have them).
5.  Click **Create repository**.

## Step 2: Connect & Push
1.  Copy the URL of your new repo (e.g., `https://github.com/YOUR_USERNAME/prompt-lab.git`).
2.  Open **Cursor Terminal** in this window (`Ctrl+` `).
3.  Run these 3 commands (replace `URL` with your actual link):

```powershell
git remote add origin https://github.com/YOUR_USERNAME/prompt-lab.git
git branch -M main
git push -u origin main
```

## Step 3: Done
Your prompts are now safe in the cloud. You can clone them to your laptop using:

```powershell
git clone https://github.com/YOUR_USERNAME/prompt-lab.git "C:\Worktugal apps\prompt-lab"
```
