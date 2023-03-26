# Git-Crashkurs

## Git Basics

    git config --global user.name "Dein Name"
    git config --global user.email "deine.email@example.com"

### Repo Initialisieren

    git init

### Dateien hinzufügen und commiten

    git add <file>
    git commit -m "Commit-Nachricht"

### Commit-Verlauf anzeigen

    git log
    git log --oneline

### Commits anzeigen und rückgängig machen

    git show <commit-id>
    git revert <commit-id>
    git reset <commit-id>

### Stashing

    git stash save "Stash-Nachricht"
    git stash pop <stash-id>
    git stash drop <stash-id>

## Github

### Repository verbinden

    git remote add origin <repository-url>

### Änderungen von Github holen

    git fetch
    git pull

## Branching

### Branch erstellen und wechseln

    git checkout -b <branch-name>

### Zu einem existierenden Branch wechseln

    git checkout <branch-name>

### Branch löschen

    git branch -d <branch-name>

### Branches zusammenführen

    git merge <branch-name>
    git rebase <branch-name>

### Commits squashen aas

    git rebase -i HEAD~3
