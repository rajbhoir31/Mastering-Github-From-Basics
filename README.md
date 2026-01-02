# Linux & Git Fundamentals

This repository documents **core Linux and Git skills**
The goal is operational clarity, not theory.

---

## PART 1 — Linux Fundamentals

### 1. Navigation & Awareness

```bash
pwd        # show current directory
ls         # list files
ls -la     # permissions + hidden files
cd dir     # move into directory
cd ..      # move up
cd ~       # home directory
```

### 2. File & Directory Control

``` bash
mkdir app
touch application.yml
cp a b
mv old new
rm file
rm -r dir
```

### 3. Viewing Logs & Files
``` bash
cat file
less file
tail -f app.log
grep "ERROR" app.log
```

### 4. Disk & Permissions
```bash
df -h
chmod +x script.sh
sudo command
```

## PART 2 — Git Mental Model

Git operates in three zones:
```bash
Working Directory → Staging Area → Repository
```

## PART 3 — Git Essentials

### 1. One-Time Setup

```bash
git --version
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

### 2. Create / Check Repository

```bash
git init
git status
```

### 3. Ignore Files (Before First Commit)

```bash
touch .gitignore
```
Recommended ignores for Java projects:
```
/target
/.idea
*.log
.env
```

### 4. Stage Changes
```
git add file
git add .
git add -u
```

### 5. Commit
```
git commit -m "Add user service"
```

### 6. History & Inspection
```
git log --oneline
git diff
git diff --staged
```

## PART 4 — Undoing Changes Safely

### Safe Undo (Team-Safe)
```
git restore file
git restore --staged file
git revert commit_hash
```

### Dangerous (Local Only)
```
git reset --soft
git reset --mixed
git reset --hard
```

## PART 5 — Branching Workflow
```
git branch
git checkout -b feature-auth
git switch main
git merge feature-auth
```

## PART 6 — Remote Repositories (GitHub)
```
git clone repo_url
git remote add origin URL
git push -u origin main
git pull
git fetch
```


