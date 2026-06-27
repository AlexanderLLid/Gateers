---
name: lore-options
description: Grounded lore paths — propose two or three distinct ways to resolve a lore question or close a hole, each naming the buildable mechanic or server/scaling lever it licenses. Reached when resolving an open question, and by the skeptic and lore-architect agents when they need to offer paths.
---

# Lore Options

Turn a lore question or hole into a short menu of **grounded** paths the human can pick from.

## Grounded is the bar

A path is **grounded** when its fiction earns its keep by licensing a concrete thing the devs can build, tune, or scale. The test for every path: *name the lever it hands the devs.* Fiction with no lever is colour, not a path — cut it.

The levers already live in the tech model (`docs/CONTEXT.md` → Storage, Stack, Planet runtime states, Field radius). Map fiction onto these, or onto a new lever devs can clearly build:

- **Reachability** — which worlds are live. *Empty = a DB row only*, seed-plus-deltas, lazy-loaded. Lore that gates *which Gates open* is really lore that decides *when a planet-server is provisioned*. ("Not all Gates are open" → a server spins up only when its Gate is dialed and fueled.)
- **World border** — how far a player roams. *Field radius* is the dev-tunable knob; the *sustaining field* is the soft border. Lore that bounds movement sets the streaming/border radius. ("Can't go past X from the Gate" → mask energy decays beyond the field.)
- **Instancing** — who is authoritative. *Solo-occupied = client-authoritative; Contested = server-authoritative instance.* Lore that decides when others reach you decides when an instance spins up.
- **Cost / scarcity** — *power cores* gate activation; the *tithe* gates holding. Lore that throttles activity maps to a resource sink devs balance.

## Method

1. **Find the lever first.** Ask which buildable knob is really at stake (reachability / border / instancing / cost / a new one). The fiction exists to justify *that*.
2. Produce **two or three genuinely distinct paths** — distinct in *mechanism*, not flavour. Three re-wordings of one idea is one path.
3. Order them **cheapest first** — least existing canon and least new tech disturbed at the top, so the quick pick is usually #1.
4. For each path, one line: **the fiction → the lever it licenses → its trade-off.**
5. **Don't pad.** Two real paths? Give two. If nothing is grounded, the finding is that the question needs a buildable lever before lore can answer it.
6. **Always recommend.** End by naming the path you'd pick and the one-line why. The pick need not be the cheapest — when it isn't, say what justifies the extra cost.

## Shape

> **Path A (cheapest)** — <fiction>. Licenses: <lever devs build/tune>. Trade-off: <what it costs>.
> **Path B** — <fiction>. Licenses: <lever>. Trade-off: <…>.
> **Path C** — <fiction>. Licenses: <lever>. Trade-off: <…>.
>
> *Recommend:* <which, and the one-line why>.
