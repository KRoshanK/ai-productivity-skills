---
name: regex-builder
description: Turn a plain-language description of what to validate or extract into a regular expression with a part-by-part explanation. Use when the user wants a regex, wants to understand a regex, or wants extraction/validation patterns.
---

# Regex Builder with Explanation

Build an expression the user can maintain.

## Process
1. Restate the match goal and the non-goals.
2. Ask (or assume explicitly) flavor: JS / PCRE / Python / Go / Rust.
3. Decide: validate full string vs find/extract.
4. Write the regex. Prefer readable over clever.
5. Explain each group.
6. Give match and non-match examples.
7. Note what regex is a bad tool for (emails, HTML, nested markup) and offer an alternative when relevant.

## Output
- Flavor + flags
- Pattern
- Group map
- Examples
- Failure modes

## Rules
- No cargo-cult email regex that rejects valid addresses unless the user wants a practical filter and you label it as such.
- Escape correctly for the host language string if asked.
