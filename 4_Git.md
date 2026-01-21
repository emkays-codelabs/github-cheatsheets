---

# 📘 Git Commands 4 – Complete Workflow Guide

*A clean, step-by-step explanation of common Git commands*

---

## 1️⃣ Removing Sensitive Files from Git Tracking

Sometimes secret files (like `.env` or token files) were already committed.
Even if they are added to `.gitignore`, Git will still track them.

### Commands:

```bash
git rm --cached .env
git rm --cached api_token.txt
```

### What this does:

* Removes files from **Git tracking**
* Keeps them on your **local system**
* Prevents them from being pushed to GitHub

After removing, commit the change:

```bash
git commit -m "Remove sensitive files"
```

---

## 2️⃣ View Staged (Cached) Changes

```bash
git diff --cached
```

### Purpose:

Shows all files currently in the **staging area**
These are the files that will be included in the next commit.

Use this to:

* Review changes
* Ensure no secrets are included

---

## 3️⃣ Pull Remote Changes with Rebase

```bash
git pull origin main --rebase
```

### Why use `--rebase`?

* Updates your branch with remote changes
* Keeps commit history clean
* Avoids unnecessary merge commits

Use when:

* Push is rejected
* Remote has new commits

---

## 4️⃣ Push Changes to GitHub

```bash
git push
```

Pushes your committed changes to the remote repository.

---

## 5️⃣ Merge & Abort Merge

### Merge branches:

```bash
git merge
```

### Abort a merge (if conflicts occur):

```bash
git merge --abort
```

Use this if:

* You want to cancel an incomplete merge
* Conflicts are too complex to resolve

---

## 6️⃣ Create `.gitignore` Using Command Line

These commands create and update the `.gitignore` file.

```bash
echo .env > .gitignore
echo *.txt >> .gitignore
echo __pycache__/ >> .gitignore
echo *.log >> .gitignore
echo node_modules/ >> .gitignore
```

### Explanation:

| Symbol | Meaning                 |
| ------ | ----------------------- |
| `>`    | Create / overwrite file |
| `>>`   | Append to file          |

### Ignored files:

* `.env` → Environment secrets
* `*.txt` → Text files
* `__pycache__/` → Python cache
* `*.log` → Log files
* `node_modules/` → JavaScript dependencies

---

## 7️⃣ Add & Remove Remote Repository

### Add a remote:

```bash
git remote add origin https://github.com/username/repository.git
```

### View remotes:

```bash
git remote -v
```

### Remove a remote:

```bash
git remote remove origin
```

---

## 8️⃣ Difference Between Push Commands

### 1. Basic push

```bash
git push
```

Pushes to the default upstream branch.

### 2. Explicit push

```bash
git push origin main
```

Pushes `main` branch to `origin`.

### 3. Set upstream & push

```bash
git push -u origin main
```

Sets `origin/main` as default for future pushes.

---

## 9️⃣ Rename Branch to `main`

```bash
git branch -M main
```

### Purpose:

* Renames the current branch to `main`
* Used to match GitHub’s default branch name

---

## 🔟 Delete a File Locally

```bash
del api_token.txt
```

Deletes the file from your system.

---

## 1️⃣1️⃣ Reset Last Commit (Dangerous)

```bash
git reset --hard HEAD~1
```

### What it does:

* Removes the last commit
* Deletes all its changes
* Cannot be undone easily

Use only if:

* You made a serious mistake
* You haven’t pushed yet

---

## 1️⃣2️⃣ Remove Git Completely

```bash
rmdir /s /q .git
```

### Purpose:

* Deletes all Git history
* Project becomes a normal folder

Use when:

* You want to restart Git from scratch

---

## 1️⃣3️⃣ Pull with Unrelated Histories

```bash
git pull origin main --allow-unrelated-histories
```

### Use this when:

* Local and remote repos were created separately
* Git refuses to merge them

---

## 1️⃣4️⃣ Force Push (Use Carefully)

```bash
git push -u origin main --force
```

### What it does:

* Overwrites remote history
* Deletes remote commits

Use only if:

* You cleaned secrets
* You understand the risks

---

## 🔄 Standard Git Workflow

```bash
git status
git add .
git commit -m "Your message"
git push
```

---

## ⚠️ Safety Rules

| Do                        | Don’t              |
| ------------------------- | ------------------ |
| Use `.gitignore`          | Upload API keys    |
| Check `git diff --cached` | Commit secrets     |
| Use `--rebase`            | Force push blindly |
| Rotate leaked tokens      | Ignore warnings    |

---

## 🧠 Summary

This guide covers:

✔ Secret removal
✔ `.gitignore` creation
✔ Push & pull
✔ Merge handling
✔ Reset & cleanup
✔ Remote management
✔ Force push risks

---


## 👨‍💻 Author

<p align="center">
  <img src="https://avatars.githubusercontent.com/emkays-codelabs" width="140px" style="border-radius: 50%;" />
</p>

<h3 align="center">Emkay</h3>

<p align="center">
  <a href="https://github.com/emkays-codelabs">
    github.com/emkays-codelabs
  </a>
</p>
<p align="center">
  <img src="https://img.shields.io/github/followers/emkays-codelabs?label=Followers&style=flat&logo=github" />
  <img src="https://img.shields.io/github/stars/emkays-codelabs?label=Stars&style=flat&logo=github" />
</p>



<p align="center">
  😎 Follow me for clean code and cool projects<br/>
  ⭐ Star my repos to boost my coding superpowers 💪
</p>


<p align="center">
  <img src="https://img.shields.io/badge/Learn-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Code-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Build-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Improve-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Level up%20Together-purple?style=for-the-badge" />
</p>


<p align="center">
  <em>Stay curious. Keep coding.🔥
</em> 
</p>
