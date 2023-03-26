# Git-Crashkurs"

## Git Basics

git config --global user.name "Dein Name"
git config --global user.email "deine.email@example.com"

#### Repo Initialisieren

git init
git add <file>
git commit -m "Commit-Nachricht"

git log
git log --oneline

git show <commit-id>

git revert <commit-id>
git reset <commit-id>

## Github

git remote add origin <repository-url>
git fetch
git pull

### Branching

git checkout -b <branch-name>
git checkout <branch-name>

git merge <branch-name>
git branch -d <branch-name>

git checkout -- <datei>

## Git advanced concepts

git stash save "Stash-Nachricht"
git stash
