---
type: system
status: draft
tags: []
sources: []
aliases: [Coordinates, Obscurity, Coordinate Database, Mortal Home]
updated: 2026-06-28
---

# Coordinates & Obscurity

How hidden homes get found — the mechanism behind the **mortal home**: protection is obscurity (a decaying share-trail), not invulnerability. [tentative]

## Purpose

- Gives real, ARK-style stakes back (a home _can_ be wiped) **without** the defender tax. The tax came from the **certainty** of offline loss; hidden coordinates remove the certainty, not the possibility.
- Only your **existence** is unloseable (see [[consciousness-link|Consciousness Link]]); your **civilization is mortal**.

## Coordinates as intel (COORD-1)

- You never build a new Gate; you **dial from the one you own** and save the **coordinate** — a re-dialable address in your homebase **coordinate database**.
- The DB is a **raidable asset** — a breach can steal the **map** (scouted planets and routes).
- A bookmark removes the _discovery_ cost, never the _travel_ cost (re-dialing still burns distance-scaled fuel).
- **Blind exploration-dialing** (dial the unknown for a fuel cost → a random planet of random richness/danger) is the variable-ratio hook for explorers. [leaning yes]

## Found by avatar-shares (SHARE-1)

- A home coordinate is a **geohash**; **every fielded avatar carries a share** of it.
- **Loot a dead avatar → get its share.** Below a threshold = a coarse region (hunt/scout, can't dial); at/above threshold = the exact dialable coordinate. Shares are **tradeable intel** — buy the last one you need in the [[world-types|Safe Core]].
- **Shares go stale.** A collected share **decays over time** — a trail assembled from old shares loses the lock as they age out, so a hunter has to keep you found by staying on you, and a player who goes quiet fades back into obscurity on their own. **Share-decay rate + the threshold _k_ are the master knobs** for the online:offline raid ratio.
- **Anti-dodge:** every fielded avatar carries a live share (no clean decoy avatars); shares decay rather than bank forever (no assembling a stale trail at leisure).

## The odds — what "safe" promises (player-facing)

The player-facing read of SHARE-1; the mechanism (shares + threshold + decay) is above, not restated.

- "Safe" is never a wall — it's a **high probability of staying unfound**. A home whose coordinate nobody has assembled simply can't be dialed; once someone has assembled it, it's raidable — online or off — but rarely, because assembling it is hard and the trail goes cold if they stop collecting.
- The odds move with **how you play, not a toggle**:
  - **Quiet, small, rarely out** → odds strongly in your favor: few avatars fielded = few shares shed; low [[potential|Potential]] keeps you off big hunters' reach.
  - **Loud, large, always out** → odds against you: many avatars leak shares fast; high Potential makes you visible and reachable; big tribes are findable by construction (endgame siege targets).
- **Offline tends _toward_ safety, not away from it.** While you're away you field no avatars, so you shed no new shares, and the shares a hunter already collected **decay as they age**. Quiet-and-safe last week ≈ still safe after a week away; loud-and-found before logging off is not. How strongly offline favors you is the **share-decay rate** (the master knob, SHARE-1).
- `reach = exposure` read as probability: the small are nearly unraidable, the big are worth the siege.

## Consequence — uphill relocates

- Home raids are gated by **finding** (assembling shares), not a power wall. Anti-whale-farm protection moves to [[potential|frontier-visibility]].
- Ownership is the **[[potential|tribe]]**: one shared coordinate, every member sheds shares of it — so big tribes are inherently **leaky** (endgame siege targets) and solos stay stealthy. `reach = exposure` at the group level.

## Why / rejected

- **Why mortal, not safe:** a perfectly-safe home makes the apex base un-raidable — inverts `reach = exposure` where it should bite, kills real stakes. Obscurity restores them without the tax (the tax was the _certainty_ of loss, not the possibility).
- **Rejected — inviolable home:** removes home stakes, makes the frontier pointless to leave.
- **Rejected — presence-gated wipe** (home falls only to a present defender): a no-show abuses it; obscurity makes it unneeded.
- **Rejected — a fail-closed seal** (logging off makes the Gate un-breachable): contradicted offline raiding and made obscurity redundant. Protection is **being unfound**, not a Gate state — see [[gates|Gates]] (GATE-2).
- **Rejected — permanent, never-fading coordinates:** a single leak would be forever, reviving the ARK certainty. Instead shares **decay** so the trail goes cold on its own, and you can **relocate** (claim a new Gate) for a fresh coordinate — recovery without an explicit re-key action (re-key removed).

## Data

- Threshold _k_, share-decay rate, reveal flavor (prefix-narrowing default vs. triangulation) — tunables in data. Numbers open.

## Code

Placeholder until the Unity project exists.

## Open questions

- Where "return home" lands if the home was wiped while you were away; tribe shared-ownership sub-rules (member churn, defection — can a defector sell the shared coordinate). Tracked in open-questions.md.
