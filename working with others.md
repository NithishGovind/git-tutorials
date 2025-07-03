# Git Branching and Merging Notes

## Description

This repository contains a set of notes on Git branching and merging operations, aimed at developers with at least 5 years of experience. These notes cover common tasks such as creating branches, renaming them, switching between branches, and performing merges. Understanding and mastering these Git operations is crucial for managing complex codebases and collaborating with teams.

## Key Git Techniques Used

- **`git branch`**  
  Lists all the branches in your Git repository. It’s helpful for seeing what branches are available and which one you are currently on.  
  [Git branch documentation](https://git-scm.com/docs/git-branch)

- **`git branch <branch_name>`**  
  Creates a new branch with the specified name. This is used when you want to create a feature branch or any new branch from the current state.  
  [Git branch documentation](https://git-scm.com/docs/git-branch)

- **`git branch -m <new_name>`**  
  Renames the current branch to a new name. Note that HEAD will stay on the same branch while it gets renamed.  
  [Git branch documentation](https://git-scm.com/docs/git-branch)

- **`git branch -d <branch_name>`**  
  Deletes a branch. You need to make sure that you're not on the branch you want to delete before running this command.  
  [Git branch documentation](https://git-scm.com/docs/git-branch)

- **`git status`**  
  Shows the current status of your working directory and staging area, including which branch you are on.  
  [Git status documentation](https://git-scm.com/docs/git-status)

- **`git switch`**  
  Allows you to switch between branches in your repository. This command is a more intuitive alternative to `git checkout` for switching branches.  
  [Git switch documentation](https://git-scm.com/docs/git-switch)

- **`git merge <branch_name>`**  
  Merges the changes from the specified branch into your current branch. Be sure to run this command from the branch you want to merge changes **into**.  
  [Git merge documentation](https://git-scm.com/docs/git-merge)

- **`git diff`**  
  Displays the differences between the current state of your working directory and the index, or between two commits.  
  [Git diff documentation](https://git-scm.com/docs/git-diff)

- **`git diff <branch1> <branch2>`**  
  Shows the difference between two branches. This is helpful for reviewing changes between branches before merging.  
  [Git diff documentation](https://git-scm.com/docs/git-diff)

## Technologies and Libraries

- **Git**  
  The version control system used to manage code changes and branch workflows. If you’re not familiar with the basics or advanced branching, check out the [official Git documentation](https://git-scm.com/doc).

## Project Structure

