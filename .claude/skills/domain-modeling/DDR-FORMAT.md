# DDR Format

Design Decision Records live in `docs/ddr/` and use sequential numbering:
`0001-slug.md`, `0002-slug.md`, etc. Create the directory lazily — only when the
first DDR is needed.

A DDR is the design/world counterpart of an ADR: it records a choice about how the
*game* works, not how the *code* is built.

## Template

```md
---
status: accepted        # proposed | accepted | superseded by DDR-NNNN
---

# {Short title of the decision}

{1-3 sentences: the context, what we decided, and why. Name what you rejected when
the rejection is non-obvious.}
```

A DDR can be one paragraph. The value is recording *that* a design choice was made,
*why*, and *what was rejected* — not filling out sections. Drop the `status`
frontmatter once a decision is settled and unlikely to be revisited.

## Numbering
Scan `docs/ddr/` for the highest existing number and increment by one.

## When to offer a DDR
All three must hold:
1. **Hard to reverse** — or it shapes a large amount of downstream design.
2. **Surprising without context** — a future reader will wonder "why this way?"
3. **A real trade-off** — genuine alternatives existed and you picked one.

**The decisive test:** would a future agent, lacking this record, plausibly re-make
the decision *differently*? If nobody would ever re-propose the alternative, don't
record it. And never write backward-compat or "supersedes the old X" history —
nothing is locked and there are no users (see CLAUDE.md).

### What qualifies
- **Core pillars / theses.** "Reach equals exposure." "No base decay, ever."
- **Cosmology and world rules.** "Gate vs Rift = propped vs un-propped wormhole."
- **Scope / boundary calls.** "Players are human." "The title is Gaters."
- **Deliberate deviations from the genre-obvious** — anything a reasonable reader
  would assume the opposite of; stops the next person re-proposing it.
- **Rejected alternatives when the rejection is subtle** — e.g. uniform mask-death
  vs. asymmetric; record why asymmetric won so it isn't re-litigated.
