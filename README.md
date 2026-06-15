# Learning Git and GitHub

## What is Git?

Git is a Version Control System (VCS). It helps developers:

- Track changes in code over time
- Maintain a history of modifications
- Collaborate efficiently with other developers
- Revert to previous versions when needed

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

### Global Configuration

Applies to all repositories on your computer.

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

### Local Configuration

Applies only to the current repository.

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

- **Untracked** – New files that Git is not tracking.
- **Modified** – Files that have been changed.
- **Staged** – Files that are ready to be committed.
- **Unmodified** – Files that have not changed since the last commit.

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

# Common Git Workflow

```bash
git clone <repository-link>

cd <repository-name>

git status

git add .

git commit -m "Add meaningful commit message"

git push origin main
```

---

# Learning Progress

- [x] Installed Git
- [x] Configured Git
- [x] Learned Basic Git Commands
- [ ] Branching
- [ ] Merging
- [ ] Pull Requests
- [ ] GitHub Actions

---

# Repository Purpose

This repository contains my notes, commands, and practice files while learning Git and GitHub.