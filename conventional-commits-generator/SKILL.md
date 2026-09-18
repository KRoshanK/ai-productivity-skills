---
name: conventional-commits-generator
description: Analyze code changes and write Conventional Commits messages so git history is not 'fix things' / 'update stuff'. Use when the user pastes a diff, staged changes, or asks for a commit message.
---

# Conventional Commits Generator

Write commit messages from the actual diff.

## Format
`type(scope): short summary`

Types: feat, fix, docs, style, refactor, perf, test, build, ci, chore, revert.

## Process
1. Read the diff. Group unrelated changes; recommend split commits if needed.
2. Choose type from behavior, not from file type alone.
3. Summary: imperative, 72 chars or fewer, no period, says why-level change not "update file".
4. Body only if the why is not obvious. Footer for BREAKING CHANGE and issue refs.

## Output
- Recommended message(s)
- If the diff should be split, the split plan
- What not to include (secrets, generated noise)

## Rules
- Do not invent ticket numbers.
- Do not write "misc fixes" or "update stuff".
