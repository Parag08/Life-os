---
name: git-ops
description: A skill to handle staging, committing with custom messages, and pushing code to the remote repository.
---

# 🚀 Git Operations Skill

## Overview
This skill provides a standardized way to manage version control for the Life OS. It ensures all changes are properly staged, committed with meaningful messages, and synchronized with the remote GitHub repository.

---

## 🛠️ Instructions

### 1. Stage Changes
Always verify which files are being changed before staging.
- Use `git status` to see unstaged changes.
- Use `git add .` to stage all changes, or `git add <file>` for specific files.

### 2. Commit with Message
Commits should have a clear, concise message describing the "Why" and "What".
- Use `git commit -m "<type>: <description>"`
- Standard types: `feat`, `fix`, `docs`, `refactor`, `chore`.

### 3. Authorize and Push to Remote
- Push using `git push origin $(git branch --show-current)`.
- If the push fails with a permission error, add the SSH identity and retry:
  - Run `eval $(ssh-agent)`
  - Run `ssh-add ~/.ssh/id_ed25519_parag08`

---

## 🏃 Workflow Pattern

When the user says "Commit and push with message: [message]", follow these steps:

1. **Check Status:** Run `git status` to confirm pending changes.
2. **Stage:** Run `git add -A` (unless specified otherwise).
3. **Commit:** Run `git commit -m "[message]"`
4. **Push:** Run `git push origin $(git branch --show-current)`.
5. **Authorize & retry (only if push fails):** If the push fails due to permission issues, run `eval $(ssh-agent) && ssh-add ~/.ssh/id_ed25519_parag08` and retry the push.
6. **Report:** Show the commit hash, confirm the push status, and list the files that were committed.

---

## ⚠️ Safety Checks
- Never push if there are merge conflicts.
- Ensure the user's name and email are configured (already done in previous steps).
- Confirm the remote URL is correct if a push fails.
