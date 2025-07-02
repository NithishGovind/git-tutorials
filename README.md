# 📘 Git Basics – Quick Reference

This guide provides essential Git commands for initializing a repository, tracking changes, working with branches, and pushing to GitHub.

---

## 📑 Index

- [🔍 Checking Repository Status](#checking-repository-status)
- [🛠️ Initializing a Git Repository](#initializing-a-git-repository)
- [➕ Adding Files to Staging Area](#adding-files-to-staging-area)
- [✅ Committing Changes](#committing-changes)
- [🔗 Working with Remote Repositories](#working-with-remote-repositories)
  - [Check Existing Remotes](#check-existing-remotes)
  - [Add Remote Repository](#add-remote-repository)
- [🚀 Pushing Changes to Remote Repository](#pushing-changes-to-remote-repository)
- [📥 Fetching Changes from Remote Repository](#fetching-changes-from-remote-repository)
  - [Checking Out Fetched Data](#checking-out-fetched-data)
  - [Pulling from Remote Repository](#pulling-from-remote-repository)
- [🌿 Working with Branches](#working-with-branches)
  - [Rename Current Branch](#rename-current-branch)
  - [Create a New Branch](#create-a-new-branch)
  - [Switch to a Branch](#switch-to-a-branch)
  - [List All Branches](#list-all-branches)
- [📝 Recommendations & Tips](#recommendations--tips)

---

## 🔍 Checking Repository Status

```bash
git status
```
- Shows the current state of the working directory and staging area.
- **Note:** If you're not inside a Git repository, this will return an error.

---

## 🛠️ Initializing a Git Repository

```bash
git init
```
- Initializes a new Git repository in the current directory.

---

## ➕ Adding Files to Staging Area

```bash
git add <file-name>
```
- Adds a specific file to the staging area.

```bash
git add .
```
- Adds **all** changes (new, modified, deleted files) to the staging area.

---

## ✅ Committing Changes

```bash
git commit -m "Your commit message"
```
- Records staged changes with a descriptive message.

---

## 🔗 Working with Remote Repositories

### Check Existing Remotes

```bash
git remote -v
```
- Displays the current configured remote repositories.
- If nothing is returned, no remote is set.

### Add Remote Repository

```bash
git remote add origin <repository-URL>
```
- Sets a remote repository (usually from GitHub) named `origin`.

---

## 🚀 Pushing Changes to Remote Repository

```bash
git push -u origin <branch-name>
```
- Pushes commits to the remote repository on the specified branch (e.g., `main` or `master`).
- The `-u` flag sets the upstream branch, so future pushes can use `git push` without additional arguments.

---

## 📥 Fetching Changes from Remote Repository

```bash
git fetch
```
- Downloads commits, files, and refs from a remote repository.
- **Note:** This updates your local repository’s history but does **not** modify your working directory.
- You can view the changes and commit history, but you won’t see the actual files until you check them out.

---

### 🔄 Checking Out Fetched Data

```bash
git checkout origin/main
```
- Lets you view the contents of a remote branch (e.g., `origin/main`) without merging it into your local branch.
- Use this to inspect files or branches fetched from the remote repository.

---

### ⬇️ Pulling from Remote Repository

```bash
git pull
```
- Fetches and **automatically merges** changes from the remote repository into your current working branch.
- Combines `git fetch` + `git merge`.

---

### 🖼️ Git Command Flow Illustration

![Git Command Flow](image.png?raw=true "Git Workflow")

---

## 🌿 Working with Branches

### 🔤 Rename Current Branch

```bash
git branch -m main
```
- Renames the current branch to `main`.
- Useful if your repo defaults to `master` and you want to follow modern naming conventions.

---

### 🌱 Create a New Branch

```bash
git branch <branch-name>
```
- Creates a new branch without switching to it.

Example:

```bash
git branch feature-login
```

---

### 🔁 Switch to a Branch

```bash
git checkout <branch-name>
```
- Switches to the specified branch.

Or create and switch in one step:

```bash
git checkout -b <branch-name>
```

---

### 📋 List All Branches

```bash
git branch
```
- Lists all local branches.
- The currently checked-out branch is marked with an asterisk (`*`).

---

## 📝 Recommendations & Tips

- Always run `git status` before committing to see what's staged or modified.
- Use meaningful commit messages (e.g., `"Fix login bug"` instead of `"changes"`).
- Use `.gitignore` to avoid committing unnecessary files (like `node_modules`, `*.log`, etc.).
- Use `git log` to view commit history.
- Consider creating a new branch with:

```bash
git checkout -b <branch-name>
```

- Great for working on new features or fixes without affecting the `main` branch.

---
