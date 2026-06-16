# Learning Git and GitHub

## What is Git?

Git is a Version Control System (VCS). It helps developers:

* Track changes in code over time
* Maintain a history of modifications
* Collaborate efficiently with other developers
* Revert to previous versions when needed

## What is GitHub?

GitHub is a web-based platform that allows developers to store, manage, and share code using Git.

---

# Useful Git Commands

## 1. Check Git Version

```bash
git --version
```

## 2. Configure Git

Git configuration can be done at two levels:

* Global – Applies to all repositories on your computer.
* Local – Applies only to the current repository.

Most users use the global configuration.

### Global Setup

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

### View Configuration

```bash
git config --list
```

---

# Basic Git Commands

## Clone a Repository

Clone a GitHub repository to your local machine.

```bash
git clone <repository-link>
```

## Change Directory

```bash
cd <directory-name>
```

## List Files and Folders

```bash
ls
```

## List All Files (Including Hidden Files)

```bash
ls -a
```

## Check Repository Status

```bash
git status
```

### File Status Types

* **Untracked** – New files that Git is not tracking.
* **Modified** – Files that have been changed.
* **Staged** – Files that are ready to be committed.
* **Unmodified** – Files that have not changed since the last commit.

---

# Add and Commit

## Add a Specific File

```bash
git add <file-name>
```

## Add All Files

```bash
git add .
```

## Commit Changes

```bash
git commit -m "Your commit message"
```

A commit is a snapshot of your changes.

---

# Push Changes to GitHub

Upload local repository content to a remote repository.

```bash
git push origin main
```

---

# Getting Out of a Directory

```bash
cd ..
```

---

# Creating a New Directory

```bash
mkdir <folder-name>
```

---

# Init Command

Used to create a new Git repository.

```bash
git init
```

---

# Connecting Local Repository to GitHub

Add a remote repository:

```bash
git remote add origin <repository-link>
```

Verify the remote repository:

```bash
git remote -v
```

---

# Check Current Branch

```bash
git branch
```

Earlier, the default branch name was `master`, but now most repositories use `main`.

---

# Rename Branch

```bash
git branch -M main
```

---

# Setting Upstream During Push

```bash
git push -u origin main
```

After doing this once, you can simply use:

```bash
git push
```

instead of:

```bash
git push origin main
```

every time.

---

# Git Workflow

1. Create or clone a repository.
2. Make changes to files.
3. Check status using `git status`.
4. Add changes using `git add`.
5. Commit changes using `git commit`.
6. Push changes using `git push`.

---

# Git Branches

## Check Branches

```bash
git branch
```

## Create a New Branch

```bash
git checkout -b <branch-name>
```

## Switch Branches

```bash
git checkout <branch-name>
```

## Rename Branch

```bash
git branch -M <new-branch-name>
```

## Delete Branch

```bash
git branch -d <branch-name>
```

**Note:** To delete a branch, first switch to a different branch.

---

# Push a Branch

```bash
git push origin <branch-name>
```

---

# Merging Branches

## Compare Branches

```bash
git diff <branch-name>
```

## Merge Branches

```bash
git merge <branch-name>
```

---

# Pull Request (PR)

A Pull Request (PR) allows you to tell others about changes you have pushed to a branch on GitHub. It is commonly used for code review and collaboration.

---

# Pull Command

Used to fetch and download content from a remote repository and update the local repository.

```bash
git pull origin main
```

---

# Resolving Merge Conflicts

Merge conflicts occur when Git is unable to automatically resolve differences between two commits.

---

# Undoing Changes

## Case 1: Staged Changes

For a specific file:

```bash
git reset <file-name>
```

For all files:

```bash
git reset
```

---

## Case 2: Undo Last Commit

```bash
git reset HEAD~1
```

`HEAD~1` means moving one commit back.

---

# Checking Commit History

```bash
git log
```

---

## Case 3: Undo Multiple Commits

Reset to a specific commit:

```bash
git reset <commit-hash>
```

Remove all changes after that commit:

```bash
git reset --hard <commit-hash>
```

**Warning:** This removes changes from both Git history and your local files.

---

# Fork

A fork is a copy of an existing repository.

It allows you to experiment with changes without affecting the original repository. A fork has its own copy of the code and can later be used to contribute changes back through a Pull Request.
