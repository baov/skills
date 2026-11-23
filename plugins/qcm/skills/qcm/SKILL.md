---
name: qcm
description: Clarify with the user by asking multiple-choice questions (QCM) before doing the work. Use when the user says "qcm", "clarify with me", "ask me questions first", "MCQ mode", or when a request is ambiguous enough that guessing would change the result.
---

# QCM: clarify with multiple-choice questions

Before doing the work, clarify it with me by asking me questions, multiple-choice style.

## How to ask

- Use the host's multiple-choice question tool if there is one. Otherwise, write the question as text with numbered options, then stop and wait for my answer.
- One round at a time, 3 questions maximum per round. My answers shape the next round.
- Each question has 2 to 4 short, mutually exclusive options, plus an "Other / let me explain" option.
- Recommend an option when you have a view, and say why in one line.
- Ask only what I alone can answer. What you can find in the files, the code or the context, look up yourself.
- Ask in the language I write in.

## The shape of a round

1. **What I understood**: a short bulleted summary, so I can answer knowingly.
2. **What I'm unsure about**: the 1 to 3 questions.

## Special cases

- **"Your call" / "you decide"**: make a reasonable choice, say it explicitly, and move on without asking again.
- **Options that are not exclusive**: say it is multi-select and offer "all" and "none".
- **An answer outside the options**: take it literally, not the closest option.

## When to stop

- Stop asking as soon as the remaining unknowns would not change the result.
- Never ask again about something I already settled.
- Before starting the work, give a short recap of the decisions, then do the work.
