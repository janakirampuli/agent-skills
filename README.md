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

Each skill currently uses a template-only `SKILL.md` based on the Anthropic skills template format:
- YAML frontmatter with `name` and `description`
- Placeholder body (`# Insert instructions below`)

No workflow content has been added yet.

## Inspiration

- https://agentskills.io/what-are-skills
- https://github.com/anthropics/skills
- https://github.com/openai/skills
- https://github.com/tw93/Waza
