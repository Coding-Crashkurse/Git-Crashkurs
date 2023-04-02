# Git-Crashkurs

In diesem Crashkurs lernst du die Grundlagen von Git und GitHub kennen. Du erfährst, wie du deine Projekte verwalten, Änderungen verfolgen, mit remote Repositories interagieren und Branches verwenden kannst, um verschiedene Versionen deines Codes zu entwickeln.

## Git Basics

    git config --global user.name "Dein Name"

Setzt den globalen Benutzernamen, der für alle deine Git-Projekte verwendet wird.

    git config --global user.email "deine.email@example.com"

Setzt die globale E-Mail-Adresse, die für alle deine Git-Projekte verwendet wird.

### Repo Initialisieren

    git init

Initialisiert ein neues Git-Repository im aktuellen Verzeichnis.

### Dateien hinzufügen und commiten

    git add <file>

Fügt eine oder mehrere Dateien zum Staging-Bereich hinzu, um sie für den nächsten Commit vorzubereiten.

    git commit -m "Commit-Nachricht"

Erstellt einen neuen Commit mit den Änderungen im Staging-Bereich und der angegebenen Commit-Nachricht.

### Commit-Verlauf anzeigen

    git log

Zeigt die Commit-Historie des aktuellen Branches an.

    git log --oneline

Zeigt die Commit-Historie in einer kompakten, einzeiligen Ansicht.

### Commits anzeigen und rückgängig machen

    git show <commit-id>

Zeigt die Änderungen und Informationen zu einem bestimmten Commit anhand der Commit-ID.

    git revert <commit-id>

Erstellt einen neuen Commit, der die Änderungen des angegebenen Commits rückgängig macht.

    git reset <commit-id>

Setzt den aktuellen Branch auf den angegebenen Commit zurück.

### Stashing

    git stash save "Stash-Nachricht"

Speichert alle aktuellen Änderungen in einem neuen Stash und setzt das Arbeitsverzeichnis auf den letzten Commit zurück.

    git stash pop <stash-id>

Wendet die Änderungen eines Stash an und entfernt ihn aus der Stash-Liste.

    git stash drop <stash-id>

Entfernt einen Stash ohne die Änderungen anzuwenden.

## Github

### Repository verbinden

    git remote add origin <repository-url>

Verknüpft das lokale Repository mit dem entfernten Repository unter der angegebenen URL.

### Änderungen von Github holen

    git fetch

Lädt alle Änderungen vom entfernten Repository herunter, ohne den lokalen Code zu ändern.

    git pull

Lädt Änderungen vom entfernten Repository herunter und integriert sie in den aktuellen Branch.

## Branching

### Branch erstellen und wechseln

    git checkout -b <branch-name>

Erstellt einen neuen Branch und wechselt direkt zu diesem.

### Zu einem existierenden Branch wechseln

    git checkout <branch-name>

Wechselt zu einem anderen Branch.

### Branch löschen

    git branch -d <branch-name>

Löscht den angegebenen Branch.

### Branches zusammenführen

    git merge <branch-name>

Führt Änderungen eines anderen Branches in den aktuellen Branch ein.

    git rebase <branch-name>

Integriert Änderungen eines anderen Branches, indem Commits neu angewendet werden, anstatt einen Merge-Commit zu erstellen.

### Commits squashen

    git rebase -i HEAD~3

Startet einen interaktiven Rebase, um die letzten 3 Commits zusammenzuführen (anzupassen).
