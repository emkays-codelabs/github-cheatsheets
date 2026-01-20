# Git Concepts Explained Clearly

## 1. What is Git?

Git is a version control system used to track changes in files.

---

## 2. Repository

A folder that contains a `.git` directory.

---

## 3. Commit ID (SHA-1)

Each commit has a unique **40-character** alphanumeric hash.
Example (short):

```
a8603ad
```

---

## 4. HEAD Pointer

HEAD always points to the **latest commit** of the current branch.

When a new commit happens → HEAD moves forward.

---

## 5. Branch

The default branch (master/main) is created automatically after the first commit.

---

## 6. Working Directory

Where you edit your files normally.

---

## 7. Staging Area

Holds files that are prepared for commit.
Added using:

```bash
git add file.txt
```

---

## 8. Commit Object

A commit object contains:

* Author
* Date
* Message
* Reference to previous commit

Stored in:

```
.git/objects/
```

---

## 9. Commit Chain

```
C1  --->  C2
```

C2 references C1. This forms Git history.

---

## 10. Delta Storage

Git stores only **changes**, not full copies of files.

---

## 11. Git Reset

Used to:

* Unstage files
* Undo commits
* Move HEAD

---

## 12. Git Status Symbols

| Symbol | Meaning              |
| ------ | -------------------- |
| ??     | Untracked            |
| A      | Added                |
| M      | Modified             |
| Clean  | Everything committed |

---

## 13. Example Commit Log

```
a8603ad (HEAD -> master) first file
```

Meaning:

* a8603ad → Commit ID
* HEAD → Current position
* master → Branch
* first file → Commit message

---

## 14. Object Storage

Git stores:

* Blobs
* Trees
* Commits
* Refs

All inside:

```
.git/
```
