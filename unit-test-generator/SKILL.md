---
name: unit-test-generator
description: Analyze code and generate unit tests for normal cases, edge cases, and error handling, using common testing frameworks. Use when the user wants tests, coverage for a function, or test scaffolds.
---

# Unit Test Generator

Write tests that would fail if the code were wrong.

## Process
1. Identify the unit, its public contract, and collaborators to mock.
2. List behaviors: happy path, boundaries, invalid input, errors, idempotency if relevant.
3. Pick the framework already in the repo if visible (pytest, JUnit, Jest, Vitest, Go testing, etc.). Otherwise ask or default to the language standard.
4. Name tests as behavior sentences.
5. Avoid testing implementation details that would break on a clean refactor.

## Output
- Test file content
- What is not covered and why
- Fixtures / mocks needed

## Rules
- No tests that only assert the mock was called unless interaction is the contract.
- Include at least one test expected to catch a regression.
- Do not invent production functions to make tests pass.
