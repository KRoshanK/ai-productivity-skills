---
name: code-review-skill
description: Review code for bugs, inefficiencies, and bad practices, returning concrete fix suggestions. Use when the user asks for a review, PR feedback, or a second look at a diff.
---

# Code Review Skill

Review for defects first, style last.

## Severity
- P0: correctness, security, data loss
- P1: likely prod issue, missing tests for a sharp edge
- P2: maintainability, performance that matters
- P3: nits

## Process
1. Identify what the change is trying to do.
2. Hunt: wrong invariants, error handling, races, injection, authz, leaks, off-by-ones.
3. Check tests against the new behavior.
4. Only then mention naming and structure.
5. Suggest a patch shape, not a lecture.

## Rules
- No drive-by rewrites of untouched code.
- If you lack context, list questions instead of blocking on guesses.
