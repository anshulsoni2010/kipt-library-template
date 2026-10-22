---
title: Turn a bug report into a fix plan
description: Agent brief that reproduces a bug first, then fixes it with a test
tags: [code, debugging]
tools: [claude-code, codex]
kind: task
created: 2026-10-22
---
Here is a bug report:

{{bug}}

Before changing any code:
1. Find where this happens. Start in {{area:the part of the code the report mentions}}.
2. Write a failing test that shows the bug.
3. Explain the cause in two or three sentences.

Then fix it with the smallest change that makes the test pass, run the full test suite, and tell me what you changed and why.
