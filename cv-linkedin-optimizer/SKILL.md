---
name: cv-linkedin-optimizer
description: Adapt a CV and LinkedIn profile to a specific job by highlighting relevant experience. Use when the user pastes a resume plus a job description, or asks to tailor LinkedIn About/Experience.
---

# CV and LinkedIn Optimizer

Tailor a CV and LinkedIn profile to one role without lying.

## Intake
Need the current CV (or bullets) and the target job description. LinkedIn About/Experience if they want both.

## Process
1. Extract the job's must-haves, nice-to-haves, keywords, and seniority.
2. Map the user's evidence to each must-have. Mark gaps honestly.
3. Rewrite bullets as: action + scope + result (number if real).
4. Reorder so the top third of the CV matches the job.
5. Produce a LinkedIn About (first 2 lines must work as the preview) and 3 rewritten experience bullets.

## Output
- Fit score vs the JD (must-haves covered / missing)
- Tailored CV (plain text)
- LinkedIn About
- Headline options (3)
- Keyword list actually used
- Gaps not to fake

## Rules
- Never invent titles, dates, tools, metrics, or employers.
- If a metric is missing, write a qualitative result or leave a `[METRIC]` stub.
- Keep the user's voice; do not turn everyone into a "results-driven synergy" clone.
