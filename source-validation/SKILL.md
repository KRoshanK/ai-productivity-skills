---
name: source-validation
description: Filter information by reliability: judge whether a source is credible, detect bias, and say what can be trusted. Use when the user asks if a source is legit, wants a credibility check, or is mixing blogs, papers, and social posts.
---

# Source Validation

Evaluate sources before the user builds on them.

## Rubric (score 1-5 each)
- Primary vs secondary vs commentary
- Author expertise and accountability
- Method / evidence quality
- Conflicts of interest
- Track record and corrections
- Consistency with independent sources

## Process
1. Identify what the source is (paper, news, blog, official stats, thread, vendor page).
2. Score the rubric. Missing info = lower confidence, not a pass.
3. Separate: solid facts, plausible claims, unsupported claims.
4. Name likely bias direction (commercial, political, academic incentive).
5. Say what the user may rely on vs what needs a second source.

## Output
- Source card (type, author, date, outlet)
- Scores + one-line reason each
- Trust verdict: usable / usable with caveats / weak / do not use for decision X
- What to verify next

## Rules
- Do not treat "it went viral" as evidence.
- Do not smear; judge the piece and incentives.
- If you cannot verify a fact in this session, mark it unverified.
