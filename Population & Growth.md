---
title: Population & Growth
tags: index-linked
---

## Simplified model #decided

After weighing a multi-group-per-tile simulation against loop design, settled on the simpler version:

- **One population number per tile.**
- **One loyalty meter per tile**, pointing at a collective.
- No per-tile multi-group mixing, no integration curves, no origin-tag tracking of sub-populations.

Reasoning: the richer model (growth per tile, newborns inheriting local group mix proportionally, slow
integration meters) added simulation cost and had no clear player-facing decision attached to it — see
rejected version below. A game loop needs a decision the player can make on a timescale they can act on.

## Rejected: multi-group model #open

Earlier direction, kept here for reference in case a v2 wants more depth:

- Growth tied to tile (food surplus, housing, stability), not to the player/collective in a vacuum.
- A tile with mixed control produces new pops in proportion to the existing local mix.
- Integration between groups sharing a tile as a slow meter, rate set by policy (assimilation / autonomy /
  segregation).
- Each group keeps its own skills/loyalties/grievances.

Cut primarily because: pop-level behavior (e.g. minorities fleeing a border) removes player agency rather than
creating a decision, and the added state is expensive to tick hourly across many tiles.

## Loyalty as the active lever #decided (direction)

Loyalty is the number players actually manage: policies, garrisons, propaganda, and public works push it up or
down, acted on during the daily cadence. Loyalty crossing a threshold is what triggers a [[Splits & Secession|
split]] event.

## Open: pop attributes #open

Do pops carry only an origin tag, or real attributes like skills and loyalty? Leaning toward "just loyalty,
per tile" given the simplification above, but not fully closed.
