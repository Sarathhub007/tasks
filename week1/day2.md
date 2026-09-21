1. GitHub Desktop

GitHub Desktop provides a GUI to perform Git operations such as cloning, branching, committing, pushing, and pulling.

Commands:

git clone <url>
git status
git branch
git switch <branch>
git switch -c <branch>
git add .
git commit -m "message"
git push
git pull
2. Pull Request

A Pull Request is used to propose merging changes from one branch into another for code review.

Workflow:

Branch → Changes → Commit → Push → Pull Request → Review → Merge
3. Merge Conflicts

A merge conflict occurs when Git cannot automatically combine changes, usually because developers changed the same part of a file.

Commands:

git merge <branch>
git status
git add .
git commit -m "Resolve conflict"




git push


Cancel merge:

git merge --abort