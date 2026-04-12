<div align="center">
  <h1>agent-skills</h1>
  <p><b>Reusable skills for how I build, think, write, and learn.</b></p>
</div>

## Why

This repository is a personal skill library built on the Agent Skills format.

The goal is to encode practical engineering habits into reusable skill folders so they can be improved over time and reused across projects.

## Skills

| Skill | Focus |
| :--- | :--- |
| [`frontend-design`](skills/frontend-design/SKILL.md) | Designing web interfaces and UI direction |
| [`think`](skills/think/SKILL.md) | Challenge the problem and validate architecture before building |
| [`write`](skills/write/SKILL.md) | Write and edit text to sound natural |
| [`learn`](skills/learn/SKILL.md) | Deep learning workflow (details to be expanded) |
| [`research`](skills/research/SKILL.md) | Structured topic research before decisions |
| [`read`](skills/read/SKILL.md) | Fetch and normalize content from online sources |

## Install

Install directly from GitHub with the `skills` CLI.

### Codex

```bash
npx skills add janakirampuli/agent-skills -a codex -g -y
```

### Claude Code

```bash
npx skills add janakirampuli/agent-skills -a claude-code -g -y
```

Notes:
- Remove `-y` if you want interactive selection instead of installing all skills.
- Re-run the same command anytime to get updates.
- After install, restart your tool and run `/skills` to verify available skills.

## Structure

```text
.
├── LICENSE
├── README.md
└── skills
    ├── frontend-design
    │   └── SKILL.md
    ├── think
    │   └── SKILL.md
    ├── write
    │   └── SKILL.md
    ├── learn
    │   └── SKILL.md
    ├── research
    │   └── SKILL.md
    └── read
        └── SKILL.md
```

## Template

Skills follow the Anthropic template format:
- YAML frontmatter with `name` and `description`
- Markdown instructions body (some skills are still placeholder scaffolds)

## Inspiration

- https://agentskills.io/what-are-skills
- https://github.com/anthropics/skills
- https://github.com/openai/skills
- https://github.com/tw93/Waza
