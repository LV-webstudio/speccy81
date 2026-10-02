# Idempotent memory (rule 11)

## Principles
- **One topic per file** and a **short index** (`MEMORY.md`: one line per file).
- **State files** (what changes): **rewritten in full** with «State as of <date and time>», never with text
  appended at the end. **Decision files** (what is stable): not touched unless the decision changes.
- **A `resume.md`** as the entry point. It is rewritten at the close of each phase or block, and always before
  restarting a long session (instead of compacting).
- Links between files with `[[name]]`. Nothing that the repository already keeps (code, git history).
- **No secrets or third-party data.** The user's own data goes only in local memory.
- **Compact only when a block is closed**, with the memory already saved; if it happens by itself, work resumes from `resume.md`.

## `resume.md` template
```markdown
---
name: resume
description: START HERE when opening a new session on <project>: where things were left, open threads and what to check first
metadata:
  type: project
---

**State as of <date time>.** Idempotent file: rewritten in full at the close of each block.

## What to check first (5 minutes)
1. <last commit / clean tree>
2. <mailbox or status of other machines>
3. <active sessions and their names>

## Open threads (in order)
| # | Thread | Next step | Where |
|---|---|---|---|

## Working rules that do not change
- <the project's inviolable rules>
```

## State file template
```markdown
---
name: <topic>
description: <one line to decide whether it is relevant>
metadata:
  type: project
---

**State as of <date time>.** Rewritten in full.

- <fact> · <where> · <pending> · <decision awaiting the user>

See [[resume]].
```

## Index (`MEMORY.md`)
```markdown
- [RESUME · start here](resume.md) — where the work was left and what to check
- [<Topic>](<topic>.md) — <one-line hook>

State files (…): they are REWRITTEN in full at the close of each block. The rest are stable decisions.
```
