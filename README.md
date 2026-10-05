# Pi Agent Learning

A source-driven learning workspace for understanding Pi Agent from first principles.

This repository follows a stateful teaching workflow inspired by Matt Pocock's `teach` skill:

```text
Mission
  ↓
Technical Foundation
  ↓
Primary Source Reading
  ↓
Source Walkthrough
  ↓
Execution Trace / Mental Model
  ↓
Practice
  ↓
Learning Gate
  ↓
Learning Record
  ↓
Next Lesson
```

## Learning rule

For Pi facts, source priority is:

1. **Current Pi source code**
2. **Current Pi official docs**
3. **Matt Pocock's teach skill** for teaching methodology
4. **Uploaded Bilibili subtitle** as a secondary explanatory reference only

If the subtitle and current source disagree, the current source wins and the difference should be recorded explicitly.

## Workspace

- [MISSION.md](MISSION.md) — why we are learning Pi and what "done" means
- [ROADMAP.md](ROADMAP.md) — lesson sequence and learning gates
- [RESOURCES.md](RESOURCES.md) — primary and secondary sources
- [NOTES.md](NOTES.md) — teaching preferences and working notes
- [lessons/](lessons/) — short, self-contained lessons
- [reference/](reference/) — compressed references for later lookup
- [learning-records/](learning-records/) — evidence of what has actually been learned
- [assets/](assets/) — reusable lesson assets

## Current status

**Lesson 01 — Minimal Agent Loop:** prepared, not yet passed.

Open: [lessons/0001-minimal-agent-loop.html](lessons/0001-minimal-agent-loop.html)

## Primary codebase

Pi: https://github.com/earendil-works/pi

The first source path is:

```text
packages/agent/src/
├── types.ts
├── agent.ts
└── agent-loop.ts
```

The goal is not merely to use Pi CLI. The goal is to be able to read the implementation, reconstruct its execution model from memory, evaluate its design trade-offs, and modify or reimplement the core ideas independently.
