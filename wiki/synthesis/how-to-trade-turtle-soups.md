---
type: synthesis
aliases: [Turtle Soup Playbook, Liquidity Sweep Playbook, How to Trade Liquidity Sweeps]
tags: [synthesis, playbook, liquidity, reversal]
---

# How to Trade Turtle Soups

This page is the operator guide for **Turtle Soup / liquidity sweep** setups. The practical sequence is: identify the swing point, decide whether the leg is a sweep or a run, require the best version of the setup to have no FVG in the lead-in leg, and then trade the reversal only when the market has clearly failed to stay comfortable beyond the level ([[models/turtle-soup]], [[sources/how-to-trade-turtle-soups]] @ 3:48, @ 8:30, @ 11:47, @ 13:57).

## Core idea

Turtle Soup is not just "price went above a high and came back." The source treats it as a specific liquidity behavior:
- a swing point is the pool,
- breakout traders place stops around it,
- the sweep takes those stops,
- and the reversal uses that harvested liquidity as fuel.

The cleanest version is the one where the market is not simply running through the level in the same direction.

## How to classify the move

### 1. Identify the swing point

Start with the nearest meaningful swing high or swing low. That swing is liquidity because it is where breakout orders and protective stops cluster.

### 2. Decide sweep vs run

Ask whether price:
- trades through the level and immediately reverses = sweep,
- or trades through and stays comfortably beyond it = run.

Comfort above a high or below a low is the giveaway that it is not a clean sweep.

### 3. Check the lead-in leg

The source is clear that a sweep is more likely when the leg into the swing point has no FVG. If the leg already contains an FVG, the market is more likely to continue as a run than to reverse sharply.

### 4. Use candle-science / fractal confirmation

The same logic works on different scales:
- a current-TF swing sweep,
- or a previous-candle-high / previous-candle-low sweep on a lower TF.

The source treats those as fractal versions of the same structure.

### 5. Be extra careful with mitigated gaps

Once price trades into a fair value area or FVG, that area is no longer the main trade location. The source prefers the swing point left behind at the gap, not the already-mitigated gap itself.

## Practical execution map

### Carry-forward pre-session variant

If a prior-session FVG is still the active short-side or long-side reference into the new session, you can carry it forward as part of the setup context. But the Turtle Soup decision still depends on the fresh swing being swept or run in the current session; the older array is context, not a substitute for the new liquidity event.

### Premarket ICT short variant

The premarket live-execution short on January 21, 2025 uses the same logic on the NQ pre-open: a buy-side raid, then a rejection back lower, with the stop above the working imbalance and the target on the sellside draw ([[sources/january-21-2025-live-execution-nq-premarket-turtle-soup-short]] @ 0:11, @ 1:08, @ 1:42, @ 5:37, @ 11:25).

### Asian-range variant

The derivative "insane winrate" framing applies the same Turtle Soup logic to the Asian session high/low after the 2:00 a.m. New York close: mark the completed Asian range, wait for one side to be taken, then require the opposite side to be taken as well before taking the reversal. The actual entry comes after acceptance back into the range or a double-sweep retest on the 15-minute chart ([[sources/best-ict-turtle-soup-trading-strategy-that-works-insane-winrate]] @ 2:25, @ 3:58, @ 6:46, @ 10:04, @ 10:28).

This is a clean derivative example of the Asian-range scaffold inside a Turtle Soup-style reversal model.

### A. Best-case long Turtle Soup

1. Price sweeps sellside liquidity below a swing low.
2. The market immediately rejects and reclaims.
3. There is no strong FVG in the leg into the low.
4. Entry is taken on the rejection / expansion back higher.

### B. Best-case short Turtle Soup

1. Price sweeps buyside liquidity above a swing high.
2. The market immediately rejects and loses the level.
3. There is no strong FVG in the leg into the high.
4. Entry is taken on the rejection / expansion lower.

### C. When not to call it Turtle Soup

If price stays above the high or below the low for too long, or if the lead-in leg already has a strong FVG, treat it as a run instead of forcing a reversal label.

## What to avoid

- Do not use every wick-through as a Turtle Soup.
- Do not ignore the difference between sweep and run.
- Do not fade a strong FVG-supported run as if it were a sweep.
- Do not keep the old gap as the trade location after it has been mitigated.

## Fast checklist

Before trading, ask:
1. What is the swing point / liquidity pool?
2. Did price sweep or run?
3. Is the market comfortable beyond the level?
4. Was there an FVG in the lead-in leg?
5. Is the setup aligned with the fractal / candle-science version of the same idea?

## See also

- [[models/turtle-soup]]
- [[concepts/liquidity-sweep]]
- [[concepts/liquidity-run]]
- [[deferred/concepts/last-line-of-defense]]
- [[deferred/concepts/rejection-block]]
- [[concepts/fair-value-gap]]
- [[concepts/candle-science]]
- [[timing/asian-range]]
- [[sources/how-to-trade-turtle-soups]]
- [[sources/2025-lecture-series-nq-review-presession-buyside-turtle-soup-trade-may-14-2025]]
