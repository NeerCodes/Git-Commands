# Git Commands Cheat Sheet

## 🔧 Git Configuration

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global core.editor "code --wait"
```

## 📁 Working with Branches

```bash
# Create a new branch
git branch new-branch

# Switch to a branch
git checkout new-branch

# Create and switch to a branch
git checkout -b new-branch

# List all branches
git branch

# Delete a branch
git branch -d branch-name
```

## 🔄 Merging & Rebasing

```bash
# Merge a branch into current one
git merge feature-branch

# Rebase current branch onto another
git rebase main

# Abort rebase if conflicts

# During conflict resolution, in VS Code:
# 'Current changes' → your branch
# 'Incoming changes' → the branch you’re rebasing onto

# After resolving conflict:
git add <resolved-files>
git rebase --continue
```

## 💾 Staging & Committing

```bash
# Stage files
git add .

# Commit changes
git commit -m "Your commit message"

# Amend last commit
git commit --amend
```

## ⏱️ Stashing

```bash
# Stash current changes
git stash

# Create new branch and apply stash
git checkout -b new-branch

# Apply last stashed changes
git stash pop
```

## 🚀 Pushing & Pulling

```bash
# Push to a branch
git push origin branch-name

# Pull latest changes
git pull origin branch-name

# Push with force (use cautiously)
git push --force
```

## 🗂️ Removing/Restoring Files

```bash
# Remove a file from repo but keep locally
git rm --cached path/to/file

# Restore deleted file
git checkout HEAD path/to/file
```

## 🧹 Clean & Reset

```bash
# Remove all untracked files
git clean -fd

# Reset all changes
git reset --hard HEAD
```

## ✅ Pull Request Fixes

```bash
# Remove a file already pushed (e.g. .env.dev)
git rm --cached .env.dev
git commit -m "Remove .env.dev"
git push
```

## 🔍 Checking Logs & Status

```bash
# View commit logs
git log

# View status of working directory
git status
```

---

Feel free to copy and adjust according to your use case!
