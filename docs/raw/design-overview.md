# Gaters — Comprehensive Design Overview (Raw Braindump)

> **What this is.** A single, deliberately exhaustive dump of everything established
> about the game **Gaters** so far. It is *not* formatted as final wiki pages. Each
> concept gets its own named heading and a self-contained paragraph so another agent
> can lift it into its own page. Every claim is tagged:
> **[decided]** = firmly committed, **[tentative]** = current leaning / proposed,
> **[open]** = undecided / not yet established. Where two ideas conflict, the conflict
> is flagged rather than smoothed over. Recurring concepts use consistent names:
> **Gate**, **planet-base**, **hub world**, **sealed / port-open / gate-open**,
> **mask energy**, **siege timer**, **Rift**, **sustaining field**, **away reserve**,
> **coordinates**.
>
> **Naming note.** The title is **Gaters** [decided, recent]. Earlier drafts and the
> request header used "Gateers"; that is superseded. A phonetic/searchability concern
> for "Gaters" (reads as "gators"; the "gay-ter" / "gaiters" homophones) was raised and
> is **unresolved** — see Open Questions. The in-world term for a player/operator is
> **[open]** (candidates discussed: Gateers, Gaterunners, Gatehands).
>
> **Scope note.** Nothing in the Lore sections has been invented to fill gaps. Where a
> category (characters, species, religions, myths, languages) has no established content,
> it is listed explicitly as undecided rather than fabricated.

---

# PART I — LORE / WORLD

### Premise & Central Conflict
[decided] Gaters is a sci-fi multiplayer game in which each player controls a single
**planet-base** sitting on an ancient **Gate**. A long-dormant galaxy-spanning network of
Gates has suddenly switched on, and a **central authority** is deputizing independent
operators (the players) to find, claim, exploit, and hold the worlds those Gates sit on.
The central conflict is a **gold rush over finite, un-manufacturable Gate infrastructure**:
reach and wealth require opening your Gate, and opening your Gate is the only way you can be
attacked. The whole design exists to deliver the *aggressor* fantasy (raiding, PvP, looting)
without the *defender* tax (base-babysitting, decay, offline vulnerability, forced 24/7
presence) that the designer disliked in ARK and Rust.

### Design Thesis ("Reach equals exposure")
[decided] The single organizing principle: **you can only act on the world as far as you
have opened yourself to it; you choose when and toward whom; and you cannot be touched while
you are not present.** A **sealed** planet-base is safe by default but stagnant. Acting
(trading, raiding) requires opening, which creates risk. This is intended to be "MAD in
space": mutual vulnerability breeds deterrence, alliances, and "cover my Gate while I trade"
pacts emerge naturally.

### Origin Problem / Designer Intent
[decided] The project is a deliberate reaction to survival-PvP genre pain. **Loved** and to
be preserved: PvP combat, raiding/breaching, looting, high-stakes offense. **Hated** and to
be designed out: babysitting one's own base, upkeep/decay timers, getting raided while
offline, the "unpaid-labor" feeling of logging in to maintain rather than play, and being
forced online constantly to avoid loss. The diagnosis: persistent shared-world progress +
offline vulnerability mechanically rewards the highest-time-investment, most-aggressive
players and punishes everyone else, and "toxicity" and "base-babysitting" are two surfaces of
that one design choice.

### Setting & Tone
[tentative] Frontier sci-fi; a freshly-opened, lawless gold-rush among the bones of a
vanished precursor civilization. Tone leans toward dangerous-frontier-opportunity with an
undercurrent of cosmic unease (the network woke for a reason nobody understands). Aesthetic
touchstones below. Exact tone register (gritty vs. adventurous vs. eerie) is **[open]**.

### The Wake (the inciting event)
[tentative] The Gates were always present but **dormant and undetectable** for so long nobody
knew they existed. Then **something switched the entire network on at once** — "the Wake."
The central authority detected the system-wide activation. This is the in-world "year zero."
The name "the Wake" is a placeholder label for the event **[open]**.

### The Central Authority
[tentative] An overstretched power that detected the Wake, realized the discovery was too
vast to claim alone, and **issued charters** to independent operators (players) to claim and
hold Gate-worlds in exchange for a **cut/tithe**. It **holds the root of the network** (the
first Gate, or a master relay used to wake everything), which is why it can dispense access.
It **guarantees claims** (no one wipes your Gate-world off the registry while you hold the
charter) and **runs a safe core** (a policed market + new-player spawn/tutorial zone), but its
writ **stops at the frontier edge** — past that line, reach equals exposure is the only law.
Placeholder names: Directorate / Survey / Compact / Commission / Charter Office **[open]**.

### The Gates (the central object)
[decided] Gates are ring/aperture structures; **owning a planet means owning its Gate**, which
is *why* bases are planets rather than an arbitrary rule. [decided] Gates **woke sealed** — the
network came online with every aperture shut, which is the in-world justification for
safe-by-default. [decided] Gates **cannot be manufactured by anyone alive**; they can only be
**found, claimed, and repaired**. Their finiteness is the root cause of all conflict. See the
Gate *system* in Part II for mechanics. Placeholder in-world names for the object: Rings /
Apertures / Wayrings / Conduits **[open]**.

### The Network ("the Lattice")
[tentative] The full web of Gates. Placeholder name **the Lattice** (alternatives: the Old
Roads, the Weave). [tentative] More of the Lattice "waking" over time is one of the two
in-world drivers of content unlocks (the other being rising charter clearance). The network
periodically **self-updates** (Gates sync coordinates with neighbors) — a lore hook that
doubles as a propagating-cyber-weapon vector (see Gate Uses). **[open]:** the network's true
extent, topology, and whether it spans one system, many systems, or galaxies.

### Stable vs. Unstable Wormholes (the cosmology)
[tentative] Gates and Rifts are **two states of one physics**, not two unrelated systems. A
**Gate** is a *stable* wormhole — Builder-engineered, persistent, dial-able, sealable, safe by
default, with two controllable endpoints (you and a dialed target). A **Rift** is an *unstable*
wormhole — spontaneous, uncontrollable, one end opening "somewhere," that **collapses on its own**
after a short life (this self-collapse is the in-world source of a Rift's countdown, not a
bolted-on timer). Rifts tend to tear open **near** Gates, because a stable wormhole marks a spot
where the fabric is already thin and active — so holding a Gate makes you a magnet for Rifts,
concentrating both opportunity and danger on Gate-holders. This unifies the cosmology and feeds
the mystery: the Wake didn't merely switch the network on, it **destabilized** it, so "Rifts are
increasing" reads at once as a difficulty ramp and as the Lattice tearing while something reaches
through. See Rifts and "Rifts → New Gates" in Part II. **[open]:** whether Rifts can be stabilized
into new Gates, and whether players can ever influence where/when a Rift opens or it is pure RNG.

### The Builders (deliberately unknown)
[decided] Who built the Gates, and why, is **unknown to everyone** — the authority, the
players, and (for now) the design. This ignorance is an intentional, ownable choice (more
distinctive and more unsettling than a named precursor pantheon) and is treated as the
long-game mystery engine. **[open]:** literally everything about them, by design — they should
remain unnamed until/unless the mystery payoff requires otherwise.

### Power Cores (the fuel resource, lore framing)
[tentative] Gates run on rare **power cores** that are **scavenged, not manufactured**. Local
Gate jumps sip power; long jumps drain whole cores. Scarcity of cores is a primary economic
driver. (Mechanical framing in Economy / Part II.) Exact nature, rarity curve, and whether
cores are consumable or rechargeable are **[open]**.

### Regions & World Types
These double as the unlock ladder (see Progression). Each is a place-type that can become its
own page.
- **Home planet-base** [decided]: the player's own claimed world on a single Gate; safe when
  sealed; the seat of building, solo PvE, and defense.
- **Small surface worlds** [tentative]: the starting tier; only short-range Gates have woken,
  confining early play to one local cluster. The confinement is a *feature* that explains
  starting scope.
- **Larger / richer worlds** [tentative]: more to build, defend, and take; escalation of stakes.
- **Orbital / space Gates ("space planets")** [tentative]: free-floating Gates with no planet
  beneath them. Crucially, they **cannot be turtled the way a sealed home planet-base can**, so
  they function as always-live PvP zones where lawless action concentrates.
- **Hub worlds** [tentative]: neutral, lawless crossroads (see Hub Worlds in Part II).
- **Megastructure / Supergate sites** [tentative]: rare precursor megastructures that pass
  fleets; server-event scale; the macro-expansion path between systems.
- **The Safe Core** [tentative]: the authority-policed market + spawn/tutorial region.
- **The Frontier** [tentative]: everything past the authority's writ, where exposure rules apply.

### Factions / Organizations
- **The Central Authority** [tentative]: described above; the only firmly-conceived faction.
- **Chartered operators (players)** [decided as a concept]: the player population, holding
  charters. Whether there are formal NPC factions, player alliances as first-class entities,
  or guild systems is **[open]**.
- **Pirates / raiders at hubs** [tentative]: emergent rather than a designed NPC faction;
  whether piracy is purely player-driven or has NPC presence is **[open]**.
- **"Zerg" clans** [tentative]: large organized groups; acknowledged as something the design
  funnels toward hub conflict and away from farming sleeping casuals. Not a formal faction.
- **[open]:** any named in-world factions, their politics, rivalries, leadership, or NPC powers.

### Key Characters
[open] **None established.** No named NPCs, authority figures, rival operators, or quest-givers
exist yet. Do not invent. (If the mystery or onboarding later needs a face for the authority,
that is a future decision.)

### Species & Peoples
[open] **None established.** It is undecided whether players are all one species (e.g. humans),
whether multiple playable or NPC peoples exist, or whether the setting is post-human / alien.
Do not invent.

### Cultures
[open] **None established.**

### Religions
[open] **None established.** (Possible future hook: belief systems around the unknown Builders
or the meaning of the Wake — explicitly *not* yet created.)

### Myths
[open] **None established.** (The Builders and the Wake are obvious future myth-fuel, but no
myths have been written.)

### Languages
[open] **None established.** No conlang, glyph set, or naming conventions decided. (Note: any
Gate "glyph/symbol" set must avoid copying Stargate's chevron/glyph expression — see IP note.)

### Notable Items / Objects
These are objects/items already implied by the design and can each become a page.
- **Power core** [tentative]: scavenged Gate fuel (above); also **portable mask fuel** a raider
  can carry to extend **away reserve** on hostile soil (see Mask sections).
- **Gate control device** [tentative]: the per-Gate console that supplies power, controls
  dialing, and does the targeting math; a discrete, attackable, *stealable* component (the
  "DHD-equivalent," but must be given an original name and expression — **[open]** name).
- **Transponder / access codes** [tentative]: identification a Gate accepts to distinguish
  friendly trade traffic from anonymous raiders; spoofable (infiltration hook).
- **Gate segments** [tentative]: pieces from which megastructure/Supergates are assembled and
  repaired.
- **Beacon** [tentative]: a lightweight, plantable "landing site" near a target that permitted
  players can jump to, distinct from a full Gate (EVE cyno-beacon analog). Also doubles as a
  **small temporary sustaining field**, letting a raider hold a foothold on hostile soil before
  **away reserve** drains (see The Sustaining Field).
- **Coordinate database** [tentative]: the per-homebase log of discovered **coordinates**
  (re-dialable addresses). A first-class, **raidable asset** — breaching a homebase can let an
  attacker steal the map (scouted planets and routes). See Coordinate Discovery.
- **Jammer** [tentative]: a structure that denies Gate-jumping across an area (EVE cyno-jammer
  analog).
- **[open]:** weapons, armor, building materials, consumables, trade goods, artifacts.

### Timeline / History
[tentative] **The Wake = year zero**; gameplay begins moments after, in a land rush "that
started five minutes ago." Before that: an indeterminate **dormancy** of the sealed network,
preceded by the **vanished Builders' era**. [decided] The design wants events to begin *now*
so all players start the rush together. **[open]:** any dated history, prior wars, the
authority's founding, how long dormancy lasted, or what (if anything) happened between the
Builders' disappearance and the Wake.

### The Mystery (cover story vs. truth)
[tentative] **Official story:** the authority found a dormant relay and switched the network
on — routine, profitable, under control. **Hidden truth (players slowly uncover):** the Gates
did *not* wake on a timer or because the authority flipped a switch — **something woke them,
and that something is using the Lattice too.** Three candidate truths, **not yet chosen
[open]:**
1. A signal from *outside* the system — something is coming, and the Gates are how it gets in.
2. The network is a **tripwire** — lighting it told the original owners that someone is home.
3. The authority's "discovery" was a **lie** — it knew, and woke the Gates deliberately for
   undisclosed reasons.
This is the intended late-game escalation and the reason the frontier keeps pushing outward.
[tentative] Mechanically this couples to **Rifts** and the stable/unstable cosmology: the Wake
**destabilized** the Lattice, and rising Rift frequency/rank over the game's life is both the
difficulty ramp and the visible symptom of whichever hidden truth becomes canon.

### IP / Originality Constraint
[decided] The Gate/wormhole *mechanic* is genre-generic and not ownable, but Gaters must avoid
Stargate's specific *expression*: no "Stargate," no Egyptian-mythology skin, no chevron/glyph
set, no copied proper nouns, no ascended-precursor lore, no named dialing device. Serial
numbers off; original names and story throughout. (Stated as a practical design line, not
legal advice.)

---

# PART II — SYSTEMS / MECHANICS

### Core Loop — Moment-to-Moment
[tentative] On your own **planet-base** you explore, gather, and build in a **client-authoritative
solo PvE** sandbox while **sealed** (safe). When you choose to act — trade or raid — you bring
your **Gate** to **port-open** or **gate-open**, accepting risk. Raiding: open a directional
tunnel to a target, push a strike force through, fight at and beyond the aperture under a
**mask energy** constraint, take loot, withdraw. Defending: if someone opens a raid tunnel to
your open Gate, a **siege timer** locks it open for a bounded fight you opted into. Exact
verbs of second-to-second play (movement, shooting, abilities) are **[open]**.

### Core Loop — Session
[tentative] Log in → your stuff is intact (no offline loss, no decay to repair) → choose
whether to stay sealed and build, open a **port** to trade, or open your **Gate** to raid /
visit a **hub world** → resolve contained, finite engagements → log off and reseal. The
explicit goal is "log in when you feel like it" with **no maintenance obligation**.

### Core Loop — Long-Term
[tentative] Grow your planet-base, accumulate power cores and loot, raise **charter clearance**,
and unlock higher **Region/World tiers** (small worlds → larger worlds → orbital/space Gates →
hub/relay Gates → megastructure Gates) as more of the **Lattice** wakes — culminating in
fleet-scale Supergate play and, eventually, the mystery payoff. No persistent base to babysit
across this arc, by design.

### The Gate System
[decided] Each planet-base has a Gate. [decided] Travel is **one-way and directional**: the
*dialing* side opens the tunnel and pays the power, so a raid is inherently the attacker
pushing through a tunnel they opened. [tentative] Momentum is conserved and **weapons fire
passes through** a live Gate (you can shoot up/down an open tunnel — breaching is a firefight
at the aperture, not a loading screen). [tentative] **Bigger aperture = bigger payload = more
power** (the basis of the gate-tier ladder). [tentative] Dialing requires **knowing the
target's coordinates** (coordinates are intel: discoverable, tradeable, stealable, hideable — a
planet whose coordinates nobody knows is effectively hidden; see Coordinate Discovery). Term
note: **coordinates** is the standardized term for what earlier drafts called the "address."
Specific dialing UX is **[open]**.

### Gate States: sealed / port-open / gate-open
[tentative] Exposure is **tiered, not binary**:
- **Sealed** [tentative]: safe, isolated, stagnant. Incoming matter cannot reintegrate; the
  aperture is shut. Communication can still pass (see Comms), but no goods, energy, or people
  transit.
- **Port-open** [tentative]: can trade; pirates can hit your **cargo/convoys** but **cannot
  breach your vault/home**. Trading therefore risks goods, never your whole civilization.
- **Gate-open** [tentative]: can launch raids and is **fully breachable**.
Each step out buys more reach at the cost of more risk. The three-tier model is the agreed
shape; exact thresholds and naming are **[tentative]**.

### Presence Requirement
[decided] A Gate can only be **open while the owner is online and choosing it**; logging off
normally **seals** it. This is the mechanic that removes offline raiding and the babysitting
tax. **[open]:** exact rules for disconnects, AFK, and grace windows.

### The Siege Timer
[tentative] Once a raid is initiated against an **open** Gate, a **siege timer** **locks it
open** for a bounded window so the defender cannot instantly slam the door (offline-dodge
fix), but the fight still ends. Current proposed window **20–30 minutes [tentative]**, with a
lore-justified hard ceiling around **~38 minutes [tentative]** (the in-world max wormhole
duration). **Conflict:** the 20–30 figure and the ~38 ceiling need reconciling to one number,
and that number must also serve target session length — see Conflicts.

### Directional Bilateral Tunnels (anti-zerg)
[tentative] Opening a Gate is **not** shields-down to the whole galaxy; it is a **jump tunnel
to one specific planet**. Raiding Planet A opens a **two-way** tunnel between you and A (A can
counter-attack through it), but **third parties cannot pile in** unless they also open their
own Gates to you. Each raid is a **duel/feud**, not a free-for-all. Trade routes work the same
way: two planets mutually open to each other, and that single link is the only vulnerable
surface.

### The Four Design Traps (and their solutions)
A consolidated, page-worthy set. Each trap is a failure mode the exposure model could fall into.
- **Turtle equilibrium** [decided problem]: if sealed = safe forever with no downside, everyone
  bunkers and the game dies. **Solution [tentative]:** the **economy forces exposure** — a
  sealed planet-base stagnates (finite stored resources, no growth, no tech progress); growth
  requires imports, imports require open routes, so ambition itself creates targets.
- **Trade-suicide** [decided problem]: if trading exposes your core like raiding does, every
  economic act invites a wipe. **Solution [tentative]:** the **tiered** sealed/port-open/gate-open
  model — trading at **port-open** only risks goods, not the vault.
- **Offline-dodge exploit** [decided problem]: if you can instantly seal mid-raid (or alt-F4),
  raiding is impossible; if you can't close, you're trapped online. **Solution [tentative]:**
  **presence requirement + committed siege timer** — opt-in, synchronous, finite, and you
  cannot be jumped while offline.
- **Zerg pile-on** [decided problem]: if opening exposes you to everyone, a dogpile returns
  power to whoever has the most bodies. **Solution [tentative]:** **directional bilateral
  tunnels** — raids are contained duels/feuds.

### Mask Energy & Survival
[decided] **mask energy** is the survival/life-support layer, and the **Gate is its energy
source**: the player wears a life-support **mask** powered by a field drawn from the Gate (framed
as "magnetic"/projected energy — exact physics **[open]**). This creates a **natural raider timer**
(a raider away from a sustaining field is on a depleting budget and must be efficient) and an
**asymmetric home-soil advantage** (inside your own field you are topped up and strong; deep in
enemy territory you are on a clock). It replaces the ARK/Rust survival grind — tied to the core
Gate fantasy rather than a hunger/thirst chore. **Crucially, mask energy must be split into two
independent numbers** (see next section) or world-expansion will erode raids. **[open] (do not
invent specifics):** what the mask physically is, exact drain curve, recharge rules.

### The Sustaining Field (soft world border)
[tentative] Each active Gate projects a **sustaining field**. Inside it the mask tops up, giving
effectively unlimited time on your own soil. Moving outward, the field **weakens on a gradient**, so
the mask drains faster the farther you go. This is the game's **soft world border**: not a wall at
radius X, but a **cost curve** / risk gradient, so the dangerous fringe becomes a *place*, not an
edge. The fringe is exactly where **Rifts** naturally belong ("grab the loot and get back before the
mask dies"). It replaces a hard map boundary. **Dev/lore lever:** field radius is the
**authority-tunable expansion knob** — the studio grows the playable world over time by having the
authority "expand the field" (see Authority as Patch Channel). **Technical fit:** a field bubble per
*active* Gate matches the lazy-load, cost-scales-with-online-players architecture — only the area
around online Gates needs simulating, so the soft border and the cheap-server design are the same
line. **[open]:** gradient vs. hard radius (leaning gradient); whether field radius is purely
authority-set or also a capped per-player upgrade.

### Mask: Field Radius vs. Away Reserve (the two-number split) — CRITICAL
[tentative, load-bearing] Mask energy governs two things that pull in opposite directions, and they
**must be separate numbers**:
- **Field radius** — how far from your Gate you can roam/build; the soft border; the
  **dev-expandable** lever.
- **Away reserve** — how long the mask lasts once you leave a sustaining field (i.e. when raiding);
  the **raider timer**.
If these are the *same* stat, every "expand the field 10%" patch also lets raiders camp enemy soil
10% longer, eroding raid tension with every content update. Keeping them separate lets the map
expand for years **without touching the raid clock**. Raiders extend **away reserve** by carrying
**power cores** as portable mask fuel and/or planting a **beacon** as a small temporary field to
hold a foothold (both already in the item list).

### Mask-at-Zero Outcome (asymmetric by location)
[tentative] What happens when the mask empties is **asymmetric**, which solves two problems at once:
- **On your own soil / inside a field:** *soft* failure — emergency recall to the Gate, no loss. A
  leash, not a punishment (preserves the anti-decay thesis).
- **In hostile territory during a raid:** *hard* failure — you go down, vulnerable,
  finishable/lootable. The real risk that stops raiding from being a free teleport home.
Alternative considered: uniform death everywhere (simpler, but closer to the ARK feeling being
designed out). Asymmetric preferred. **[open]:** confirm; define the recall and downed states.

### Other Survival Meters
[open] **Undecided.** Whether Gaters has hunger, thirst, temperature, stamina, or health-regen
systems beyond **mask energy** is not established. The anti-"chore" intent suggests minimal
survival nagging, but nothing is decided.

### Building System
[tentative] Building on your **planet-base** is assumed to exist (building was a "loved" pillar
from ARK/Valheim) and happens in the safe **sealed** state. **Crucially, there is no persistent
base decay/upkeep [decided]** — that is the central thing being designed out. **[open]:**
build system depth, materials, structure types, whether defenses are buildable, grid vs.
free-form, and whether anything analogous to taming exists.

### Combat System
[tentative] "Real PvP combat" is a required ingredient of the first playable. Two combat
contexts are implied:
- **Personal/infantry combat** [tentative]: ground raids through standard Gates (strike teams,
  breaching, looting).
- **Fleet/ship combat** [tentative]: space-Gate raids, framed as a **two-phase** structure —
  **fleet raids on orbital control**, then **infantry raids on the base** — slated as a later
  expansion.
**[open]:** perspective (FPS / third-person), whether combat is gun-based, melee, ability-based,
or vehicular; TTK; gear/power scaling; and how defender vs. attacker advantage is tuned at the
aperture.

### Trade System
[tentative] Trade happens at **port-open**, risking **cargo/convoys** but not the vault. Distant
trade can be routed cheaply through **hub worlds** (paying a toll and accepting exposure) or
**dialed direct** (expensive, private). **Access lists** can permit specific partners; tolls
and the authority **tithe** are economic sinks. **[open]:** what is actually traded (goods,
resource types, currency), pricing/market mechanics, contracts, and whether trade is
player-to-player only or includes NPC markets in the safe core.

### Raiding System — Two Distinct Modes
[tentative] The design keeps **two raiding modes cleanly separate**:
- **Home raid** [tentative]: **direct Gate, bilateral feud** — contained, opt-in, two-way,
  governed by presence + siege timer. The babysitting fix and anti-zerg rule hold here.
- **Hub raid / hub warzone** [tentative]: **opt-in, chaotic, many-vs-many** — you choose to
  walk into it.
**Guardrail [decided as a principle]:** a hub may lower your *travel cost* to a target's
doorstep but must **never** lower the *target's defenses*. The moment a hub lets you punch into
a **sealed** home, the design has "rebuilt ARK." The destination always obeys
presence + siege timer.

### Hub Worlds
[tentative] Neutral, **lawless crossroads** that serve a **dual purpose**: **raiding staging
grounds** and **trade routing nodes** for reaching distant partners affordably. You **cannot
turtle** at a hub; PvP is always live, so action concentrates there by design — the players who
want endless PvP go fight at the hub instead of farming sleeping casuals. **Optionally
capturable [tentative]:** hold the relay/core and you can **tax** traffic, **throttle** (allies
cheap, enemies expensive or gate-locked), and gain **intel** on who moves through. A hub is
therefore a market *and* a chokepoint — the territorial prize big clans fight over.
**Acknowledged tension:** the hub deliberately *reintroduces* the zerg pile-on within itself;
that is accepted as the place for it, but hub balance is unsolved (see Conflicts).

### Rifts (spontaneous events — the dopamine engine)
[tentative] **Rifts** are the *unstable* half of the cosmology: spontaneous wormholes that open on
their own, can't be controlled, and **collapse on a countdown**. Design intent (inspired by Solo
Leveling's gates) is **opportunity, not invasion** — and this is the line that must not bend: a Rift
opens **next to** your Gate, as a *separate* hole in your surroundings, **never through your sealed
Gate and never as a backdoor for enemy players into a sealed home.** A Rift opens onto **content**
(a PvE dungeon-pocket, a derelict, a rich anomaly, a monster spill) that you *choose* to enter;
ignoring it costs nothing but the loot. Each Rift telegraphs a **rank + countdown** ("Rank-5 Rift
stabilizing, 18:42" — the countdown is the instability decaying). Random rank + scaling loot + time
limit = variable-ratio reward and anticipation (the "what do I get this time" pull); a rare top-rank
Rift is a server-wide event. **Healthy-vs-toxic line (the project's own thesis):** Rifts must make
players *excited to log in and see what's open*, never *obligated to log in or lose something*. The
moment an uncleared Rift punishes an offline player, it has reinvented decay. Two flavors, both
opt-in:
- **Solo Rift (PvE)** [tentative]: opens on/near your planet; cleared alone; **away reserve is the
  difficulty leash** (clear it before life-support drains). The everyday loop, and the answer to
  "what do I actually *do* while sealed and building?"
- **Open Rift (opt-in PvP)** [tentative]: a high-value Rift visible to several players —
  effectively a **procedurally-spawned, temporary hub world**. Fighting happens **at the Rift, over
  the loot**, not at anyone's home. Delivers the "a level-5 gate is locking in, others incoming"
  tension *without* breaking the home rule.
**Optional downside for ignoring a big Rift** [open]: a **PvE incursion** — monsters spill onto your
surface and you fight them — **never** an auto-opened door for raiders, and **only while you are
present** (same presence rule), so logging off can never cost your base. Name: **Rift** for the
unstable hole, kept distinct from **Gate** (alt: "Conjunction," fitting the "connection made"
phrasing). **[open]:** rank scale (E–S vs. 1–10), surface vs. orbit vs. both, the ignore-it
downside, and how Rift loot relates to raid loot so neither trivializes the other.

### Rifts → New Gates (finite but replenishing)
[tentative, resolves a flagged conflict] If an unstable **Rift** can be **stabilized**, that is
where new Gates come from: you still never *manufacture* a Gate, you **tame** a naturally-occurring
unstable wormhole into a permanent one. This reconciles "Gates are finite and unbuildable" with the
need for more Gates as the playerbase grows — **finite, but slowly replenishing, born from Rifts.**
**New sub-tension to resolve:** stabilization is *player-driven* expansion, which rubs against
*authority-controlled* expansion and Authority-as-Patch-Channel. Reconciliation options: gate
stabilization behind **authority tech / a license** (new Gates appear on the studio's schedule,
framed as the Directorate learning to stabilize the network), or simply keep stabilization **rare
and hard**. Needs a call (see Conflicts).

### Coordinate Discovery & the Coordinate Database
[tentative] The concrete form of "coordinates are intel." **Coordinates are information, not
Gates.** You never build a new Gate; you **dial from the Gate you already own**, and what you save
is the **coordinate** — a re-dialable address logged in your homebase **coordinate database**.
"Locking into a planet to revisit later" means **re-dialing a saved bookmark**, not constructing a
second gate (so the finite/unbuildable rule holds). **Guardrail:** a bookmark removes the *discovery*
cost, never the *travel* cost — re-dialing a known coordinate still burns fuel scaled by distance,
keeping the hub/distance economy intact. **The loop:** dial out or send a probe → reach a planet →
its coordinates log to your DB → some planets hold resources beyond your current tech, so the
bookmark is a **deferred target** → later, with the tech or tier, return to **claim** it (if still
empty) or extract what you couldn't before. Payoffs:
- **Discovery feeds PvP for free** [tentative]: a rich planet found early won't stay empty — either
  you claim it later or someone else does, turning your old bookmark into a **scouted raid target**
  you mapped before anyone lived there. Early exploration becomes a late-game hit list (rides the
  three-state model: bookmarked-empty = claim opportunity; bookmarked-occupied = raid).
- **The coordinate DB is raidable** [tentative]: breaching a homebase can let an attacker **steal
  the map** — scouted planets and routes — loot beyond materials, and a reason to protect what
  you've charted.
- **Blind exploration-dialing as a slot machine** [tentative]: re-dialing *known* coordinates is
  precise, but dialing into the *unknown* for a fuel cost yields a **random planet of random
  richness and danger** — the variable-ratio hook applied to exploration, and a natural fit for the
  instability cosmology (dialing blind into a half-formed connection).
**[open]:** whether discovery is travel-only or also via probes / buying / stealing; whether blind
exploration-dialing exists (leaning yes); whether the coordinate DB is stealable on a raid (leaning
yes).

### Authority as Patch Channel (a principle worth locking)
[tentative → decide] The **central authority is the in-world voice for developer changes.** Field
expansions, new world tiers, new world types, even buffs and nerfs ship as **"Directorate
bulletins"**, so patch notes become lore. The world literally grows over the game's life (the same
unlock ladder) with a **diegetic reason**, and a balance change never has to read as a balance
change — it is always the authority adjusting the network. "Field harmonics improved 10%" is a
patch; "we don't know why the Rifts are increasing" is the plot. Worth locking early because it
shapes how every future update is written. (Flagged tentative only because it has not been formally
signed off; it is a strong leaning.)

### Gate Uses Catalogue (mechanic option space)
A research-derived menu of things Gates can *do*, framed as design options. The five tagged
"sharpest" below are the current leaning for inclusion **[tentative]**; the rest are catalogued
**[open]** options not yet integrated. Each could be its own page.

**Sharpest / leaning-in [tentative]:**
- **No caller ID + transponder codes**: an incoming raid does not reveal *who* it is until it
  commits; friendly trade requires an accepted code; spoofing codes is an infiltration play.
  The cleanest way to separate "open for business" from "open to attack."
- **Occupy-to-lock / jamming**: holding a Gate open (or keeping a line busy) can lock a target
  out of the network or refuse connections — a denial/siege tactic that doesn't touch the
  safe-by-default home rule.
- **Buffer wipe of in-transit forces**: troops "in transit" sit in a vulnerable buffer; cutting
  the connection mid-raid can wipe an in-flight strike force — a genuine raid-commitment
  mechanic.
- **Stealable Gate control device**: damage or steal a planet's control console and it can
  receive but barely dial out — a "stranded, raidable, can't retaliate" consequence state that
  is *not* permanent base loss.
- **Gate-as-bomb (overload)**: overloading a Gate yields a planet-scale explosion — a rare,
  costly scorched-earth / siege-ender, server-event tier.

**Catalogued, not yet integrated [open]:**
- **Unstable-vortex / aperture burst**: activation can disintegrate whatever is stacked at the
  aperture — a defensive anti-pile trap.
- **Dial-into-a-star**: route a tunnel through a sun to sabotage a target system — an exotic
  super-weapon gated behind disabling safeties.
- **Safeties as a tech resource**: the Builders' safety protocols refuse dangerous jumps;
  researching/disabling them unlocks weapon-grade uses (risk/reward; manual dial bypasses
  safeties).
- **Comms through a sealed Gate**: radio/data pass even when the aperture is shut — diplomacy,
  threats, ransom, alliance pings without dropping exposure.
- **Subspace relay / data network**: Gates carry data; controlling Gates controls information.
- **Recon probes**: send an unmanned probe through to scout before committing a raid.
- **Gate bridges (chained call-forwarding)**: chains of Gates forward travelers hop-to-hop for
  far less power than one long jump — the in-world basis for the cheap-distance **hub**.
- **Harvested / relocatable Gates**: found (often orbital) Gates can be claimed and moved to
  build new routes (see Conflict with "Gates are unbuildable").
- **Reprogram-the-route**: whoever controls a relay/hub can reroute, misdirect, or trap traffic.
- **Network self-update as a worm vector**: the auto-sync between neighbor Gates can propagate a
  cyber-weapon across the Lattice.
- **Proximity priority conflicts**: placing a competing Gate near a rival's can override/suppress
  theirs — territorial jamming by proximity.
- **Time/exotic physics**: solar-flare time travel; black-hole time dilation bleeding through an
  un-severable connection; the ~38-minute wormhole cap (already borrowed as the siege ceiling).
- **EVE-proven economy/access layer**: access lists (incl. asymmetric one-way), tolls, fuel
  scaling with mass × distance, a **hard mass cap** that forces the biggest fleets onto rare
  Supergates, plantable **beacons** as landing sites, system-wide **jammers** for area denial,
  and **Gates being killable / needing defense**.

### Progression & Tech
[tentative] Two in-world drivers gate the same tier ladder: **rising charter clearance** (you
prove yourself) and **more of the Lattice waking**. Unlock ladder: small surface worlds →
larger/richer worlds → orbital/space Gates → relay/hub Gates → megastructure/Supergates.
[tentative] **Gate tiers** as an upgrade path: **Standard** (strike team / cargo) → **Heavy**
(vehicles, light armor, bulk) → **Supergate** (fleets, capital ships, siege; megastructure,
impossible to hide, drains a full core). [tentative] A tech path around **Gate safeties**
unlocks weapon-grade uses. [decided] **No base decay** anywhere in progression. **[open]:** the
actual tech tree, research mechanics, character/skill progression, and gear tiers.

### Economy
[tentative] Drivers and sinks:
- **Stagnation pressure** [tentative]: sealed planet-bases don't grow; growth needs imports —
  the engine that makes players open up. (See the critical tension in Conflicts: too much
  pressure recreates an obligation.)
- **Power cores** [tentative]: scarce, scavenged Gate fuel; the primary consumable behind all
  Gate activation.
- **Activation cost** [tentative]: proposed rule **activation cost = gate tier × distance band**.
  Distance bands: **local** (a trickle / power cell) → **regional** (partial core) → **cross-map**
  (a full, possibly unrecoverable core). A Supergate across the map is intended to be the single
  most expensive act in the game.
- **Direct-dial vs. hub routing** [tentative]: direct = high fuel, private, no third-party
  exposure; hub = low fuel, plus a toll, plus exposure in a live PvP crossroads.
- **Tolls** [tentative]: hub controllers tax traffic.
- **Authority tithe** [tentative]: the cut owed for your charter — a baseline sink.
- **Loot** [decided as a pillar]: raiding for goods is a core reward.
- **Fuel scales with mass × distance + hard mass cap** [tentative, EVE-inspired].
**[open]:** concrete currencies, resource taxonomy, crafting inputs, sink/faucet balance, and
whether there's a unified currency or barter.

### Decided / Proposed Formulas & Numbers (consolidated)
- **activation cost = gate tier × distance band** — [tentative] (rule stated; values **[open]**).
- **Distance bands**: local / regional / cross-map ≈ power cell / partial core / full core —
  [tentative].
- **Gate tiers & payloads**: Standard = strike team + cargo; Heavy = vehicles + light armor +
  bulk; Supergate = fleets + capital ships + siege — [tentative].
- **Siege timer**: 20–30 min proposed, ~38 min lore ceiling — [tentative] (**must reconcile to
  one number**; see Conflicts).
- **Mass cap on convenience Gates** forcing big fleets onto Supergates — [tentative].
- Everything else numeric (mask-energy drain rates, prices, TTK, gather rates) — **[open]**.

### Multiplayer / Networking Architecture
[decided] **Authority model is split by context:** **server-authoritative only during contested
raids/trades**; **client-authoritative simulation for solo PvE** on home planet-bases.
[decided] **Three-state planet model:** **empty** (just a database row) → **solo-occupied**
(client-authoritative) → **contested** (a server-authoritative instance spun up). [decided]
**Seed-plus-deltas storage:** planets are **lazy-loaded on demand**, so **server cost is
proportional to online players**, not to world size. [decided] **Gate-based instancing
dramatically reduces infrastructure cost** vs. a persistent shared world — treated as a
foundational architectural advantage that makes the game viable solo. **[open]:** anti-cheat
strategy for the client-authoritative solo state (see Conflicts), matchmaking/handoff details,
and how bilateral tunnels are instanced.

### Tech Stack
[decided] **Unity with C#** (matches the designer's existing language comfort). [decided]
**Native-first Unity build, with a web export as a demo/playtest funnel.** [decided] A
**`PlanetGenerator` abstraction from day one** so procedural generation can be swapped in later
as a single-class change. [decided] The **Gate mechanic is the mask-energy source** (engine-level
tie between Gate energy, survivable range, the raider timer, and home-soil advantage). **[open]:**
netcode library/transport, hosting model, persistence backend specifics.

### Aesthetic / Art Direction
[tentative] Touchstones: **Minecraft**, **Valheim**, **No Man's Sky**. **NMS is the
*aspirational* visual target**; the Gate structure deliberately **sidesteps NMS's hardest
engineering problem** (seamless space-to-surface flight is replaced by **Gate loads**).
**Valheim** represents the *achievable* Unity aesthetic. [decided as a principle] Distinguish
**visual style (cheap, achievable solo)** from **engine tech of reference games (NMS's custom
engine and seamless flight — not achievable solo).** [tentative] Practical path to the NMS look
solo: **low-poly, flat-shaded 3D with strong post-processing.** [decided] **Art direction is
deferred until after greybox validation.** **[open]:** the final art identity (NMS-lush vs.
low-poly-stylized), palette, UI style.

### Validation Plan (greybox-before-art)
[decided] The biggest risk is **not technical** — it is whether **opt-in, presence-gated raiding
is actually fun**, i.e. **will players actually open their Gates?** Plan: build a **greybox proof
of concept** before any art. [tentative] **Minimum viable slice:** sealed/open states, a
bilateral raid tunnel, loot worth taking, economic pressure against permanent sealing, and real
PvP combat. [tentative] **Ground Gates only** for the initial concept proof; **space Gates**
(the two-phase fleet-then-infantry structure) come later. [decided as a principle] **Design for
success enabling expansion, not requiring it** — a working small version should be a complete
thing, not a broken large one.

---

# CONFLICTS / TENSIONS TO RESOLVE
Flagged rather than smoothed.

1. **Raid-clock governance — siege timer vs. away reserve.** The **siege timer** bounds the raid
   from the *defender* side (locks their Gate open 20–30 min); the mask's **away reserve** bounds it
   from the *attacker* side (life-support leash away from a sustaining field). The two-number split
   (Field Radius vs. Away Reserve) settles that **away reserve**, not field radius, is the raider
   timer — but the relationship between **away reserve** and the **siege timer** is still
   unresolved: same clock or two, which actually ends a raid, and can they contradict (attacker's
   reserve empties before the siege timer, or vice versa)? Note raiders can extend away reserve with
   **power cores**/**beacons**, so the attacker clock is partly player-controlled.
2. **Siege-timer number.** 20–30 min (design) vs. ~38 min (lore ceiling) vs. target session
   length — needs to collapse to one defended value.
3. **"Gates are unbuildable" vs. getting more Gates over time.** Reconcile **manufacturing** a Gate
   (forbidden) with the several ways the design now adds reach: **relocating found Gates /
   reassembling megastructures from found segments**, **stabilizing Rifts into new Gates**
   (finite-but-replenishing), and **saving coordinates** (re-dialable bookmarks, which are
   *information, not new Gates* — this one is already resolved). State the umbrella rule: you never
   fabricate a Gate from nothing; you find, relocate, reassemble, or tame one, and you re-dial saved
   coordinates. **Open sub-tension:** Rift-stabilization is *player-driven* expansion vs. the
   *authority-controlled* expansion implied by Authority-as-Patch-Channel — see conflict 11.
4. **Client-authoritative solo PvE vs. cheat-resistance.** If a planet-base is client-authoritative
   while solo, a player could doctor their world/inventory/defenses client-side *before* a raid
   lands and the state hands off to server-authoritative. The handoff is an exploit surface with
   no decided mitigation.
5. **Economic stagnation pressure vs. the "no obligation / log in when you want" promise.** This
   is the project's central balancing act: stagnation must be strong enough to push players to
   open up, but if it's too strong it becomes a *soft upkeep tax* — recreating the very obligation
   the game exists to remove. Where is the line?
6. **Raider anonymity ("no caller ID") vs. the central registry / claim guarantee.** The authority
   knows who holds what and guarantees claims; raids are supposed to be anonymous until committed.
   Does the registry leak attacker identity, and how do these coexist?
7. **Hub zerg problem.** Hubs intentionally concentrate many-vs-many chaos, but that means the
   zerg/pile-on dynamic is alive and **unsolved inside the hub**. Is unbalanced hub PvP acceptable,
   or does it need its own structure?
8. **"Sealed = isolated/stagnant" vs. "comms pass through a sealed Gate."** Communication is meant
   to pass while sealed, but the economy treats sealed as cut off. Confirm the intended split
   (information yes; goods/energy/people no) so "isolated" isn't misread as total silence.
9. **NMS-aspirational visuals vs. low-poly-achievable-solo.** Two different target identities are
   both cited; the actual look is deferred and undecided, which leaves scope/feasibility ambiguous.
10. **Title "Gaters" — phonetics & searchability.** Reads as "gators"; homophones "gay-ters" /
    "gaiters"; SEO/searchability and community-harassment risks were raised and not resolved.
11. **Player-driven Rift-stabilization vs. authority-controlled (dev-paced) expansion.** Letting
    players stabilize Rifts into new Gates is satisfying but hands world-growth pacing to players,
    which conflicts with using the authority as the studio's patch/expansion channel. Decide:
    license/tech-gate stabilization (studio keeps the schedule) or accept player-paced Gate supply.
12. **Field radius and away reserve must stay decoupled.** The whole point of the two-number split:
    if a future "expand the field" patch ever also lengthens away reserve, world-expansion silently
    nerfs raid tension. A standing implementation rule, easy to violate by accident.

---

# BIGGEST OPEN DESIGN QUESTIONS
1. **Is the core fun real?** Will players actually open their Gates — i.e. does opt-in,
   presence-gated raiding produce the aggressor thrill without the defender tax? (The one
   greybox must answer.)
2. **What governs the raid clock** — siege timer, the mask's away reserve, or both — and how do
   they relate? (Away reserve is now the attacker-side timer; its link to the siege timer is open.)
3. **How hard should economic stagnation push** without becoming a disguised upkeep obligation?
4. **Which mystery truth** (outside signal / tripwire / authority lie) is canon?
5. **What is the combat model** (perspective, gun/melee/ability/vehicle, TTK, aperture
   advantage)?
6. **How is the client-authoritative solo planet protected** from pre-raid tampering at handoff?
7. **What is the final art identity** (NMS-lush vs. low-poly-stylized)?
8. **Are there survival meters beyond mask energy** — and how minimal should survival be?
9. **How do raider anonymity and a central claim-registry coexist?**
10. **Does the title "Gaters" survive** the phonetic/searchability/harassment concerns, and what
    is the in-world player term?
11. **Can Rifts be stabilized into Gates** — and is that player-driven or authority/tech-gated?
12. **Rift specifics:** rank scale (E–S vs. 1–10), spawn location (surface / orbit / both), the
    ignore-it downside (missable loot vs. PvE incursion), and Rift-loot vs. raid-loot balance.
13. **Mask/field specifics:** gradient vs. hard radius (leaning gradient); field radius as
    authority-only or a capped per-player upgrade; confirm the **asymmetric mask-at-zero** outcome.
14. **Lock "Authority as Patch Channel" as canon?** (Strong leaning; needs formal sign-off.)
