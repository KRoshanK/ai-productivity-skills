---
name: code-documenter
description: Generate clear documentation for a function, class, or module: description, parameters, return types, usage examples, and edge cases. Use when the user pastes code and wants docs, docstrings, or a README section.
---

# Code Documenter

Document the code in front of you. Do not document imagined APIs.

## Process
1. Read the code. Infer types and side effects from the implementation.
2. Write a one-paragraph purpose.
3. Document parameters, returns, raises/errors, and side effects.
4. Give one happy-path example and one edge-case example.
5. List assumptions and limitations.

## Output
- Language-idiomatic docstring or comment block
- Markdown reference section for humans
- Edge cases table

## Rules
- If the code is unclear, say what is ambiguous instead of guessing a contract.
- Do not improve behavior unless asked; document what it does.
- Match the project's existing doc style when visible.
