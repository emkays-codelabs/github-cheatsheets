---
# 🚀 Git & GitHub Basics – Beginner Friendly Guide

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
8. 🌿 Branch Basics  
9. 📜 View Commit History  
10. ☁️ Host Project on GitHub  
11. ⚠️ Important Rules & Tips  
12. 🔄 Git Workflow Summary  

---

## 1️⃣ 🔧 Git Setup (One-Time)

Set your Git identity (used in commits):

```cmd
git config --global user.name "emkays-codelabs"
git config --global user.email "your_new_email@example.com"
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

📌 **Important:**

> Git tracks **files**, not empty folders.
> To track an empty folder, add a placeholder file:

```cmd
type nul > folder_name/.gitkeep
```

---

## 3️⃣ 🧱 Initialize Git Repository

⚠️ Always initialize Git in the **main project folder**, not a subfolder.

```cmd
git init
```

✔️ Creates a hidden `.git` folder
✔️ Starts Git tracking

---

## 4️⃣ 👀 View Files & Git Status

View all files (including hidden):

```cmd
dir /a
```

Clean view:

```cmd
dir /a /b
```

Check Git status:

```cmd
git status
```

Short format:

```cmd
git status -s
```

Verbose (shows diff):

```cmd
git status -v
```

---

## 5️⃣ ➕ Stage Files (Add to Tracking)

Add a single file:

```cmd
git add filename
```

Add all files (**use carefully**):

```cmd
git add .
```

📦 **Staging Area** = Files ready to be committed

---

## 6️⃣ ❌ Unstage & Delete Files

### 🔄 Undo `git add` (Unstage files)

```cmd
git rm --cached f1.txt f2.txt
```

Unstage everything:

```cmd
git restore --staged .
```

---

### 🗑️ Delete a file (from Git + system)

```cmd
git rm filename
```

---

## 7️⃣ 💾 Commit Changes

Save staged changes permanently:

```cmd
git commit -m "Your commit message"
```

✔️ Creates a snapshot of your project

---

## 8️⃣ 🌿 Branch Basics

Check current branch:

```cmd
git branch
```

Rename default branch to `main`:

```cmd
git branch -m main
```

📌 `main` is the modern standard branch name.

---

## 9️⃣ 📜 View Commit History

View all commits:

```cmd
git log
```

Compact view:

```cmd
git log --oneline
```

View last commit details:

```cmd
git show
```

List all committed files:

```cmd
git ls-tree --name-only -r HEAD
```

---

## 🔟 ☁️ Host Project on GitHub

### 🧩 Step 1: Create a Repository on GitHub

* Go to 👉 [https://github.com](https://github.com)
* Click **New Repository**
* Copy the HTTPS URL

---

### 🔗 Step 2: Connect Local Project to GitHub

```cmd
git remote add origin https://github.com/emkays-codelabs/REPO_NAME.git
```

Verify:

```cmd
git remote -v
```

---

### 🚀 Step 3: Push Code to GitHub

```cmd
git push -u origin main
```

🎉 Your project is now **hosted on GitHub**!

---

## 1️⃣1️⃣ ⚠️ Important Rules & Tips

* ❌ Do not create `.git` inside subfolders
* ✅ Only one Git repository per main project
* 📂 Git does not track empty folders
* 🔍 Always run `git status` before commit
* 🧹 Use `.gitignore` to ignore unnecessary files

---

## 1️⃣2️⃣ 🔄 Git Workflow Summary

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

## 👤 Author

**emkays-codelabs**
Happy Coding 🚀

````





