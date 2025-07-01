# 📘 Git Basics – Quick Reference

This guide provides essential Git commands for initializing a repository, tracking changes, and pushing to GitHub.

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

## 📝 Recommendations & Tips

- Always run `git status` before committing to see what's staged or modified.
- Use meaningful commit messages (e.g., `"Fix login bug"` instead of `"changes"`).
- Use `.gitignore` to avoid committing unnecessary files (like `node_modules`, `*.log`, etc.).
- Use `git log` to view commit history.
- Consider creating a new branch with `git checkout -b <branch-name>` for new features or fixes.

---

