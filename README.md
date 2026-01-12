# git-cheat-sheet-
this repo contains my git commands for Daly use 

1. Initial Setup (One-time)
git config --global user.name "Your Name"
git config --global user.email "your@email.com"


Check config:

git config --list

🔹 2. Create / Clone Repository
Create new repo
git init

Clone existing repo
git clone git@github.com:username/repo.git

🔹 3. Daily Workflow (MOST USED)

Check status:

git status


Add files:

git add file.txt
git add .


Commit:

git commit -m "Meaningful commit message"


Push:

git push origin branch-name


Pull latest:

git pull origin main

🔹 4. Branching (REAL WORKFLOW)

Create & switch branch:

git switch -c feature-branch


List branches:

git branch


Switch branch:

git switch main


Delete branch:

git branch -d feature-branch

🔹 5. GitHub Pull Request Flow

Push feature branch:

git push origin feature-branch


After PR merge:

git switch main
git pull origin main
git branch -d feature-branch

🔹 6. Remote Repository Commands

Check remote:

git remote -v


Add remote:

git remote add origin git@github.com:user/repo.git


Change remote URL:

git remote set-url origin git@github.com:user/repo.git

🔹 7. Undo / Fix Mistakes (VERY IMPORTANT)

Undo last commit (keep changes):

git reset --soft HEAD~1


Unstage file:

git restore --staged file.txt


Discard local changes:

git restore file.txt

🔹 8. View History & Logs

View commits:

git log


Short log:

git log --oneline


See file changes:

git diff

🔹 9. Merge Branches (Local)
git switch main
git merge feature-branch

🔹 10. Stash (When you’re stuck)

Save work temporarily:

git stash


Restore work:

git stash pop

🔹 11. SSH (GitHub Auth – YOU SET THIS)

Test SSH:

ssh -T git@github.com

🔹 12. Common Interview Commands
git fetch
git rebase main
git cherry-pick <commit-id>
git tag v1.0

## Fixing Common Git Mistakes

### Undo last commit (but keep changes)

git reset --soft HEAD~1

Discard local changes
git checkout -- filename

Check commit history
git log --oneline

Rename last commit message
git commit --amend

