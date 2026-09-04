# Git & GitHub

### Git

Git is a **version control system** used to track code changes and maintain project history.

### GitHub

GitHub is an **online platform** where Git repositories are stored and shared with other developers.

### GitHub Desktop

GitHub Desktop is a **GUI for Git** that helps us manage changes, commits, branches, pushes, pulls, and conflicts without using the terminal.

## Basic Workflow

```text
Edit Code
   ↓
Changes
   ↓
Commit
   ↓
Push
   ↓
GitHub
```

### Commit

A **commit** is a saved snapshot of our changes.

### Push

**Push** uploads our local commits to GitHub.

```bash
git push
```

### Pull

**Pull** gets the latest changes from GitHub.

```bash
git pull
```

## Branches

A **branch** is a separate line of development. Developers use branches to work on features without directly changing `main`.

```text
main
 │
 ├── feature/login
 ├── feature/payment
 └── bugfix
```

Typical workflow:

```text
Create Branch
     ↓
Write Code
     ↓
Commit
     ↓
Push
     ↓
Pull Request
     ↓
Review
     ↓
Merge → main
```

## Merge Conflict

A conflict happens when two branches make **conflicting changes to the same part of the code**, and Git cannot decide which change to keep.

```text
Developer A ──┐
              ├── Merge → Conflict ❌
Developer B ──┘
```

The developer must manually decide the correct code.

## Important Commands

```bash
git init       # Create Git repository
git status     # Check changes
git add .      # Stage changes
git commit     # Save changes
git push       # Upload to GitHub
git pull       # Get latest changes
git branch     # Manage branches
git merge      # Combine branches
```

### Remember

**Git = Version Control**

**GitHub = Online Repository**

**GitHub Desktop = GUI for Git**
