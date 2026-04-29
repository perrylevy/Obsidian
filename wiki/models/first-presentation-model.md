---
type: model
aliases: [First Presentation Model, First Presentation Scalping, First Presentation Gap Model]
tags: [model, timing, scalping, ict-core]
---

# First Presentation Model

A **session-scalping model** built around the first valid 1-minute fair value gap after the open. The setup starts from a higher-time-frame inefficiency, waits for the session's first presented FVG, and uses that gap as the execution anchor for a small, one-way run ([[sources/first-presentation-model-1-scalping]] @ 1:47, @ 3:40, @ 4:11, @ 18:47).

## Status in this wiki

For Hermes-trading-analyst, this is the **default opening-session execution model**. If the task is to generate trade ideas for the user's 9:30–11:00 a.m. ET workflow, this page should usually outrank broader or more derivative model pages unless the chart is clearly behaving like a liquidity-sweep reversal or a fixed-window Silver Bullet setup.

## Working definition

- Start by marking the 15-minute or 5-minute inefficiency that frames the morning range ([[sources/first-presentation-model-1-scalping]] @ 1:47).
- After 9:30 ET, wait for the first 1-minute FVG to appear; that is the first presentation [[timing/first-presented-fvg|first presented FVG]] ([[sources/first-presentation-model-1-scalping]] @ 3:40).
- Enter inside the gap, with the 50% line treated as the best anchor ([[sources/first-presentation-model-1-scalping]] @ 18:47).
- Favor modest targets: minor inefficiency fills, scalp-size expansion, or the nearest liquidity checkpoint rather than a swing objective ([[sources/first-presentation-model-1-scalping]] @ 4:11).
- The source emphasizes one-way order flow and notes that the same logic can be fractalized to 15-second charts for tighter execution ([[sources/first-presentation-model-1-scalping]] @ 4:11, @ 14:45).
- Logging the day, time, and screenshot is part of the process; the model is built by tracking recurring conditions over time ([[sources/first-presentation-model-1-scalping]] @ 19:21).
- The May 12, 2025 Venom example is a deferred-entry variant of this same family: after a sellside raid, ICT wants the buyer at the opening price or lower and then lets the first presented FVG / inversion FVG carry the move ([[sources/2025-lecture-series-ict-venom-example-may-12-2025]]).

## Risk & stop placement

- **Entry trigger**: wait for the first qualifying FVG inside the session window to form *after* a displacement leg; do not anticipate ([[concepts/displacement]], [[concepts/fair-value-gap]]).
- **Stop placement**: beyond the swing that created the first presentation — i.e. above the high for a short or below the low for a long. If the entry is taken from a 1m FVG nested inside a 5m FVG, the pragmatic stop is the far side of the 5m parent FVG so small 1m wicks don't take you out ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 6:46, @ 15:22). Invalidation is a full-body close back through the FVG's far boundary.
- **Target**: the next [[concepts/draw-on-liquidity|draw on liquidity]] — typically the relative equal high/low, prior session high/low, or opposing FVG that framed the session. On a clean expansion, the first presentation usually runs one liquidity pool, not two, so partial at the first target and trail the runner behind the last FVG ([[synthesis/how-to-use-order-flow-entries]]).
- **Invalidation / time stop**: if the market does not displace within the first-presentation window, stand down — this model is narrow by design.

## Relationship to other pages

- Inherits its timing anchor from [[timing/first-presented-fvg]].
- Uses [[concepts/fair-value-gap]] as the actual entry array.
- The execution style is related to [[synthesis/how-to-use-order-flow-entries]] because it prefers a one-way run after the first presentation.
- It is a morning-session cousin of [[models/silver-bullet]], but narrower and more scalping-oriented.
- It is usually traded inside the opening-range frame after the cash open rather than as a standalone all-day model.

## See also

- [[sources/first-presentation-model-1-scalping]]
- [[timing/first-presented-fvg]]
- [[concepts/fair-value-gap]]
- [[synthesis/how-to-use-order-flow-entries]]
- [[deferred/models/venom-model]]
- [[timing/macros]]
- [[concepts/liquidity]]
- [[timing/opening-range]]
- [[timing/new-york-local-time]]
