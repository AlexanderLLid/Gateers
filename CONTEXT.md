# CONTEXT.md - Shared Language

The working vocabulary for Gaters. Use these terms consistently in pages, code,
commits, and chat. Add a term when a concept keeps needing a sentence to
explain. This is a glossary, not canon; it decodes jargon.

## Core concept
- Gate - the network device connecting planet-bases; a stable, controllable
  wormhole. Sealed by default.
- Planet-base - a single player's planet and home base.
- Hub world - a neutral, lawless crossroads world for staging raids and routing
  trade to distant partners.
- Rift - a spontaneous, unstable wormhole that collapses on a countdown. Opens
  onto content (PvE pocket / loot / monster spill) next to a Gate, never through
  a sealed Gate and never as a backdoor for players. The dopamine engine.
- Coordinates - a re-dialable address for a known planet. Information, not a
  Gate. Standardized term for the old "address".

## Cosmology
- Stable vs unstable - a Gate is a stable, engineered wormhole; a Rift is an
  unstable, spontaneous one. Two states of one physics. Rifts tear open near
  Gates. The Wake destabilized the network.
- Stabilizing - taming an unstable Rift into a permanent Gate; the (tentative)
  source of new, finite-but-replenishing Gates.

## Exposure states
- Sealed - gate closed, planet safe. The default safety guarantee.
- Port open - partial exposure for trade.
- Gate open - full exposure; raiding is possible.
- Siege timer - the committed window once a gate is opened (defender-side raid
  clock).

## Survival / mask
- Mask energy - life-support drawn from the Gate; the survival layer. Split into
  two independent numbers (below).
- Sustaining field - the bubble a Gate projects; the mask tops up inside it and
  drains on a gradient outside. Acts as the soft world border.
- Field radius - how far the sustaining field reaches; the dev-expandable world-
  size lever (authority-tuned). Must stay decoupled from away reserve.
- Away reserve - how long the mask lasts outside a field; the attacker-side
  raider timer.
- Mask-at-zero - asymmetric outcome: soft recall on home soil, downed/lootable
  in hostile territory.

## Discovery
- Coordinate database - per-homebase log of discovered coordinates; a raidable
  asset (steal the map). Re-dialing a saved coordinate still costs travel fuel.
- Blind dial - dialing into the unknown for a fuel cost; a random planet. The
  exploration slot machine.

## Planet runtime states
- Empty - a database row only.
- Solo-occupied - one owner present; client-authoritative PvE.
- Contested - a raid or trade in progress; server-authoritative instance.

## Storage
- Seed-plus-deltas - planets stored as a seed plus changes, lazy-loaded on
  demand, so server cost scales with online players.

## Stack
- Unity with C#. Server-authoritative only during contested sessions.

## Dev / meta
- Central authority - the in-world power that charters players; also the
  in-world voice for dev changes (see patch channel).
- Authority as patch channel - patches ship as "Directorate bulletins"; world
  expansion and balance changes are framed as the authority adjusting the
  network. Strong leaning, not yet locked.

(Replace or extend as the design firms up. Keep each definition to a line.)
