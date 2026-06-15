Learning Git and GitHub
What is Git?

Git is a Version Control System (VCS). It helps developers:

Track changes in code over time
Maintain a history of modifications
Collaborate efficiently with other developers
Revert to previous versions when needed
What is GitHub?

GitHub is a web-based platform that allows developers to store, manage, and share code using Git.

Repository Link:

(Add your repository link here)
Useful Git Commands
1. Check Git Version
git --version
2. Configure Git

Git configuration can be done at two levels:

Global – Applies to all repositories on your computer.
Local – Applies only to the current repository.

Most users use the global configuration.

Global Setup
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
View Configuration
git config --list
Basic Git Commands
Clone a Repository

Clone a GitHub repository to your local machine:

git clone <repository-link>
Change Directory
cd <directory-name>
List Files and Folders
ls

List all files, including hidden files:

ls -a
Check Repository Status
git status
Types of File Status
Untracked – New files that Git is not tracking yet.
Modified – Files that have been changed.
Staged – Files ready to be committed.
Unmodified – Files that have not changed since the last commit.
Add and Commit
Add Files

Add a specific file:

git add <file-name>

Add all files:

git add .
Commit Changes

A commit is a snapshot of your changes.

git commit -m "Your commit message"
Push Changes

Upload local repository content to GitHub:

git push origin main.