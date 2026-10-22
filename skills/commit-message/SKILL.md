---
name: commit-message
description: Writes a clear git commit message for the staged changes. Use when the user asks to commit, wants a commit message, or says "write the commit".
---

# Commit message

## Steps

1. Read the staged changes with `git diff --staged`. If nothing is staged, say so and stop.
2. Work out the one main reason for the change. If the diff does two unrelated things, suggest splitting it into two commits.
3. Write the message:
   - **Subject**: imperative mood, under 60 characters, no period. "Add retry to image uploads", not "Added retries".
   - **Blank line.**
   - **Body** (only if the why isn't obvious): what was wrong or missing, and why this fixes it. Wrap at 72 characters.
4. Show the message and ask before committing.

## Avoid

- Vague subjects like "Update files" or "Fix stuff".
- Listing every file that changed. The diff already does that.
