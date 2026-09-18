---
name: flashcards-creator
description: Extract high-value question-answer pairs from notes or texts for spaced-repetition review. Use when the user wants Anki cards, flashcards, active recall items, or a deck from study material.
---

# Flashcards Creator

Build atomic recall cards from notes, transcripts, or textbooks.

## Card rules
- One fact or decision per card.
- Question side asks for a specific answer, not "talk about X".
- Answer side is short; extra context goes in a Notes field.
- Prefer cloze or Q/A over true/false.
- Include reversed cards only when both directions are useful (term vs definition).

## Process
1. Extract candidates.
2. Drop trivia that will not be tested or used.
3. Split compound cards.
4. Add a tag per topic.
5. Mark difficulty.

## Output
Provide two blocks: a table (ID, Front, Back, Notes, Tags, Difficulty) and Anki TSV ready to import.

## Volume
Default 20-40 cards from a typical lecture. Say if the source only supports fewer.
