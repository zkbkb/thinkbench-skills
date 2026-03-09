# ThinkBench Skills

A collection of Claude skills I wrote for the thinking and writing workflows I use most.

## What is this?

These are custom [Claude skills](https://docs.anthropic.com/en/docs/build-with-claude/projects#skills) for Claude.ai (web and desktop). They target cognitive work rather than code generation or file manipulation — the kind of tasks where you need to compare, structure, draft, and refine ideas.

Each skill encodes a workflow I've found myself repeating, so I don't have to re-explain the process every time.

## Skills

| Skill | Description |
|---|---|
| <a href="skills/doc-merge/"><nobr>doc-merge</nobr></a><br><a href="https://manus.im/app#settings/skills/import?githubUrl=https://github.com/zkbkb/thinkbench-skills/tree/main/skills/doc-merge"><img src="https://raw.githubusercontent.com/zkbkb/thinkbench-skills/main/assets/manus-glyph.svg" width="14" height="14" alt="Manus" style="vertical-align:middle;margin-right:4px"/>Import to Manus</a> | Multi-document semantic comparison and interactive merge resolution. Takes multiple documents on the same topic, diagnoses differences at multiple levels (framework, structure, argument, expression), and guides you through resolving conflicts into a single output. |
| <a href="skills/context-handoff/"><nobr>context-handoff</nobr></a><br><a href="https://manus.im/app#settings/skills/import?githubUrl=https://github.com/zkbkb/thinkbench-skills/tree/main/skills/context-handoff"><img src="https://raw.githubusercontent.com/zkbkb/thinkbench-skills/main/assets/manus-glyph.svg" width="14" height="14" alt="Manus" style="vertical-align:middle;margin-right:4px"/>Import to Manus</a> | Generates structured context handoff documents that compress a conversation's working state into a 12-module summary for seamless continuation in a new session. Inspired by Claude Code's `/compact` but redesigned for general-purpose conversations. |

## Usage

**Claude (for example):**

1. Go to **Claude.ai** > **Settings** > **Profile** > **Custom skills**
1. Upload the skill folder
1. Claude will automatically discover and use the skill when your task matches

**Manus:**

1. Click the **Import to Manus** link above
1. Confirm the import in Manus settings

Each skill folder contains a `SKILL.md` (core instructions) and optionally a `references/` directory with supporting materials and an `assets/` directory with templates.

## Repository structure

```text
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
├── assets/
│   └── manus-glyph.svg
└── README.md
```

## Licence

MIT
