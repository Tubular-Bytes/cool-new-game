---
title: Territory & Logistics
tags: index-linked
---

## World shape #decided

World is formed from **planets + tiles** (not a single flat map).

## Claiming tiles #decided (direction)

- Free/unoccupied tiles: claimed by spending some resource.
- Occupied tiles: claimed via diplomacy or war.

## Interplanetary expansion #decided (direction), #open (exact curve)

- Advanced players can attempt to control tiles on other planets.
- Doing so puts an **exponentially growing strain** on:
  - Economy — moving materials/goods between planets vs. locally.
  - Military — moving/supplying units across planets vs. locally.
- This is meant to be a natural soft cap on empire size, rather than a hard rule against expansion.

## Legibility requirement #decided (principle)

The exponential strain curve needs to be **visible to players before they overextend**, not a hidden
multiplier discovered after the fact. Direction: surface something like a "logistics strain: 340%, efficiency
loss on transfers" number, so overreach is a legible choice rather than a trap.

Not yet designed: the actual formula/curve, or the exact UI for surfacing it.

## Relationship to other systems

- Feeds into [[Market]] — whether the market is global or regionalized should be decided consistently with
  this system (a regionalized market ties trade into the same distance/strain logic; a global market floats
  above it).
- Capitals are exempt from the [[Splits & Secession|split]] claim process entirely — can only change hands via
  declared war.
