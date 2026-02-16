# ThinkBench Skills

A collection of Claude skills I wrote for the thinking and writing workflows I use most.

## What is this?

These are custom [Claude skills](https://docs.anthropic.com/en/docs/build-with-claude/projects#skills) for Claude.ai (web and desktop). They target cognitive work rather than code generation or file manipulation — the kind of tasks where you need to compare, structure, draft, and refine ideas.

Each skill encodes a workflow I’ve found myself repeating, so I don’t have to re-explain the process every time.

## Skills

|Skill                         |Description                                                                                                                                                                                                                                                             |
|------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|[doc-merge](skills/doc-merge/)|Multi-document semantic comparison and interactive merge resolution. Takes multiple documents on the same topic, diagnoses differences at multiple levels (framework, structure, argument, expression), and guides you through resolving conflicts into a single output.|

## Usage

1. Go to **Claude.ai** > **Settings** > **Profile** > **Custom skills**
1. Upload the skill folder
1. Claude will automatically discover and use the skill when your task matches

Each skill folder contains a `SKILL.md` (core instructions) and optionally a `references/` directory with supporting materials and an `assets/` directory with templates.

## Repository structure

```
thinkbench-skills/
├── skills/
│   └── doc-merge/
│       ├── SKILL.md
│       ├── references/
│       │   ├── difference_taxonomy.md
│       │   ├── alignment_strategy.md
│       │   ├── output_formats.md
│       │   ├── resolution_workflow.md
│       │   └── batch_logic.md
│       └── assets/
│           ├── diagnostic_report_template.html
│           └── resolution_batch_template.html
└── README.md
```

## Licence

MIT
