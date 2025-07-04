# Git Commands Notes

## Description

This repository contains a set of notes for a lecture on common Git commands and concepts used in daily development. These notes are aimed at experienced developers who already have a strong understanding of version control and Git workflows. The commands described in the notes are essential for working with Git in a professional development environment, including handling commits, restoring files, managing detached HEAD states, and more.

## Key Git Techniques Used

- **`git log --oneline`**  
  Displays a simplified commit history with commit IDs. This is useful for getting a quick overview of recent changes in the repo.  
  [Git log documentation](https://git-scm.com/docs/git-log)

- **`git checkout <commit_id>`**  
  Used to switch to a specific commit, detaching the HEAD from the current branch. This is helpful for inspecting older versions of the repository without affecting the current branch.  
  [Git checkout documentation](https://git-scm.com/docs/git-checkout)

- **`git restore`**  
  Restores files to the last committed state. This is especially useful when you have local changes that haven’t been committed yet and need to undo them.  
  [Git restore documentation](https://git-scm.com/docs/git-restore)

- **`git restore --source HEAD~2 <myfile.txt>`**  
  Restores a file from two commits back in the history. This is helpful when you need to roll back specific files without affecting the entire project.  
  [Git restore documentation](https://git-scm.com/docs/git-restore)

- **`git reset`**  
  Resets the current branch to a specific state, while preserving the working directory changes. This is useful if you accidentally committed to the wrong branch and want to move those changes elsewhere.  
  [Git reset documentation](https://git-scm.com/docs/git-reset)

- **`git revert`**  
  Creates a new commit that undoes the changes from the previous commit, allowing you to "revert" a commit without removing it from the history. This is commonly used for undoing changes in a shared repository.  
  [Git revert documentation](https://git-scm.com/docs/git-revert)

## Technologies and Libraries

- **Git**  
  The primary version control system used for managing project history. If you're unfamiliar with advanced Git operations, it's recommended to check out the [official Git documentation](https://git-scm.com/doc).

- **MDN Documentation**  
  For further reading and reference, we link to various MDN docs throughout the notes, especially for web-related topics like CSS and JavaScript features.  
  [MDN Web Docs](https://developer.mozilla.org/en-US/)



