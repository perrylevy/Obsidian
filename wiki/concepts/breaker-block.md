---
type: concept
aliases: [Breaker Block, BB]
tags: [concept, pd-array, order-flow]
---

# Breaker Block

A breaker block is a prior order-block-like structure that has been violated and then reused in the opposite direction as a continuation or retest reference. In the current wiki, it sits between strict OB logic and broader PD-array reuse logic ([[concepts/order-block]], [[concepts/pd-array]], [[sources/internal-external-liquidity]] @ 14:23, @ 14:38, [[sources/2025-lecture-series-nq-review-may-29-2025]] @ 9:35).

## Core idea

The practical logic is:
- a directional structure forms,
- price later trades through it,
- and once violated, that level can flip role and act as a new reference in the opposite direction ([[concepts/order-block]], [[concepts/fair-value-gap]], [[sources/2024-04-18-ob-tape-reading]] @ 2:03:51, @ 2:08:29, [[sources/internal-external-liquidity]] @ 14:23, @ 14:38).

## Why it matters

Breaker blocks matter because they give the trader a way to think about failed support/resistance as a reusable delivery reference rather than a dead level. They fit naturally inside the PD-array matrix and often appear near discount / premium transitions or after a liquidity raid ([[concepts/pd-array]], [[concepts/discount-premium]], [[concepts/liquidity-sweep]]).

## Relationship to order blocks

This wiki treats breaker-block usage as adjacent to OB logic rather than identical to it:
- an OB is the origin structure that sets delivery in motion,
- a breaker block is the later reuse of a violated structure after the market has changed state.

That makes breaker-block logic especially useful after a sweep or after a clean failure of an old OB-level reference ([[concepts/order-block]], [[concepts/change-in-state-of-delivery]]).

## Practical usage

Use breaker-block thinking when:
- an obvious prior support/resistance zone has already failed,
- you want to know whether the market is retesting the broken level for continuation,
- or the broken zone aligns with FVG / discount / liquidity confluence.

The continuation-breaker clip adds a more tactical rule: wait for the sweep, wait for the close through the level, then let the breaker act as the retest entry rather than trying to fade the first move. If SMT is present, the sweep can be treated as protected and the same breaker logic still applies.

The old-daily-lows IFVG reentry clip shows the same idea after a profitable stop-out: the broken daily-low zone can still function as a breaker if the higher-time-frame draw has not completed.

## See also

- [[concepts/order-block]]
- [[concepts/fair-value-gap]]
- [[concepts/pd-array]]
- [[concepts/change-in-state-of-delivery]]
- [[concepts/discount-premium]]
- [[concepts/liquidity-sweep]]
- [[models/internal-external-liquidity-model]]
