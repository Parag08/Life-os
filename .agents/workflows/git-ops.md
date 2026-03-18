---
description: Commit and push changes with a custom message
---

# /git-ops [message]

1. Read the Git Operations skill:
   - Open and read `/home/parag/Life-os/.agents/skills/git-ops/SKILL.md`

2. Execute the git sequence:
   - Run `git status`
   - Run `git add -A`
   - Run `git commit -m "[message]"`
   - Run `git push origin $(git branch --show-current)`

3. Report results:
   - Show the commit hash.
   - Confirm the push was successful.
   - List the files that were committed.
