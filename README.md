# ThinkBench Skills

A collection of Claude skills I wrote for the thinking and writing workflows I use most.

## What is this?

These are custom [Claude skills](https://docs.anthropic.com/en/docs/build-with-claude/projects#skills) for Claude.ai (web and desktop). They target cognitive work rather than code generation or file manipulation — the kind of tasks where you need to compare, structure, draft, and refine ideas.

Each skill encodes a workflow I've found myself repeating, so I don't have to re-explain the process every time.

## Skills

| Skill | Description |
|-------|-------------|
| [doc-merge](skills/doc-merge/SKILL.md) | Multi-document semantic comparison and interactive merge resolution. Takes multiple documents on the same topic, diagnoses differences at multiple levels (framework, structure, argument, expression), and guides you through resolving conflicts into a single output. |
| [context-handoff](skills/context-handoff/SKILL.md) | Generates structured context handoff documents that compress a conversation's working state into a 12-module summary for seamless continuation in a new session. Inspired by Claude Code's `/compact` but redesigned for general-purpose conversations. |

## Quick Install

| Skill | Manus | Claude |
|-------|-------|--------|
| **context-handoff** | [<img src="https://files.manuscdn.com/assets/image/brand/image/Manus-Glyph-Black.svg" height="14" alt="Manus"> Import to Manus](https://manus.im/app#settings/skills/import?githubUrl=https://github.com/zkbkb/thinkbench-skills/tree/main/skills/context-handoff) | Manual upload (see below) |
| **doc-merge** | [<img src="https://files.manuscdn.com/assets/image/brand/image/Manus-Glyph-Black.svg" height="14" alt="Manus"> Import to Manus](https://manus.im/app#settings/skills/import?githubUrl=https://github.com/zkbkb/thinkbench-skills/tree/main/skills/doc-merge) | Manual upload (see below) |

## Usage (Claude.ai)

**Claude (for example):**
1. Go to **Claude.ai** > **Settings** > **Profile** > **Custom skills**
1. Upload the skill folder
1. Claude will automatically discover and use the skill when your task matches

Each skill folder contains a `SKILL.md` (core instructions) and optionally a `references/` directory with supporting materials and an `assets/` directory with templates.

## Repository structure

```
thinkbench-skills/
├── skills/
│   ├── doc-merge/
│   │   ├── SKILL.md
│   │   ├── references/
│   │   └── assets/
│   └── context-handoff/
│       ├── SKILL.md
│       └── references/
│           └── prompt-template.md
└── README.md
```

## Licence

MIT
