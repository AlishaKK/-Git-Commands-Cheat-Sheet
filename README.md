### Git-Commands-Cheat-Sheet

Here's a **clean, clear, and beginner-friendly version** of the Git Commands Cheat Sheet — perfectly structured for your GitHub repository. It avoids jargon, explains what each command does, and is easy to follow even if you're just starting with Git.

---

# 🚀 Git Commands for Beginners

Welcome to your all-in-one **Git cheat sheet**! This guide includes everything you need — from setting up Git to fixing common mistakes — in **simple, clear language**.

---

## 🔧 1. Git Setup

### Set your name and email (needed once):
```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

### Check your current settings:
```bash
git config --list
```

---

## 📁 2. Start a New Git Project

### Create a new Git repository:
```bash
git init
```

### OR clone an existing project:
```bash
git clone https://github.com/username/project-name.git
```

---

## 📌 3. Track and Save Changes

### Check the current status:
```bash
git status
```

### Add all files to be saved:
```bash
git add .
```

### Add a specific file only:
```bash
git add filename.txt
```

### Save your changes (with a message):
```bash
git commit -m "Write a short message about your changes"
```

---

## 🌍 4. Work with GitHub (Remote)

### Connect your GitHub repo (only once):
```bash
git remote add origin https://github.com/username/project-name.git
```

### Upload your code to GitHub:
```bash
git push origin main
```

### Get the latest code from GitHub:
```bash
git pull origin main
```

---

## 🌿 5. Use Branches (for new features)

### Create a new branch:
```bash
git branch new-branch-name
```

### Switch to that branch:
```bash
git checkout new-branch-name
```

### Create and switch at the same time:
```bash
git checkout -b new-branch-name
```

### Merge your branch into `main`:
```bash
git checkout main
git merge new-branch-name
```

---

## 🧹 6. Fix Mistakes (Common Errors)

### Undo your last commit (keep the changes):
```bash
git reset --soft HEAD~1
```

### Undo your last commit (remove the changes):
```bash
git reset --hard HEAD~1
```

### Unstage a file (remove from staging):
```bash
git reset filename.txt
```

### Discard all changes in a file:
```bash
git checkout -- filename.txt
```

### Restore a deleted file:
```bash
git checkout HEAD filename.txt
```

### Temporarily save your work:
```bash
git stash
```

### Get back stashed changes:
```bash
git stash pop
```

---

## 🔍 7. View History & Changes

### See all commits:
```bash
git log
```

### See commits in one line:
```bash
git log --oneline
```

### See who changed what in a file:
```bash
git blame filename.txt
```

### See the difference in files:
```bash
git diff
```

---

## 🛡️ 8. Ignore Sensitive Files (like `.env`)

### Add `.env` to `.gitignore`:
```bash
echo ".env" >> .gitignore
```

### Remove it from Git tracking (if already added):
```bash
git rm --cached .env
git commit -m "Remove .env from version control"
```

### Share a sample config file:
```bash
touch .env.example
# Add placeholders like:
# API_KEY=your_api_key_here
```

---

## ✅ 9. Good Habits for Beginners

- 🧠 Always run `git pull` before `git push`
- 🌿 Use branches for new features or fixes
- 🧾 Write clear commit messages
- 🔒 Never commit `.env` or passwords

---


