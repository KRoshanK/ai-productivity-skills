---
name: exam-preparer
description: Build a personalized mock exam from notes or a syllabus: multiple-choice, short answer, essay, and case questions with answers and a marking scheme. Use when the user wants practice questions, a simulacro, quiz generation, or exam prep from study material.
---

# Exam Preparer

Generate a realistic mock exam from the user's notes, syllabus, or textbook extract.

## Defaults
If the user does not specify:
- Length: 60 minutes
- Mix: 8 MCQ + 4 short answer + 2 essay/case
- Difficulty: match the source, with 20% stretch items
- Include an answer key in a second section

Ask only if duration, exam board style, or open-book vs closed-book is material.

## Process
1. Inventory topics and weight them by how central they are in the source.
2. Write questions that test application, not trivia copying.
3. For MCQ: 4 options, one correct, plausible distractors, no "all of the above".
4. For short answer: 2-6 mark style with a marking scheme.
5. For essay/case: a prompt, required structure, and a rubric (content, reasoning, precision).
6. Tag each item with topic + difficulty (easy / medium / hard).

## Output
### Paper
- Header: subject, time, total marks, allowed materials
- Numbered questions
- Mark totals that add up

### Answer key (separate heading)
- Correct option + 1-line rationale for MCQ
- Bullet mark scheme for short answers
- Rubric + model outline for essays

## Rules
- Do not leak answers inside the paper.
- Cover the syllabus; do not cluster all hard items at the end.
- If the source is too thin for a fair paper, say so and generate a shorter quiz.
