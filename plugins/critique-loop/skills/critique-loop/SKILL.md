---
name: critique-loop
description: Challenges and critiques a deliverable (text, plan, code, idea, pitch) in an autonomous critique-and-fix loop, with no pause between iterations, rotating Edward de Bono's thinking hats. 10 iterations by default; the user can set the number ("critique-loop 5", "iterate 5 times"). Stops early when a pass finds no defect that changes the result. Use when the user says "critique loop", "iterate on this", "challenge and improve this", "stress-test this N times".
---

# Critique loop

Challenge and critique a deliverable, fix it, and repeat, without pausing between iterations. Then hand back the best version and what is still fragile.

## Setup

- **Target**: what the user points to. If they point to nothing, the last thing produced in the conversation.
- **Iterations**: 10 by default. If the user gives a number ("critique-loop 5", "iterate 5 times"), use it.
- Do not ask questions before starting, and do not stop between iterations to ask for validation.

## One iteration

1. **Pick a hat** (the blue hat's job, see below).
2. **Critique** the current version through that hat only. When the host can run a subagent, have the critique done by a fresh subagent that sees only the current version: no history, no previous versions, no reasoning behind them. Otherwise, critique as if you were seeing it for the first time.
3. **Fix** the defects found that change the result.
4. **Compare** with the best version so far and keep the better one. A fix that breaks something an earlier pass got right is rolled back.
5. **Log** one line: `Iteration N · <hat>: <what was found> → <what changed>`.

## The hats

| Hat | Critique angle | When |
|---|---|---|
| Black | Risks, flaws, errors, gaps in logic, contradictions | Every cycle |
| White | Facts and claims: is each one true and sourced? Check against something outside the model whenever possible: run the tests or the code, search the web, open the source. | Every cycle |
| Green | Alternatives: a simpler or better way to reach the same goal | Every cycle |
| Yellow | Strengths: what works and must not be lost in the next fixes | Every cycle |
| Red | Gut feeling: how a human reader or user will feel about it | Only when the deliverable is meant for people (pitch, post, email, UX) |
| Blue | Steering: picks the next hat and decides when to stop | Not a critique pass: it runs the loop |

The blue hat starts with black and adapts the order to what the previous passes found. Hats are a tool for changing angle, not a checklist: never run a pass only to cover a hat.

## When to stop

- **Early stop**: stop as soon as a full pass finds no defect that changes the result (an error, a gap in logic, a contradiction, a false or unsourced claim). Style and wording preferences do not count. Say why the loop stopped.
- Otherwise, stop at the iteration count.

## Output

1. The iteration log, one line per iteration.
2. Why the loop stopped (early stop or count reached).
3. The final version (the best one, not necessarily the last).
4. What is still fragile: the defects that remain, and the blind spots of a loop where the same model critiques and fixes.
