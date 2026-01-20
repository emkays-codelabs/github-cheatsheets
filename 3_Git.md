---

# 🚀 Git Workflow & Log Commands – Beginner Friendly Guide

![Git](https://img.shields.io/badge/Git-Version%20Control-orange)
![GitHub](https://img.shields.io/badge/GitHub-Hosting-black)
![Level](https://img.shields.io/badge/Level-Beginner-green)
![Status](https://img.shields.io/badge/Status-Learning-blue)
![Format](https://img.shields.io/badge/Format-Markdown-lightgrey)

A clear guide to understand **Git history, commit inspection, branches, reset behavior, and internal storage**.

---

## 🧭 Table of Contents

1. 🔄 Reset Changes  
2. 📜 View Commit History  
3. 📁 View Committed Files  
4. 🌿 Branch Information  
5. 🌐 Remote Branches  
6. 🌳 Visual Commit Graph  
7. 🗂️ Where Git Stores Commits  
8. 🔄 Git Workflow Summary  

---

## 1️⃣ 🔄 Reset Changes

```bash
git reset
````

### What it does:

* Removes files from the **staging area**
* Keeps your file changes
* Does NOT delete commits

Use this when you accidentally run `git add`.

---

## 2️⃣ 📜 View Commit History

### Compact history:

```bash
git log --oneline
```

Example output:

```
a8603ad (HEAD -> main) first file
```

### Full history:

```bash
git log
```

Shows:

* Commit ID
* Author
* Date
* Commit message

---

## 3️⃣ 📁 View Committed Files

### Files in the latest commit:

```bash
git show --name-only
```

### List all committed files:

```bash
git ls-tree -r HEAD --name-only
```

This shows **only committed files**, not untracked ones.

---

## 4️⃣ 🌿 Branch Information

### List local branches:

```bash
git branch
```

### List remote branches:

```bash
git branch -r
```

### List all branches:

```bash
git branch -a
```

---

## 5️⃣ 🌐 Remote Branches Explained

Remote branches look like:

```
origin/main  
origin/dev  
```

They represent branches that exist on **GitHub**, not locally.

---

## 6️⃣ 🌳 Visual Commit Graph

```bash
git log --graph --oneline --all
```

Shows:

* Branch structure
* Merge history
* Commit flow

Example:

```
* a1b2c3 (main)
|\
| * d4e5f6 (feature)
|/
* 123abc
```

---

## 7️⃣ 🗂️ Where Git Stores Commits

All Git data is stored inside:

```
.git/
```

Commit objects are stored in:

```
.git/objects/
```

Each commit object contains:

* Author
* Date
* Commit message
* Reference to the previous commit

Git does **not** store full copies of files.
It stores only the **changes (delta)** between commits.

---

## 8️⃣ 🔄 Git Workflow Summary

```
Edit File ✏️
     ↓
git add ➕
     ↓
git commit 💾
     ↓
git push ☁️
```

For inspection:

```
git log
git show --name-only
git ls-tree
git branch -a
git log --graph
```

---

## 📌 Command Summary

| Command                           | Purpose              |
| --------------------------------- | -------------------- |
| `git reset`                       | Unstage files        |
| `git log --oneline`               | Compact history      |
| `git log`                         | Full history         |
| `git show --name-only`            | Files in last commit |
| `git ls-tree -r HEAD --name-only` | All committed files  |
| `git branch -r`                   | Remote branches      |
| `git branch -a`                   | All branches         |
| `git log --graph`                 | Visual commit tree   |

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
  <img src="https://img.shields.io/github/followers/emkays-codelabs?style=for-the-badge&logo=github&color=blue" />
  <img src="https://img.shields.io/github/stars/emkays-codelabs?style=for-the-badge&logo=github&color=yellow" />
</p>

<p align="center" style="font-size:18px; font-weight:bold;">
  <span style="color:#ff5733;">Learn.</span>
  <span style="color:#33c1ff;">Code.</span>
  <span style="color:#28a745;">Build.</span>
  <span style="color:#ffc107;">Improve.</span>
  <span style="color:#6f42c1;">Grow together!</span> 😊
</p>


<p align="center">
  <em>Happy Coding!</em> 🚀
</p>

---





## 📤 Push the Updated File

```bash
git add README.md
git commit -m "Reorganize workflow: focus on logs, branches, reset, and Git internals"
git push
````

---


