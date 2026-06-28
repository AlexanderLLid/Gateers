---
status: accepted
---

# Architecture & tech stack: server-authoritative, Gate-instanced, Unity/C#

How the game is built. The Gate fiction is an **engineering device dressed as lore** — most of the hard survival-MMO problems are removed by it rather than solved (see [technical-challenges.md](../technical-challenges.md)).

## Networking / authority

- **Server-authoritative always.** One authority owns each planet at all times — no authority transition between solo and contested play to reconcile or exploit.
- **Cost cap = the presence requirement, not offloaded simulation.** A base is live only while its owner is online; sealed/offline = nothing to simulate. One bounded exception: a home whose [[coordinates|coordinate]] has been assembled can be raided offline (rare — finding gates it), so cost still scales ≈ with active players.
- **Three-state planet model:** **empty** (a DB row) → **solo-occupied** (a cheap server-side tick) → **contested** (a full server-authoritative instance spun up).
- **Seed-plus-deltas storage**, lazy-loaded on demand → **server cost ∝ online players, not world size.**
- **Gate-based instancing** is the foundational cost advantage vs. a persistent shared world.

## Tech stack

- **Unity with C#** (matches the designer's language comfort).
- **Native-first**, with a **web export** as a demo/playtest funnel (a slice, not parity).
- A **`PlanetGenerator` abstraction from day one** so procedural generation is a single-class swap later.
- The **Gate mechanic is the [[mask-energy|mask-energy]] source** — an engine-level tie between Gate energy, survivable range, the raider clock, and home-soil advantage.

## Open

- Matchmaking and how bilateral tunnels are instanced; hosting model; netcode library/transport; persistence backend.

## Why / rejected

- A persistent shared world simulated 24/7 is the genre default this avoids — it's the single biggest server cost, removed by presence + sealed-by-default.
- Authority hand-off between models (common in survival MMOs) is sidestepped by server-authoritative-always.
