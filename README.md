# Git Cheat Sheet

Welcome to the Git Cheat Sheet! This cheat sheet provides a comprehensive list of commonly used Git commands for various tasks.
## Cheatsheet By : Abhisheksingh

## Index

- [Getting Started](#getting-started)
- [Basic Snapshotting](#basic-snapshotting)
- [Branching and Merging](#branching-and-merging)
- [Sharing and Updating Projects](#sharing-and-updating-projects)
- [Inspecting and Comparing](#inspecting-and-comparing)
- [Undoing Changes](#undoing-changes)
- [Stashing Changes](#stashing-changes)
- [Additional](#additional)

## Getting Started

### Initialize a Repository
```bash
git init
```
Initialize a new Git repository in the current directory.

### Clone a Repository
```bash
git clone <repository_URL>
```
Create a local copy of a remote repository.

## Basic Snapshotting

### Check Status
```bash
git status
```
Check the status of the working directory and staging area.

### Add Changes to Staging Area
```bash
git add <file_name>
```
Add changes in a specified file to the staging area.

### Commit Changes
```bash
git commit -m "Commit message"
```
Commit changes in the staging area to the repository.

### View Commit History
```bash
git log
```
View the commit history of the repository.

## Branching and Merging

### List Branches (local)
```bash
git branch
```
List all local branches.

### List All Branches (local and remote)
```bash
git branch -a
```
List all local and remote branches.

### Create a New Branch
```bash
git branch <branch_name>
```
Create a new branch with the specified name.

### Switch to a Branch
```bash
git checkout <branch_name>
```
Switch to the specified branch.

### Create and Switch to a New Branch
```bash
git checkout -b <branch_name>
```
Create a new branch with the specified name and switch to it.

### Merge Branches
```bash
git merge <branch_name>
```
Merge changes from the specified branch into the current branch.

### Delete a Branch (local)
```bash
git branch -d <branch_name>
```
Delete the specified local branch.

## Sharing and Updating Projects

### Add a Remote Repository
```bash
git remote add origin <repository_URL>
```
Add a remote repository with the specified URL.

### Push Changes to Remote Repository
```bash
git push -u origin <branch_name>
```
Push changes to the remote repository.

### Pull Changes from Remote Repository
```bash
git pull origin <branch_name>
```
Pull changes from the remote repository.

## Inspecting and Comparing

### View Changes (in working directory)
```bash
git diff
```
View the changes between the working directory and the staging area.

### View Changes (staged for commit)
```bash
git diff --staged
```
View the changes between the staging area and the last commit.

## Undoing Changes

### Discard Changes in Working Directory
```bash
git checkout -- <file_name>
```
Discard changes in the specified file from the working directory.

### Undo Last Commit (Keep Changes)
```bash
git reset HEAD~1
```
Undo the last commit while keeping changes in the working directory.

### Undo Last Commit (Discard Changes)
```bash
git reset --hard HEAD~1
```
Undo the last commit and discard changes in the working directory.

## Stashing Changes

### Stash Changes
```bash
git stash
```
Stash changes in the working directory.

### Apply Stashed Changes
```bash
git stash apply
```
Apply the most recently stashed changes.

### List Stashes
```bash
git stash list
```
List all stashes in the repository.

## Additional

### Rename a Local Branch
```bash
git branch -m <old_branch_name> <new_branch_name>
```
Rename a local branch from old_branch_name to new_branch_name.

### Delete a Remote Branch
```bash
git push origin --delete <branch_name>
```
Delete the specified remote branch.

### Set a Repository's Origin Branch to SSH
```bash
git remote set-url origin <SSH_repository_URL>
```

