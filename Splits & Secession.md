---
title: Splits & Secession
tags: index-linked
---

## Design principle #decided

A split should never resolve as something a player watches happen to them with no choice attached (e.g. the
originally-considered "fleeing pops" migration mechanic was cut for exactly this reason). Every mechanic here
should map to a decision, on a timescale the player can act on.

## Two-tier structure #decided

### Tier 1 — Clean secession (a right, no consent needed)

- The splitting side may take only tiles where **their own loyalty is overwhelming**.
- Cheap, cannot be blocked or refused by the parent collective.
- In taking this option, the splitter **gives up any claim on the shared/contested pool**.
- The parent's only counter-play is to have shored up loyalty *before* this point (see
  [[Population & Growth]]).

### Tier 2 — Negotiated split (for anything beyond overwhelming-loyalty tiles)

- Covers mixed-loyalty land and shared assets (stockpiles, fleets, buildings).
- Requires the claim + negotiation process below.
- Splitter gets access to more, but has to bargain and pay for it.

There is no "refusal" mechanic as such — the parent can't block a split outright, only contest what goes
beyond the splitter's own overwhelming-loyalty ground.

## Claims #decided (direction), #open (exact formula)

- Each side gets a **claim budget**, not an unbounded self-declared "share." Budget should reflect
  contribution: founding stake, pops held, loyalty.
- Tile cost against that budget is a function of concrete factors: **resource value of the tile**, **distance
  from capital**, etc.
- **Capitals cannot be claimed** through this process at all — only through a declared war.
- Claims should be **hidden until a cutoff**, then revealed simultaneously. This prevents each side tuning
  their claim against the other's declared amount, and makes out-of-game coordination actually matter (it's
  the only reliable way to avoid overlap/war).

Not yet fully designed: the exact budget formula, and how founding stake/pop count/loyalty are weighted
against each other.

## Negotiation window #decided

- Not a fixed number of cycles. It's a **standing proposal**: if both sides' hidden claims are compatible at a
  cutoff, it resolves immediately.
- If incompatible, either side can choose **"keep talking"** (extend) or **"resolve now"** (force resolution
  with current claims). Calling "resolve now" early is itself a real bet that your claims are good enough.
- A hard cap on total extension (e.g. three daily cycles) prevents indefinite stalling.

Rationale: shouldn't force multiple negotiation turns if players can agree in one, and shouldn't force a
single-turn resolution if players genuinely need to work it out.

## Escalation threshold #decided (direction), #open (exact %)

- Below some contested-tile percentage threshold: unresolved overlap goes to **fallback allocation** (see
  below) — no war.
- Above the threshold: escalates into **open conflict**, resolved via the hourly combat layer, scoped only to
  the contested tiles (not a full civil war), since the rest of the split is already settled.
- Exact percentage not yet set.

## Fallback allocation (no war, below threshold) #decided

Explicitly rejected pure randomness — losing a capital-adjacent or otherwise valuable tile to a coin flip
was judged to feel bad and undermine trust in the system. Settled on a deterministic rule instead:

1. Claim budgets reflect contribution (founding stake, pops, loyalty) — see Claims above.
2. Contested tiles are awarded to whichever side has **higher local loyalty** on that specific tile — most
   defensible/legible principle.
3. True ties go to an **alternating draft** (smaller side picks first) until budgets are exhausted.

No dice anywhere in the fallback path — players should be able to predict the outcome given the visible
inputs (loyalty, budgets).

## Cost to declare #open

Without some cost or cooldown on declaring a split, large collectives could fragment constantly, which would
undercut the political themes the game is trying to explore. Direction agreed (there should be safeguards and
an associated cost, considering tile resource value, distance from capital, etc. — same inputs as the claim
budget) but the specific cost/cooldown mechanism is not designed yet.

## Explicitly open questions

- Can the losing side of a loyalty-based fallback allocation escalate to conflict anyway, or is escalation
  only available for over-threshold overlap? (See [[Open Questions]].)
- Exact escalation-threshold percentage.
- Exact claim budget formula and weighting.
- Exact cost/cooldown to declare a split.
