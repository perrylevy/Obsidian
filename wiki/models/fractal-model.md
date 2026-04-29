---
type: model
aliases: [Fractal Model, Fractal IFVG Model]
tags: [model, fractal, entry]
---

# Fractal Model

The fractal model is the multi-timeframe entry framework used in the IFVG material: higher-timeframe bias and swing context define the setup, and the lower timeframe provides the candle-two sweep and inversion entry. The same logic repeats across daily, 4H, 15m, and lower execution frames ([[sources/how-to-trade-ifvg]] @ 2:03, @ 8:14, [[sources/how-to-trade-ifvg]] @ 26:26–29:00).

The "This Stupid Simple Strategy Works Everyday" clip shows the same nesting in a deliberately compressed form: HTF FVG tap → 5-minute FVG confirmation → inversion → liquidity target. It is a clean reminder that the fractal model is about the relationship between layers, not about collecting more indicators ([[sources/this-stupid-simple-strategy-works-everyday-stupid-simple-and-proven]]).

The "Next Day Model - Fractal Way To Get Bias For Trading" clip extends that logic into a bias scaffold: the previous candle’s close, range failure, and phase change are used to anticipate the next candle or next session before the lower-time-frame entry even matters ([[sources/next-day-model-fractal-way-to-get-bias-for-trading]]).

## Status in this wiki

For Hermes-trading-analyst, the fractal model is a **time-frame alignment / nesting framework**. It improves confirmation quality, but it should not usually originate the trade idea by itself.

## Core idea

The model is built from recurring nested pieces:

- HTF expansion / bias,
- a lower-timeframe sweep candle,
- a small supporting wick,
- then an inversion / continuation trigger.

The important point is that the structure is fractal: the same sweep-and-invert logic can appear at multiple scales.

## Why it matters

Fractal structure is what lets the IFVG setup work across timeframes instead of being a single isolated pattern.

It also explains why [[concepts/time-frame-alignment]] is mandatory: the lower timeframe only matters when it is nested inside the larger context.

## Practical use

Use the fractal model when reading IFVGs or sweep-based reversals:

- identify the HTF narrative,
- find the sweeping candle on the lower TF,
- check that the wick / expansion shape supports the move,
- then take the inversion only if the structure is aligned.

## Risk & stop placement

- **Entry trigger**: HTF narrative aligned, LTF sweep + [[concepts/displacement|displacement]] back through the sweeping candle, entry on the IFVG or FVG created by that displacement ([[concepts/inversion-fair-value-gap]]).
- **Stop placement**: beyond the extreme of the sweeping candle — i.e. above the wick that took the buy-side for a short, below the wick that took the sell-side for a long. Do not hide the stop inside the reversal zone; that is the level the algorithm just used ([[sources/june-24-2024-nq-turtle-soup-short]] @ 2:16 applied as general sweep-stop rule).
- **Target**: next HTF liquidity pool in the direction of the new read; partial at the first LTF equal high/low and trail behind the last displacement FVG.
- **Invalidation**: full-body close back through the sweeping candle's extreme negates the fractal and the entry is wrong.

## See also
