# Git Commands Reference Guide

## Setup & Configuration
* **`git init`**: Initializes a brand new, empty Git repository in the current directory.
* **`git clone <url>`**: Copies an existing remote repository (via HTTPS or SSH) down to your local machine.
* **`.gitignore`**: A configuration file containing a list of file names or folder patterns that Git should ignore and never track.

## Basic Workflow
* **`git add <file-name>`**: Adds a specific modified or new file to the staging area.
* **`git add .`**: Adds all modified, deleted, and new files in the current directory to the staging area.
* **`git commit -m "message"`**: Takes a snapshot of the staged files and commits them to the local repository history.
* **`git push origin <branch-name>`**: Uploads your local committed changes to the remote repository (e.g., GitHub).
* **`git pull origin <branch-name>`**: Fetches new changes from the remote repository and automatically merges them into your local repository.

## File Management
* **`git rm --cached <file-name>`**: Untracks a file from Git's index but leaves the actual file safely on your hard drive.
* **`git rm <file-name>`**: Removes the file from Git's index AND permanently deletes it from your hard drive.

## Viewing History & Undoing
* **`git log`**: Displays the full commit history, including commit IDs (hashes), authors, dates, and messages.
* **`git log --oneline`**: Displays a compressed version of the commit history, showing just the short ID and the message on a single line.
* **`git revert <commit-id>`**: Creates a brand new commit that undoes the changes made in a specific previous commit (safe for public history).

## Branching & Merging
* **`git branch`**: Lists all local branches and highlights the one you are currently working on.
* **`git checkout -b <new-branch-name>`**: Creates a new branch and immediately switches your working directory to it.
* **`git merge <branch-name>`**: Merges the specified branch into your current active branch. *(Example: If you are on `main` and run `git merge feature-a`, the changes from `feature-a` are brought into `main`.)*