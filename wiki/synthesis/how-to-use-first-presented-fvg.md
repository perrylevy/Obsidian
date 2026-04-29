---
type: synthesis
aliases: [First Presented FVG Playbook, 9:30 First FVG Guide]
tags: [synthesis, playbook, NQ, timing]
---

# How to Use First Presented FVG

This page is a practical guide for using the **first presented fair value gap** as an execution scaffold on NQ, especially around the AM and PM opening windows.

## Core idea

The first presented FVG is not just "the first FVG you happen to notice." In the clearest ICT-direct formulation currently in this wiki, it means the **first valid 1-minute FVG inside a defined session window** — most importantly the 9:30–10:00 AM opening range, and by extension the 1:30–2:00 PM session window ([[timing/first-presented-fvg]], [[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 8:29, @ 12:01, @ 47:42).

## When to use it

Use first presented FVG logic when:
- a new session window has begun,
- you want the session's first trustworthy displacement array,
- and the chart is noisy enough that plotting every later FVG would create clutter instead of clarity.

This is especially useful when the trader wants a repeatable routine rather than improvising a new array selection process each day ([[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 20:16, @ 47:42, @ 48:11).

The 03/08/2026 market commentary reinforces the same habit: define the RTH opening-range gap first, then let the first valid 1-minute FVG inside that window do the work while ETH remains contextual background only ([[sources/ict-2026-market-commentary-march-08-2026]] @ 10:02, @ 13:19–13:43, @ 15:30, @ 17:29–18:26).

## Session-specific rule set

### AM session

For the morning session, the operative rule is:
- use the **first valid 1-minute FVG formed between 9:31 and 10:00 ET** as the morning's working array ([[timing/first-presented-fvg]], [[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 8:29, @ 47:42).

### PM session

For the afternoon session, repeat the same logic in the **1:30–2:00 ET** opening window. The PM session gets its own first-presented-FVG reference and should not be assumed to be identical to the AM one ([[timing/first-presented-fvg]], [[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 12:01, @ 43:48).

### Weekly-close / Asian-session variation

The same doctrine can show up outside the U.S. open. On the May 29 review, an **Asian-session first presented FVG** is used as the opening anchor, then the same idea is revisited through the PM session while the weekly close remains in view ([[sources/2025-lecture-series-nq-review-may-29-2025]] @ 6:49, @ 8:25, @ 9:35).

That means the operator should keep the session logic, but not make it U.S.-open exclusive:
- the active session still supplies the working array,
- the higher-time-frame weekly draw still matters,
- and the first valid FVG in the relevant window remains the anchor.

### Carry-forward / prior-session variation

The April 9 extraordinary-volatility review shows a useful carry-forward wrinkle: ICT keeps a Friday 9:35 first presented FVG and a later 12:10 FVG in view while building the next day’s map, but the live session still needs its own validation before the array becomes operative ([[sources/2025-lecture-series-nq-review-extraordinary-volatility-04092025]] @ 11:38, @ 12:44, @ 15:00, @ 16:01).

Practical rule:
- keep older arrays on the chart when they still explain the draw,
- but do not let them replace the active session’s first valid 1-minute FVG.

### Venom / deferred-entry variation

The May 12 Venom example shows the same first-presented-FVG logic from a more selective angle: on a premium-open Monday, the market can spend a long time in sideways distortion, but the workable long is still the one that waits for the sellside raid, then buys at the opening price or lower once the turn is proven. In that clip, the first presented FVG and the inversion FVG are the validation layer, not the chase trigger ([[sources/2025-lecture-series-ict-venom-example-may-12-2025]]).

### News / impulse variation

On impulse-driven days like CPI, the first presented FVG after the driver move can become the operative array — but only if price validates it instead of immediately losing it. If validation is weak, the correct action is often no trade ([[timing/first-presented-fvg]], [[sources/2025-lecture-series-nq-review-cpi-no-trade-may-13-2025]] @ 1:23, @ 3:51).

The April 30 NQ review shows the same pattern in a cleaner post-spike form: the first presented FVG becomes an inversion FVG after the 10:00 news impulse, then the session resumes from the validated array rather than chasing the spike itself ([[sources/nq-review-april-30-2025]] @ 7:24, @ 9:04, @ 9:31).

The 04/04/2025 NFP delivery review is the clean open-to-news variant for this page: the 9:30 open’s first presented FVG stays live through the 10:00 release if bodies continue to validate it, and the better morning rhythm is 9:50–10:10 for the first drive with 10:50–11:10 as the late-morning objective window ([[sources/2025-lecture-series-nq-nfp-algorithmic-price-delivery-04042025]] @ 0:33, @ 1:04, @ 1:22, @ 1:39, @ 7:55, @ 9:04, @ 10:51).

## How to frame it correctly

### 1. Start with time first

Do not begin by scanning for every visible FVG. Begin by defining the session window:
- 9:30–10:00 AM,
- or 1:30–2:00 PM,
- or the specific post-news impulse window.

This follows the broader ICT principle that time leads delivery and price then refers to the proper array ([[timing/macros]], [[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 23:28, @ 24:27).

### 2. Blend the FVG with the opening-range gap

On the May 18 source, the first presented FVG is explicitly blended with the **opening-range gap**. The opening gap from prior RTH settlement to the new RTH open is measured, and its consequent encroachment becomes a pullback expectation inside the same framework ([[concepts/new-day-opening-gap]], [[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 10:06, @ 12:46, @ 13:16, @ 14:03).

In practice this means:
- the opening-range gap and first presented FVG are often one integrated frame,
- not two unrelated tools.

### 3. Blend RTH and ETH intelligently

The first presented FVG works best when RTH and ETH are both considered:
- RTH defines the true opening structure,
- ETH preserves the overnight liquidity map from Asia, London, and premarket.

That means the array is chosen from the session window, but the draw on liquidity may still be informed by overnight pools ([[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 9:42, @ 10:39, @ 18:42, @ 19:18).

The same clip distinguishes between a tier 1 and tier 2 long framework using the 8:30 and midnight opening prices: beneath both opening prices is the deep-discount / tier 2 pocket, while between them is the more transitional tier 1 zone.

This matters because the first presented FVG is not always the best entry on its own. In a bullish setup, a deeper discount pocket or a bullish order-block / breaker refinement can be the cleaner entry inside the same frame ([[sources/nq-trade-breakdown-how-to-pick-the-right-first-presented-fvg-ict-concepts]]).

## What it helps prevent

Used correctly, first presented FVG helps prevent:
- chasing random later-session FVGs,
- over-annotating the chart,
- picking a different "favorite" gap every day,
- and treating every visible inefficiency as equally important.

The source is very explicit that the value here is routine and repeatability, not complexity for its own sake ([[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 20:44, @ 21:19, @ 47:42, @ 48:11).

## Practical checklist

1. Define the active session window.
2. Mark the first valid 1-minute FVG inside that window.
3. Check the opening-range gap / NDOG relation.
4. Identify the relevant liquidity pools from RTH + ETH context.
5. Decide whether price is validating or violating the level.
6. Use that anchored array instead of cluttering the chart with every later gap.

## What not to do

- Do not use "first presented FVG" to mean simply "the first FVG I noticed after the move was already underway."
- Do not ignore the session window.
- Do not separate the array from the opening-range gap when the source is explicitly blending them.
- Do not ignore overnight liquidity just because the execution is based on RTH structure.
- Do not assume the AM first presented FVG governs the PM session too.

## See also

- [[timing/first-presented-fvg]]
- [[concepts/fair-value-gap]]
- [[concepts/new-day-opening-gap]]
- [[concepts/new-week-opening-gap]]
- [[timing/macros]]
- [[concepts/consequent-encroachment]]
- [[instruments/NQ]]
