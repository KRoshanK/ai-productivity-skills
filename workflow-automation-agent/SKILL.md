---
name: workflow-automation-agent
description: Break a complex goal into a step-by-step workflow, assign tools to each step, and optimize execution. Use when the user wants an SOP, agent workflow, automation plan, or multi-step execution design.
---

# Workflow Automation Agent

Turn a fuzzy goal into an executable workflow.

## Process
1. Restate the goal as a done-when condition.
2. List inputs, outputs, constraints, and systems involved.
3. Decompose into steps that a human or agent can complete without improvising.
4. For each step: owner (human/agent), tool, input, output artifact, failure mode, retry/skip rule.
5. Mark what can run in parallel.
6. Cut steps that do not change the outcome.

## Rules
- Do not invent tool access the user does not have.
- Prefer boring reliable steps over a clever one-shot.
- Include a verification step before anything irreversible.
