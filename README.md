# skills

A collection of Claude Code skills by baov. Each skill is a separate plugin, so you install only the ones you want.

## Skills

| Skill | What it does |
|---|---|
| [ikigai-business-ia](plugins/ikigai-business-ia/skills/ikigai-business-ia/SKILL.md) | Generates AI business ideas from your Ikigai (what you love, what you're good at, what the world needs, what you can be paid for), one multiple-choice question at a time. It checks the market on the web with sources, scores a short-list of three and runs it through a Blue Ocean ERRC grid. |

## Install

### As a Claude Code plugin

```
/plugin marketplace add baov/skills
/plugin install ikigai-business-ia@baov-skills
```

### Manual skill install

Copy a skill folder into your personal skills (`~/.claude/skills/`) or your project's (`.claude/skills/`):

```
cp -r plugins/ikigai-business-ia/skills/ikigai-business-ia ~/.claude/skills/
```

## See also

- [handson](https://github.com/baov/handson): a strict sparring partner that never writes your code.
- [Proof Over Vibes](https://github.com/baov/proof-over-vibes): a spec-driven workflow for coding agents.

## License

MIT
