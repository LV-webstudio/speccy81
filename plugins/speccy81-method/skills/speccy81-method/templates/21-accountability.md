# Accountability (rule 2)

Closes **every** task, however short. It goes to the user or to the coordinator (and, with Wassup, to the direct channel and the
mailbox). If any section is missing, the task stays «not accounted for».

## Format
```markdown
## Accountability · <task> · <date and time>
Order (literal): «<exact text of the order, with who gave it and in which window>»
Done:
- <what was done, one line per item>
Proof: <commit, SHA-256 hash, path, log line or output of a command>
Proof: <one for each thing done; a bullet works too: «- Proof: …»>
Not done: <what was not done> — <why (permissions blocked, a datum is missing, out of scope)>
Not checked: <what is asserted without having been checked> | nothing
```

## Rules
- The line starts with `Proof:` (or `- Proof:`). Label by language: es Prueba · en Proof · ca, pt and it Prova ·
  fr Preuve (with a space before «:») · de Nachweis · nl Bewijs · pl Dowód.
- The words **done, checked, uploaded, deployed, deleted, installed, published and applied** without a
  `Proof:` in the same section are a warning.
- A proof is something another person can look at again: «I saw it» is not proof; «the app saved it» is not either, if
  it has not been read back at the destination.
- What could not be proved is said under «Not checked», with who must do it (e.g. «real iPhone: pending
  device»).
- If an error later turns up in something already accounted for, an **erratum** with the same header and «Corrects: <date>».

## Example
```markdown
## Accountability · guide index · 2026-03-01 10:40
Order (literal): «Fix the broken links in the index» (user, in the build window)
Done:
- 3 links fixed in GUIDE.md
Proof: commit 4f2a9c1
Proof: `validate-knowledge.sh` → «0 broken links»
Not done: the index of the English README — not this session's (owner: review)
Not checked: nothing
```
