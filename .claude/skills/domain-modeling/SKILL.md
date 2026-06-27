---
name: domain-modeling
description: Build and sharpen the project's shared language and decision record. Use when pinning down terminology (the docs/CONTEXT.md glossary), recording a design decision (DDR) or an architecture decision (ADR), or when another skill needs to maintain these.
---

# Domain Modeling

Actively build and sharpen the project's shared language and decisions as you
design — challenge fuzzy terms, stress-test with scenarios, and write the glossary
and decisions down the moment they crystallise. (Merely *reading* docs/CONTEXT.md
for vocabulary is a one-line habit any skill can do; this skill is for *changing*
the model.)

Two decision registers, one glossary:
- **DDR — Design Decision Record:** a game / world / lore / mechanics choice.
  Lives in `docs/ddr/`. Format: [DDR-FORMAT.md](./DDR-FORMAT.md).
- **ADR — Architecture Decision Record:** a technical / software choice (the
  eventual Unity code, the repo, tooling). Standard ADR. Lives in `docs/adr/`.
  Format: [ADR-FORMAT.md](./ADR-FORMAT.md).
- **Glossary — `docs/CONTEXT.md`:** the ubiquitous language. Format:
  [CONTEXT-FORMAT.md](./CONTEXT-FORMAT.md).

Create files lazily — only when there is something to write.

## During the session

### Challenge against the glossary
When a term conflicts with docs/CONTEXT.md, call it out at once. "CONTEXT defines
`gate-open` as full exposure, but you're using it for trade — which is it?"

### Sharpen fuzzy language
When a term is vague or overloaded, propose one canonical word and list the rest
under `_Avoid_`. "You said 'portal' — that's a Gate. Keep one word."

### Stress-test with scenarios
When relationships are being worked out, invent concrete edge cases that force
precision about the boundaries between concepts.

### Update CONTEXT.md inline
When a term resolves, write it to docs/CONTEXT.md right then — don't batch. It is a
**glossary and nothing else**: no lore, no mechanics, no implementation. Use the
format in [CONTEXT-FORMAT.md](./CONTEXT-FORMAT.md).

### Offer a decision record sparingly
Offer a DDR or ADR only when all three hold:
1. **Hard to reverse** — changing your mind later costs real work.
2. **Surprising without context** — a future reader will ask "why this way?"
3. **A real trade-off** — there were genuine alternatives and you picked one.

Miss any one, skip it. Pick the register: design/world → DDR, technical/code → ADR.
Record the *why* and *what you rejected* — not ceremony.

### Graduate open questions
docs/open-questions.md is the backlog of unresolved decisions. When one settles,
write the DDR/ADR, flip the relevant page tag `[tentative]→[decided]`, and strike
it from open-questions.
