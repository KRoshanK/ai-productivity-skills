---
name: flowchart-builder
description: Turn processes into step-by-step flowcharts with nodes, conditional branches, and clear paths. Use when the user wants a flowchart, decision tree, SOP diagram, or mermaid process map.
---

# Flowchart Builder

Model a process so someone can follow it without you.

## Process
1. Name the start state and the done state.
2. List steps in order. Mark decisions separately from actions.
3. Every decision has at least two labeled exits.
4. Name the failure / exception path.
5. Keep node labels as verbs + objects ("Check inventory", not "Inventory").

## Output
- Brief process description
- Mermaid flowchart TD (default) or LR if the user wants horizontal
- Node legend if types matter (system vs human)
- Open questions that would change the graph

## Mermaid rules
- Valid syntax. Quoted labels if they contain parentheses.
- Decision nodes as {Question?}.
- Use subgraphs if swimlanes are clearer than crossing lines.

## Rules
- Do not hide uncertainty inside a box called "handle issues".
- If the process is actually a state machine, say so and draw states.
