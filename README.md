# skills

A collection of Claude Code skills by baov. Each skill is a separate plugin, so you install only the ones you want.

## Skills

| Skill | What it does |
|---|---|
| [ikig-ai-business](plugins/ikig-ai-business/skills/ikig-ai-business/SKILL.md) | Generates AI business ideas from your Ikigai (what you love, what you're good at, what the world needs, what you can be paid for), one multiple-choice question at a time. It checks the market on the web with sources, scores a short-list of three and runs it through a Blue Ocean ERRC grid. |
| [ruthless-mentor](plugins/ruthless-mentor/skills/ruthless-mentor/SKILL.md) | A ruthless mentor that sugarcoats nothing. It challenges your assumptions, points out your blind spots and tells you bluntly, and exactly why, when an idea or reasoning is weak, until it holds up. |
| [mcq](plugins/mcq/skills/mcq/SKILL.md) | Clarifies a request with you through multiple-choice questions (MCQ) before doing the work: one question at a time until the subject is clear, with a recommended option and an "Other" escape hatch. |

## Install

### As a Claude Code plugin

```
/plugin marketplace add baov/skills
/plugin install ikig-ai-business@baov-skills
/plugin install ruthless-mentor@baov-skills
/plugin install mcq@baov-skills
```

### Manual skill install

Copy a skill folder into your personal skills (`~/.claude/skills/`) or your project's (`.claude/skills/`):

```
cp -r plugins/ikig-ai-business/skills/ikig-ai-business ~/.claude/skills/
```

## See also

- [handson](https://github.com/baov/handson): a strict sparring partner that never writes your code.
- [Proof Over Vibes](https://github.com/baov/proof-over-vibes): a spec-driven workflow for coding agents.

## License

MIT
