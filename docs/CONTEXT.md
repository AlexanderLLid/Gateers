# CONTEXT.md - Shared Language

The working vocabulary for Gaters. Use these terms consistently in pages, code,
commits, and chat. Add a term when a concept keeps needing a sentence to
explain. This is a glossary, not canon; it decodes jargon.

## Core concept
- Gate - the network device connecting planet-bases. Sealed by default. A *stable*
  wormhole; cannot be manufactured, only found/claimed/repaired.
- Planet-base - a single player's planet and home base.
- Gater - a player/operator who goes out through the Gates into the world. The game
  is named after them.
- Hub world - a neutral, lawless crossroads world for staging raids and routing
  trade to distant partners.
- Rift - an *unstable* wormhole: spontaneous, uncontrollable, self-collapsing on a
  countdown. Opens near Gates onto opt-in content. The PvE/loot event engine.
- The Lattice - the full network of Gates (placeholder name).
- Coordinates - a re-dialable Gate address; intel you discover, trade, steal, hide.
- Power core - scarce, scavenged Gate fuel; the primary activation cost.
- Charter / tithe - the license to hold a Gate-world, and the cut owed for it.

## Exposure states
- Sealed - gate closed, planet safe. The default safety guarantee.
- Port open - partial exposure for trade.
- Gate open - full exposure; raiding is possible.
- Siege timer - the committed window once a gate is opened.
- Mask energy - life-support drawn from the Gate; bounds survivable range and acts
  as the raider timer. Split into two numbers (below).
- Sustaining field - the bubble an active Gate projects; the mask tops up inside it.
  The soft world border (a cost gradient, not a wall).
- Field radius - how far you can roam/build; the dev-tunable expansion knob.
- Away reserve - how long the mask lasts once you leave a field; the raider clock.
  Kept decoupled from field radius on purpose.

## Planet runtime states
- Empty - a database row only.
- Solo-occupied - one owner present; client-authoritative PvE.
- Contested - a raid or trade in progress; server-authoritative instance.

## Storage
- Seed-plus-deltas - planets stored as a seed plus changes, lazy-loaded on
  demand, so server cost scales with online players.

## Stack
- Unity with C#. Server-authoritative only during contested sessions.

(Replace or extend as the design firms up. Keep each definition to a line.)
