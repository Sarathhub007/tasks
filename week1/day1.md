Git & GitHub — Day 1
1. Git vs GitHub

Git: Version control system used to track code changes locally.

GitHub: Cloud platform used to store Git repositories and collaborate with others.

Git = Tool | GitHub = Online platform

2. Uses of GitHub
Store projects online
Backup code
Collaborate with developers
Share projects
Create branches
Code review using Pull Requests
Maintain project history
Showcase projects
3. Basic Git Workflow
Working Directory
       ↓ git add
Staging Area
       ↓ git commit
Local Repository
       ↓ git push
GitHub
4. Staging Area

The staging area is where we prepare changes before committing them.

git add .

Flow:

Modified → git add → Staged → git commit
5. Git Pull

Downloads the latest changes from the remote repository and updates the local repository.

git pull
GitHub → Local Repository
6. Git Setup

Configure your Git identity:

git config --global user.name "Your Name"
git config --global user.email "you@example.com"
7. Check Git Installation
git --version

Shows the installed Git version.

8. Git Init

Initializes Git inside a project folder.

git init

Creates the .git directory.

9. Git Status

Shows the current state of the repository.

git status

It shows:

Modified → changed files
Staged → ready to commit
Untracked → new files
Branch → current branch
10. Git Commit

Creates a snapshot of staged changes.

git commit -m "Add Git notes"
11. Git Log

Shows commit history.

git log

Short version:

git log --oneline
12. Connect Git to GitHub
git remote add origin https://github.com/USERNAME/tasks.git

Check connection:

git remote -v

origin is the name of the remote repository.

13. Git Branch

View branches:

git branch

The * shows the current branch.

14. Create a Branch
git switch -c feature-name

Older method:

git checkout -b feature-name

Creates a new branch and switches to it.

To rename a branch:

git branch -m new-name
15. git checkout vs git switch
Checkout
git checkout branch-name

Older, multi-purpose command.

Switch
git switch branch-name

Modern command specifically for switching branches.

git switch -c new-branch

Creates and switches to a branch.

16. Git Push

Uploads local commits to GitHub.

git push

First push:

git push -u origin main

Push a specific branch:

git push origin branch-name
17. Git Clone

Downloads an existing GitHub repository.

git clone https://github.com/USERNAME/tasks.git

git init → create a new local repository
git clone → copy an existing repository

18. .gitignore

Specifies files Git should not track.

For Node/Next.js:

node_modules/
.next/
.env
.env.local
.env.development
.env.qa

Never commit passwords, API keys, or database credentials.

19. Git Restore

Discards unstaged changes in a file.

git restore filename
20. Git Diff

Shows exactly what changed.

git diff

Shows unstaged changes.

git diff --staged

Shows staged changes.


importnat commands

git --version
git init
git status
git add .
git commit -m "message"
git log
git remote -v
git branch
git switch branch
git switch -c branch
git push
git pull
git clone URL
git merge branch
git restore filename
git diff