---
type: synthesis
aliases: [Intraday NQ Playbook, Intraday MNQ Playbook, NQ Intraday Playbook, MNQ Playbook]
tags: [synthesis, playbook, intraday, nq, mnq, execution]
---

# Intraday NQ / MNQ Playbook

End-to-end operator sequence for reading the NQ / MNQ tape intraday, identifying which model is in play, and producing a trade plan with entry, stop, and target. Every step resolves to an existing wiki page; this page is the glue, not new doctrine.

Use this as the top-of-session checklist. If a step cannot be answered, stand down for that step before proceeding.

## Step 1 — HTF context (before 8:00 a.m. NY)

- **Daily bias**: read per [[synthesis/how-to-build-daily-bias]]. Identify the weekly delivery phase ([[models/power-of-three]] on the weekly scale) and whether Monday/Tuesday manipulation has already run.
- **Draw on liquidity**: mark the live [[concepts/draw-on-liquidity]] — prior day / prior week high-low, relative equal highs-lows, unclaimed NWOG/NDOG.
- **Daily wick anchor**: identify the most relevant daily wick and mark its **consequent encroachment** (midpoint down to close for shorts; midpoint up to close for longs). This is the intraday setup pocket for SB / MM Buy / MM Sell / Unicorn ([[sources/2025-storytellers-daily-high-to-low-june-21-2025]] @ 3:34).
- **PD array matrix**: grade the 20-day range by quadrant per [[synthesis/how-to-use-pd-array-matrix]]. Only trade arrays in the inner two quadrants unless expecting a full reversal.

## Step 2 — Session frame (8:00–9:25 a.m. NY)

- **Midnight opening price** and **midnight opening range** — record per [[concepts/midnight-opening-price]], [[timing/midnight-opening-range]].
- **Asian range** — mark high-low per [[timing/asian-range]].
- **New Day / New Week Opening Gap** — [[concepts/new-day-opening-gap]], [[concepts/new-week-opening-gap]].
- **Opening Range Gap** — prior settlement vs 9:30 open per [[concepts/opening-range-gap]].
- **No-initial-bias guard**: if HTF context is genuinely ambiguous, follow [[synthesis/how-to-trade-when-you-dont-have-an-initial-bias]] and do not force a model selection.

## Step 3 — Window selection (9:25 a.m. onward)

- **Silver Bullet windows**: 10:00–11:00 a.m. AM SB, 2:00–3:00 p.m. PM SB ([[timing/silver-bullet-windows]]).
- **First-presented FVG window**: per [[timing/first-presented-fvg]] — the first valid FVG inside the opening range is the executable array **after** displacement.
- **9:30–11:00 a.m. focus window**: follow [[synthesis/how-to-trade-the-930-11am-window]].
- **Macros**: [[timing/macros]], [[timing/lunch-macro]], [[timing/quarters-of-the-hour]].
- **News guard**: FOMC / CPI / NFP — on those weeks, apply [[synthesis/how-to-handle-cpi-no-trade-days]] and the PO3 FOMC rules.

## Step 4 — Model identification

Pick the one model the tape is actually expressing. If two models conflict, pick the one whose timing window is active now and whose draw is still unreached.

| Model | Trigger window | Manipulation cue | Entry array |
|-------|----------------|------------------|-------------|
| [[models/power-of-three]] | session / day / week | Judas swing takes one side | FVG/OB from displacement into Distribution |
| [[models/silver-bullet]] | 10–11 AM / 2–3 PM | sweep into draw inside window | displacement FVG (1m nested in 5m on NQ/MNQ) |
| [[models/turtle-soup]] | Asian-range / session high-low raid | sweep + SFP close back through | IFVG or candle-close entry |
| [[models/first-presentation-model]] | opening range | first displacement after cash open | first valid FVG inside opening range |
| [[models/market-maker-buy-model]] | HTF accumulation zone | sweep into discount | discount FVG / breaker / OB in accumulation |
| [[models/market-maker-sell-model]] | HTF distribution zone | role-flipped PD array | premium FVG / breaker rejecting the array |
| [[models/internal-external-liquidity-model]] | killzone | external-liquidity raid | FVG inside internal-liquidity zone after MSS |
| [[models/fractal-model]] | nested HTF → LTF | LTF sweep confirming HTF narrative | IFVG or displacement FVG on LTF |

## Step 5 — Entry trigger

Canonical sequence regardless of model:

1. Identify the **sweep** of the engineered pool (liquidity sweep / judas swing / inducement — all resolve to [[concepts/liquidity-sweep]]).
2. Wait for [[concepts/displacement]] — aggressive full-bodied delivery back through the sweep.
3. Select the PD array the displacement leaves behind: [[concepts/fair-value-gap]], [[concepts/inversion-fair-value-gap]], [[concepts/order-block]], [[concepts/breaker-block]], or [[concepts/suspension-block]].
4. Require the array to sit in the correct PD array matrix quadrant.
5. Enter on the array, ideally with body-based confirmation that it is holding ([[concepts/consequent-encroachment]] / [[concepts/mean-threshold]]).

If there is no displacement, there is no entry. No shortcuts.

## Step 6 — Stop placement (per model)

Every model page has a "Risk & stop placement" section. Summary:

- **PO3**: beyond the Manipulation extreme (far side of Judas swing / swept pool).
- **Silver Bullet**: beyond the sweep wick, or far side of the 5m parent FVG if nested.
- **Turtle Soup**: above the working candle / imbalance that defines the sweep ([[models/turtle-soup]]).
- **First Presentation**: beyond the swing that created the first presentation.
- **MM Buy**: below accumulation-zone low or smart-money-reversal low.
- **MM Sell**: above distribution high or the role-flipped PD array.
- **Internal-External Liquidity**: beyond the external-liquidity wick that was swept.
- **Fractal**: beyond the extreme of the sweeping candle on the operative LTF.

Universal rule: the stop protects the level that defines the setup. If that level is invalidated, the model is wrong — do not widen.

## Step 7 — Target & management

- **Primary target**: the [[concepts/draw-on-liquidity]] that was identified in Step 1 (opposite-side liquidity pool).
- **Intermediate partials**: first relative-equal highs-lows cluster, next FVG / OB, or consequent encroachment of the parent HTF wick.
- **Runner management**: trail the runner behind the last displacement FVG or the last respected mean threshold.
- **Model-specific targets**:
  - Silver Bullet: -2 SD projection is a documented MNQ exit reference ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 30:59).
  - MM Buy: distribution extreme / prior external buy-side.
  - MM Sell: accumulation zone / prior external sell-side.
  - PO3 weekly: prior week high / low on distribution leg.

## Step 8 — Invalidation / time stop

- **Window timeout**: Silver Bullet and macros are **time-bound**. If the setup has not triggered before the window closes, stand down.
- **Structural timeout**: a full-body close back through the sweep wick or the entry array invalidates the read.
- **News timeout**: pre-release moves on FOMC / CPI / NFP are usually Manipulation; wait for the event to digest before committing to Distribution direction ([[sources/simple-power-of-three]] @ 5:57).
- **Missed entry**: if price has already left the array without you, do not chase — follow [[synthesis/how-to-manage-missed-entries]].
- **Heavy-manipulation days**: execute smaller and tighter, or stand down; see [[synthesis/how-to-handle-heavy-manipulation-days]].

## Step 9 — Instrument selection (NQ vs MNQ vs SMT leg)

- On SMT divergence, enter on the **divergent leg** of ES/NQ/YM. If NQ is diverging, MNQ is the preferred entry instrument; if ES or YM diverges instead, defer MNQ and trade the divergent index ([[instruments/MNQ]], [[sources/intro-smt-divergence]]).
- Size MNQ at 1/10 the notional of NQ — same price action, smaller per-tick cost. MNQ tick value $0.50 vs NQ tick value $5.00 ([[instruments/MNQ]]).

## Step 10 — Journal

After the session, log per [[synthesis/how-to-journal-ict-time-signatures]]:

- HTF bias used, draw on liquidity, model chosen.
- Window timing, displacement clarity, PD array used.
- Entry, stop, targets, and whether the model executed cleanly.
- Any single-observation patterns to watch for repetition.

## See also

- [[instruments/NQ]], [[instruments/MNQ]]
- [[synthesis/how-to-build-daily-bias]]
- [[synthesis/how-to-map-ict-session-timing]]
- [[synthesis/how-to-use-pd-array-matrix]]
- [[synthesis/how-to-trade-the-930-11am-window]]
- [[synthesis/how-to-use-first-presented-fvg]]
- [[synthesis/how-to-trade-ifvg]]
- [[synthesis/how-to-trade-turtle-soups]]
- [[synthesis/how-to-use-order-flow-entries]]
- [[synthesis/how-to-manage-missed-entries]]
- [[synthesis/how-to-handle-cpi-no-trade-days]]
- [[synthesis/how-to-handle-heavy-manipulation-days]]
