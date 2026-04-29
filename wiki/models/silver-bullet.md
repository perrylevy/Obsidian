---
type: model
aliases: [Silver Bullet, SB, ICT Silver Bullet]
tags: [model, time-based, ict-core]
---

# Silver Bullet

A **time-based algorithmic trading model** applicable to all asset classes ([[sources/2023-mentorship-silver-bullet]] @ 0:06).

## Status in this wiki

For Hermes-trading-analyst, Silver Bullet is a **fixed-window execution family**, not the default cash-open model. It becomes most important when the chart is specifically trading the 10:00–11:00, 14:00–15:00, or London Silver Bullet windows rather than the broader 9:30 cash-open development.

## Windows (NY local time, DST-observant)

| Window | Label | NY Time |
|--------|-------|---------|
| London Open | London SB | 03:00–04:00 |
| AM Session | AM SB | 10:00–11:00 |
| PM Session | PM SB | 14:00–15:00 |

Cited at [[sources/2023-mentorship-silver-bullet]] @ 8:50, @ 12:18, @ 14:11. Charts must be calibrated to NY local time with DST observed ([[sources/2023-mentorship-silver-bullet]] @ 9:06).

## Entry trigger

A **[[concepts/fair-value-gap|Fair Value Gap]]** forming inside the 60-minute window ([[sources/2023-mentorship-silver-bullet]] @ 9:38). FVG is the current flagship — it "took the throne from OTE" ([[sources/2023-mentorship-silver-bullet]] @ 5:31).

## Minimum framework (potential range, not target)

- **Index futures** — 10 handles / 40 ticks ([[sources/2023-mentorship-silver-bullet]] @ 0:22).
- **Forex** — 15 pips ([[sources/2023-mentorship-silver-bullet]] @ 0:48).

This is the **potential range** the setup should offer, not the entry-to-exit target ([[sources/2023-mentorship-silver-bullet]] @ 1:13).

Equivalences: 10 handles ≈ 20 pips; 5 handles ≈ 10 pips ([[sources/2023-mentorship-silver-bullet]] @ 2:18).

## Execution rules

- Entry **must be taken inside** the 60-minute window; the trade is frequently held beyond it ([[sources/2023-mentorship-silver-bullet]] @ 11:27, @ 11:45).
- The **single most important skill** is identifying the next most likely [[concepts/draw-on-liquidity|draw on liquidity]] — *before* considering entries ([[sources/2023-mentorship-silver-bullet]] @ 7:23, @ 7:48).
- At least one Silver Bullet setup forms in *some* market every trading day ([[sources/2023-mentorship-silver-bullet]] @ 17:15).
- Specialize in one market and **wait**: if London SB doesn't deliver, wait for AM; if AM doesn't, wait for PM ([[sources/2023-mentorship-silver-bullet]] @ 18:07).

## Candidate draws on liquidity

- Previous day high / low
- Previous session (London / NY) high / low
- Previous weekly high / low
- Current or old [[concepts/new-week-opening-gap|New Week Opening Gap]]
- [[concepts/optimal-trade-entry|OTE]] zones
- FVGs sitting above / below price

Cited at [[sources/2023-mentorship-silver-bullet]] @ 3:47–6:41.

## Risk & stop placement

- **Entry trigger**: inside the Silver Bullet 1-hour window, wait for a liquidity sweep into the draw, then enter on the displacement FVG that forms within the window. Nested 1m-inside-5m FVGs are the preferred entry array on NQ/MNQ ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 0:36, @ 6:46).
- **Stop placement**: beyond the sweep wick that triggered the entry, OR the far side of the 5m parent FVG if the entry is nested — whichever is further. This protects against 1m noise inside a valid HTF array ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 15:22).
- **Target**: the draw-on-liquidity called out before the window opened — previous day/session high-low, NWOG, current NWOG, or relative equal highs-lows ([[sources/2023-mentorship-silver-bullet]] @ 3:47–6:41). -2 SD projection is a documented exit reference on MNQ ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 30:59).
- **Invalidation / time stop**: Silver Bullet is a **1-hour window**. If the setup does not trigger before the window closes, stand down — do not chase late entries outside the window.

## Confirmed on MNQ (single observation)

On **2025-02-13 PM Silver Bullet**, the model delivered textbook expansion on MNQ — a 1m FVG nested inside the upper half of a 5m FVG, -2 SD target achieved ([[sources/mnq-pm-silver-bullet-walkthrough]]). Details in [[instruments/MNQ]]. Single-trade data point; not sufficient to call a recurring MNQ edge.

## See also

- [[timing/silver-bullet-windows]]
- [[deferred/timing/killzones]]
- [[concepts/fair-value-gap]]
- [[concepts/draw-on-liquidity]]
- [[instruments/MNQ]]
