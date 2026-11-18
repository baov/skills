---
name: ikig-ai-business
description: Generates AI business ideas from the user's Ikigai (what they love / what they're good at / what the world needs / what they can be paid for), through multiple-choice questions one at a time, checks the market on the web, scores the ideas and runs the short-list through Blue Ocean. Use when the user is looking for an AI business idea, an AI SaaS, a profitable side project, or says "find me a business idea", "my ikigai", "what should I launch with AI".
---

# Ikigai AI business

Goal: surface 8 to 10 AI business ideas grounded in the user's Ikigai, then dig into 3 of them, scored and tested against the real market.

## Cross-cutting rules

- **Announce**: at the start, say in one sentence that the skill applies and what it will produce. Do not start silently.
- **One multiple-choice question at a time**: every question is multiple choice (question tool if available, otherwise a numbered list) and always includes an "Other" option. The answer shapes the next question. Never a block questionnaire.
- **Validation gates**: each phase ends with a short summary the user validates before moving to the next.
- **Persistence**: keep `ikigai-progress.md` up to date (current phase, answers, ideas, scores, sources). On every start, look for this file and offer to resume.
- **Honesty**: flag plainly an idea that misses a circle. Do not inflate scores. Market facts come from cited sources, never from memory.
- Language: English.

## Phase 0 — Framing

1. Read the user's memory / profile and pre-fill what is already known (job, stack, past projects, interests). Present this pre-fill for validation: the user corrects it, nothing is taken for granted.
2. Multiple choice: which framing for "AI business"?
   - **A. AI product**: AI is the value being sold (SaaS, agent, tool).
   - **B. Agent-run business**: any sector, set up and run solo with agents.
3. Record the framing in the progress file.

## Phase 1 — The 4 circles (iterative multiple choice)

One circle at a time, 2 to 4 questions per circle, starting from the pre-fill:

1. **What I love**: topics, problems that excite, what one would work on for free.
2. **What I'm good at**: skills, domain expertise, privileged access (network, data, sector).
3. **What the world needs**: observed problems, lived frustrations, underserved populations.
4. **What I can be paid for**: who has a budget, which models (subscription, service, commission).

Gate: summary of the 4 circles + the 4 intersections (passion, mission, vocation, profession). Validation.

## Phase 2 — Generation (8 to 10 ideas)

- Each idea must start from at least one concrete element of each circle, cited.
- Format per idea: name, one-sentence value proposition, target, role of AI (framing A) or role of agents in operations (framing B), Ikigai elements used.
- Vary the models (B2B / B2C, product / service) to avoid 10 variants of the same idea.

Gate: the user picks 3 ideas through a multi-select multiple-choice question (the skill may recommend, the user decides).

## Phase 3 — Market check (web research)

For each of the 3 ideas:
- demand: signals of need (searches, communities, calls for tender);
- competition: existing players, observed prices;
- willingness to pay: prices charged for comparable offers.

Always cite sources. Say explicitly when the signal is weak or cannot be found.

## Phase 4 — Scoring

Three criteria scored from 1 to 5 (four in framing B), each with a one-line justification:

| Criterion | Question |
|---|---|
| Coverage of the 4 circles | Score per circle; a circle at 1 or 2 = named red flag (passion without a market, a job without joy, etc.) |
| Verified market signal | Does phase 3 show real demand that can pay? |
| Defensibility | What stops a competitor or a general-purpose LLM from doing the same tomorrow? |
| Solo + agents feasibility (framing B only) | Which operating tasks stay human (customer relations, logistics, regulation, physical presence)? A recurring human task that cannot be delegated = score ≤ 2 |

No average that hides a zero: an idea with a criterion at 1 is flagged whatever its total.

## Phase 5 — Blue Ocean

For each short-listed idea: an ERRC grid (Eliminate, Reduce, Raise, Create) against the competitors found in phase 3, and the value curve summed up in one sentence.

## Phase 6 — Deliverable

Produce a document (Docs-type if available, otherwise Markdown):
1. The user's Ikigai (4 circles + intersections)
2. The 8 to 10 generated ideas (one line each)
3. The 3 ideas in depth: sourced market, scores, ERRC grid
4. Argued recommendation and main risks
5. Concrete next steps to validate the chosen idea (interviews, landing page, pre-sale)
6. Sources

Mark the progress file as "done".
