---
name: practice
description: Create a quiz, flashcards and a spaced-repetition review schedule from a learning-path module, lesson notes or a topic the user is studying, and save the flashcards to Kuliko when that connector is connected and the user asks. Use when the user asks to be tested, wants practice questions, flashcards or a review schedule, or finishes a module and wants to check understanding.
---

# Practice

## Ground rules

- Base questions on the material the user is studying: the plan module, the notes from this conversation, course material from a connector, or text they pasted. If there is none, ask what to cover instead of guessing.
- Every question needs a correct answer and a one-line explanation. Where the source has a timestamp or section, point to it.
- Do not invent facts. If the source is thin, make fewer questions rather than padding.
- Write in the language the user writes in.

## Quiz

1. Ask only what you need: which module or notes, how many questions (default 10), and difficulty (default mixed).
2. Mix question types: recall, understanding, application, and at least one "spot the mistake" item when the topic allows it.
3. Present the questions first, without answers. Put the answer key after a clear separator and tell the user to try before looking.
4. If the user answers, grade briefly, name the concept behind every miss, and suggest which lesson or section to revisit.

## Flashcards

1. Make one card per idea: a short question on the front, a short answer on the back. Aim for 10-20 cards per module.
2. Show the cards in the conversation first.
3. If the Kuliko connector is connected and the user asks to save them, create one subject per learning path (reuse it when it already exists in this conversation) and add the cards. Confirm the subject name before creating it. Never delete or edit cards you did not create in this conversation.
4. If Kuliko is not connected, offer the cards as a table the user can import elsewhere.

## Review schedule

Suggest reviewing after 1, 3, 7, 14 and 30 days, and list which questions to repeat on each date. When Kuliko holds the cards, tell the user to check its due counts instead. Offer to put review sessions on the calendar with `/studypath:save`; create nothing without being asked.

## Calibration

Short answer beats multiple choice for deeper checks. When the user misses more than half, say so kindly and propose reviewing the module before moving on.
