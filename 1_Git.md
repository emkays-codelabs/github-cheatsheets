---
# 🚀 Git Workflow Guide  
### Branch • Commit • HEAD • Staging Areas  

![Git](https://img.shields.io/badge/Git-Workflow-F05032?logo=git&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-2ECC71)
![Level](https://img.shields.io/badge/Level-Beginner-3498DB)
![GitHub](https://img.shields.io/badge/GitHub-emkays--codelabs-black?logo=github)


A clean and simple guide to understand how Git works — from `git init` to commits, branches, HEAD, and staging areas.

---

## 📌 1. Initialize a Repository

```bash
git init
````

### State:

* ❌ No commits
* ❌ No branches
* 📁 Empty repository

```
(Empty repository)
```

👉 Git does **not** create any branch at this stage.

---

## 📝 2. Working Directory (Non-Staging Area)

This is where you **create or edit files**.

### What happens here:

* Files are modified
* Git detects changes
* Changes are **NOT ready** for commit
* Called the **Non-Staging Area**

Example:

```
file.txt (modified)
```

---

## 📦 3. Staging Area

```bash
git add file.txt
```

### What happens here:

* Files move from
  **Working Directory → Staging Area**
* You choose what will be committed
* Git prepares a snapshot

---

## 🟢 4. First Commit (C1)

```bash
git commit -m "Initial commit"
```

### What happens:

* Files move from **Staging Area → Commit (C1)**
* Default branch (`main` / `master`) is created
* A **Commit ID** is generated
* **HEAD** points to the latest commit

```
HEAD → main → C1
```

✅ **In Git, the default branch is created automatically when the first commit is made.**

---

## 🔐 5. Commit ID (SHA-1)

Each commit has:

* 🔢 **40-character alphanumeric ID**
* 🔐 Generated using **SHA-1 hashing**

Example:

```
c1a3f5e9b2d4a8f6c7e1b9a0d2f3e4a5b6c7d8e9
```

Short form:

```
c1a3f5e
```

---

## 🎯 6. HEAD Pointer

* **HEAD** points to the **latest commit**
* HEAD moves when:

  * A new commit is made
  * You switch branches

Example:

```
HEAD → main → C1
```

---

## 🔁 7. Second Commit (C2)

Modify files:

```
file.txt (modified)
```

Stage:

```bash
git add file.txt
```

Commit:

```bash
git commit -m "Second commit"
```

### What happens:

* New commit **C2** is created
* **C2 contains:**

  * New changes (**delta**)
  * A reference to **C1**
* **HEAD moves to C2**

```
HEAD → main → C2 → C1
```

### Meaning of Arrow (→)

> **C2 came from C1**
> **C2 = C1 + Delta**

---

## 🌿 8. Creating a New Branch

```bash
git branch dev
```

### Result:

* New branch `dev` is created
* Both branches point to the same commit

```
main      dev
  |        |
  v        v
  C2  →   C1
```

---

## 🔄 Git Workflow Diagram

```
Working Directory (Non-Staging)
        |
        | git add
        v
Staging Area
        |
        | git commit
        v
Commit (C1, C2, C3...)
        |
        v
Branch → HEAD
```

---

## 🧠 Key Concepts Table

| Concept           | Meaning                   |
| ----------------- | ------------------------- |
| `git init`        | Creates empty repo        |
| Working Directory | Where files are edited    |
| Staging Area      | Files selected for commit |
| Commit            | Snapshot of project       |
| Commit ID         | 40-char SHA-1 hash        |
| Branch            | Pointer to a commit       |
| HEAD              | Points to latest commit   |
| Delta             | New changes               |

---

## ✅ Final Summary

* `git init` → No commits, no branches
* Edit files → Non-Staging Area
* `git add` → Files go to Staging Area
* `git commit` → First commit + default branch created
* Each commit gets **40-char SHA-1 ID**
* **HEAD** always points to latest commit
* New commit **C2** references **C1**
* **C2 = C1 + Delta**
* Arrow (→) shows history
* HEAD always moves forward

---

## ⭐ Useful Commands

```bash
git status
git log --oneline --graph
git branch
git checkout dev
```
---

## 🎉 Congratulations!

You now understand the **complete Git workflow**
from initialization to branching and commit history.

Happy Coding! 🚀
## 👤 Author

**Emkay**  
- GitHub: https://github.com/emkays-codelabs  

---

