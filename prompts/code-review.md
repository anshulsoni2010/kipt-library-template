---
title: Review this diff like a senior engineer
description: A focused code review that ranks problems by how much they matter
tags: [code, review]
tools: [claude-code, codex]
kind: task
created: 2026-10-22
---
Review the diff below as a senior {{language:TypeScript}} engineer.

Focus on {{focus:correctness, edge cases and security}}. For each problem:
1. Quote the line.
2. Say what goes wrong and when.
3. Suggest the smallest fix.

Rank problems from most to least serious. Skip style nits unless they hide a bug.
End with one sentence: is this safe to merge as is?

{{diff}}
