---
title: AGENTS.md starter
description: Rules file that Claude Code and Codex read at the start of every session
tags: [agents, setup]
tools: [claude-code, codex]
kind: rules
created: 2026-10-22
---
# {{project}}

{{one_line_summary:What this project does, in one sentence.}}

## Stack
{{stack:TypeScript, Next.js, Tailwind CSS}}

## Commands
- Install: {{install:npm install}}
- Test: {{test:npm test}}
- Lint and typecheck before saying a task is done.

## Rules
- Read the relevant code before changing it.
- Keep changes small and focused on the task.
- Never commit secrets. They live in .env.local only.
- Ask before adding a new dependency.
