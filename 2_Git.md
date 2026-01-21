---

# 📘 Git Commands 2 – Complete Workflow Guide

![Git](https://img.shields.io/badge/Git-Version%20Control-orange)
![GitHub](https://img.shields.io/badge/GitHub-Hosting-black)
![Level](https://img.shields.io/badge/Level-Beginner-green)
![Status](https://img.shields.io/badge/Status-Learning-blue)
![Format](https://img.shields.io/badge/Format-Markdown-lightgrey)

A simple, step-by-step guide to understand **Git workflow**, from creating files to **hosting your project on GitHub**.

---

## 🧭 Table of Contents

1. 🔧 Git Setup  
2. 📁 Create Files & Folders  
3. 🧱 Initialize Git Repository  
4. 👀 View Files & Git Status  
5. ➕ Stage Files  
6. ❌ Unstage & Delete Files  
7. 💾 Commit Changes  
8. 🌿 Branch Basics (master vs main, rename, create)  
9. 📜 View Commit History  
10. ☁️ Host Project on GitHub  
11. ⚠️ Important Rules & Tips  
12. 📊 Git Status Symbols  
13. 🧾 Commit Log Meaning  
14. 🗂️ Where Git Stores Commits  
15. 🔄 Git Workflow Summary  

---

## 1️⃣ 🔧 Git Setup (One-Time)

Set your Git identity:

```cmd
git config --global user.name "your-username"
git config --global user.email "your-email@example.com"
git config --global user.name "Your New Name"

````

Verify:

```cmd
git config --global --list
```

---

## 2️⃣ 📁 Create Files & Folders

Create an empty file:

```cmd
type nul > example.txt
```

📌 Git does **not** track empty folders.
Use a placeholder:

```cmd
type nul > folder_name/.gitkeep
```

---

## 3️⃣ 🧱 Initialize Git Repository

```cmd
git init
```

✔ Creates `.git`
✔ Starts version tracking

---

## 4️⃣ 👀 View Files & Git Status

```cmd
dir /a
git status
git status -s
git status -v
```

---

## 5️⃣ ➕ Stage Files

```cmd
git add filename
git add .
```

Staging Area = files ready to be committed.

---

## 6️⃣ ❌ Unstage & Delete Files

Unstage files:

```cmd
git rm --cached f1.txt
git restore --staged .
```

Delete file:

```cmd
git rm filename
```

---

## 7️⃣ 💾 Commit Changes

```cmd
git commit -m "Your commit message"
```

Creates a **commit snapshot**.

---

## 8️⃣ 🌿 Branch Basics (master vs main, rename, create)

### 🔹 What is a Branch?

A branch is a **separate line of development**.
Each branch has its own commit history.

---

### 🔹 master vs main

| Branch   | Meaning                     |
| -------- | --------------------------- |
| `master` | Old default branch name     |
| `main`   | New standard default branch |

GitHub now uses **`main`** instead of `master`.

---

### 🔹 Check Current Branch

```cmd
git branch
```

---

### 🔹 Rename master to main

```cmd
git branch -m main
```

---

### 🔹 Create a New Branch

```cmd
git branch feature1
```

---

### 🔹 Switch to a Branch

```cmd
git checkout feature1
```

Or modern command:

```cmd
git switch feature1
```

---

### 🔹 Create & Switch in One Command

```cmd
git checkout -b feature2
```

---

### 🔹 Why Use Branches?

* Work on new features safely
* Fix bugs without affecting main code
* Collaborate with teams

---

## 9️⃣ 📜 View Commit History

```cmd
git log
git log --oneline
git show
git ls-tree --name-only -r HEAD
```

---

## 🔟 ☁️ Host Project on GitHub

Add remote:

```cmd
git remote add origin https://github.com/USERNAME/REPO_NAME.git
git remote -v
```

Push:

```cmd
git push -u origin main
```

---

## 1️⃣1️⃣ ⚠️ Important Rules & Tips

* ❌ Don’t create `.git` inside subfolders
* ✅ One repo per project
* 📂 Empty folders not tracked
* 🔍 Always run `git status`
* 🧹 Use `.gitignore`

---

## 1️⃣2️⃣ 📊 Git Status Symbols

| Symbol | Meaning                   |
| ------ | ------------------------- |
| `??`   | Untracked (not committed) |
| `A`    | Added to staging          |
| `M`    | Modified                  |
| Clean  | Everything committed      |

Check using:

```cmd
git status -s
```

---

## 1️⃣3️⃣ 🧾 Commit Log Meaning

Example:

```
a8603ad (HEAD -> master) first file
```

| Part       | Meaning                |
| ---------- | ---------------------- |
| a8603ad    | Commit ID (short hash) |
| HEAD       | Your current position  |
| master     | Current branch         |
| first file | Commit message         |

View logs:

```cmd
git log --oneline
```

---

## 1️⃣4️⃣ 🗂️ Where Git Stores Commits

All Git data is stored in:

```
.git/
```

Commit objects are inside:

```
.git/objects/
```

Git stores 4 main object types:

* **Blobs** → File content
* **Trees** → Folder structure
* **Commits** → History
* **Refs** → Branch pointers

Each commit points to the **previous commit**, not a full copy.

---

## 1️⃣5️⃣ 🔄 Git Workflow Summary

```
Create / Edit File ✏️
        ↓
git add ➕
        ↓
git commit 💾
        ↓
git push ☁️
```

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

````





