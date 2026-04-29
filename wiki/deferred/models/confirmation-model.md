---
type: model
aliases: [Confirmation Model, A+ Confirmation Model, Confirmation Checklist]
tags: [model, execution, confirmation, ict-core]
---

# Confirmation Model

A supporting execution model built around stacked confirmation rather than first-touch aggression. It looks for a higher-time-frame fair value gap, a liquidity sweep inside OTE, SMT / internal-liquidity confirmation, then an IFVG and change in state of delivery before entry.

## Status in this wiki

For Hermes-trading-analyst, this is a **supporting execution checklist**, not a primary standalone trigger. Use it when a chart already has a directional bias and you want one more layer of confirmation before committing risk.

## Working definition

- Start from a higher-time-frame fair value gap and a clear draw on liquidity.
- Wait for price to retrace into OTE and sweep liquidity.
- Confirm whether SMT and internal-liquidity behavior support the thesis.
- Look for an inversion fair value gap and a change in state of delivery.
- Enter only when the target path toward opposing liquidity is still clean.
- Treat the whole sequence as a mechanical confirmation checklist, not a prediction game.

The "Confirmation Model" source version makes the sequence explicit as a checklist: HTF FVG and draw, OTE liquidity sweep, SMT / internal-liquidity confirmation, IFVG, then CISD before taking the trade toward opposing liquidity ([[sources/the-confirmation-model]]).

## Relationship to other pages

- Uses [[concepts/optimal-trade-entry]] as the older retracement zone reference.
- Relies on [[concepts/fair-value-gap]] as the main directional delivery array.
- Uses [[concepts/smt]] and [[concepts/liquidity-sweep]] as confirmation signals.
- Uses [[concepts/inversion-fair-value-gap]] and [[concepts/change-in-state-of-delivery]] as the final trigger pair.
- Fits naturally alongside [[models/internal-external-liquidity-model]] and [[models/fractal-model]] as a confirmation / routing layer.

## See also

- [[sources/the-confirmation-model]]
- [[concepts/optimal-trade-entry]]
- [[concepts/fair-value-gap]]
- [[concepts/smt]]
- [[concepts/liquidity-sweep]]
- [[concepts/inversion-fair-value-gap]]
- [[concepts/change-in-state-of-delivery]]
- [[models/internal-external-liquidity-model]]
- [[models/fractal-model]]
