# My Kipt library

Your prompts and skills, as plain files in a private repo you own. [Kipt](https://hotbar-orpin.vercel.app) reads and writes this repo; you can also edit it by hand.

```
prompts/        one Markdown file per prompt
skills/         one folder per skill, each with a SKILL.md
images/         images attached to prompts (added by Kipt)
index.json      search index, rebuilt by Kipt on every save
```

## Prompts

Each file in `prompts/` has a short header, then the prompt text. Parts that change are written as `{{name}}` or `{{name:default}}`; Kipt asks you to fill them in when you copy.

```markdown
---
title: Review this diff like a senior engineer
tags: [code, review]
kind: task
---
Review the diff below as a senior {{language:TypeScript}} engineer.
```

## Skills

Each folder in `skills/` follows the Agent Skills standard that Claude Code and Codex read. Install them all with:

```
npx skills add https://github.com/<you>/<this-repo>.git --all -g
```
