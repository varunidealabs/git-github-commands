 to **initialize git** locally and **push your code** to this GitHub repo:  

Here are the exact steps you need to run in your terminal:

```bash
# Step 1: Initialize git
git init

# Step 2: Add all files
git add .

# Step 3: Commit the changes
git commit -m "Initial commit"

# Step 4: Add the remote repository
git remote add origin https://github.com/curious-pm/mcp-todoist.git

# Step 5: Push the code to the main branch
git branch -M main
git push -u origin main
```

---
Perfect — if you want to **create a new branch** called `sse` and **start working on it**, here’s the simple flow:

---

### 📜 Commands:

```bash
# Step 1: Create a new branch named "sse"
git checkout -b sse

# Step 2: (Optional) Check that you are now on branch "sse"
git branch

# Step 3: Push this new branch to GitHub
git push -u origin sse
```

---
###Creating  a new branch "sse"
---

- `git checkout -b sse` → Create + switch to `sse`.
- `git push -u origin sse` → Upload the `sse` branch to GitHub.
- `git checkout sse` →switching between branches

---

No worries! 🤝 You're asking really good questions — let’s go slow and clear:

---

# 🔥 1. How to switch between branches?

You can **move (checkout)** from one branch to another using:

```bash
git checkout branch-name
```

For example:

- To switch to `main`:
  ```bash
  git checkout main
  ```

- To switch to `sse`:
  ```bash
  git checkout sse
  ```

---

#  What happens when you push code to `sse` branch?

- Your changes will **only** go to the `sse` branch.
- `main` branch will **stay clean and untouched** unless you merge.
- Think of it like **two parallel copies**:
  - `main` has the "stable" or "official" version.
  - `sse` is your **experimental** or **new work** branch.

> **Important**: They are *independent* until you merge them manually.

#  Later, how to bring `sse` code into `main`?

When you finish working on `sse`, you can **merge** it into `main` like this:

```bash
# Step 1: Switch to main branch
git checkout main

# Step 2: Pull latest changes from remote to be safe
git pull origin main

# Step 3: Merge 'sse' into 'main'
git merge sse

# Step 4: Push merged changes to GitHub
git push origin main
```
