---
name: release-notes
description: Writes user-facing release notes from merged commits, pull requests or a changelog. Use when preparing a release, bumping a version, or writing a "what's new" post.
---

# Release notes

Write release notes people outside the team can read in under a minute.

## Steps

1. Find what changed since the last release. Prefer the git tags: `git log <last-tag>..HEAD --oneline`. If there are no tags, ask which commit or date to start from.
2. Group the changes:
   - **New**: things people can now do.
   - **Better**: improvements to things that already existed.
   - **Fixed**: bugs people could have hit.
   Leave out refactors, dependency bumps and internal tooling unless they change behavior.
3. Write one line per change, starting with a verb, in plain words. Say what the person gets, not how it was built.
4. Put the most useful change first in each group.
5. If anything breaks existing behavior, add a **Before you upgrade** section at the top with exactly what to do.

## Style

- No commit hashes or ticket numbers in the text.
- No exclamation marks.
- Keep the whole thing under 200 words unless the release is large.
