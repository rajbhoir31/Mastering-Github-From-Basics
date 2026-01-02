# Linux & Git Fundamentals for Java Backend Developers

This repository documents **core Linux and Git skills** required for Java backend development (Spring Boot, Maven, Docker, CI/CD).  
The goal is operational clarity, not theory.

---

## Scope

- Linux commands used daily by backend engineers
- Git mental model used by professional teams
- Safe vs unsafe Git operations
- Branching and remote workflows used in companies

No DevOps depth. No system administration. Only what is required to work effectively.

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















