---
type: model
aliases: [Turtle Soup]
tags: [model, reversal, liquidity]
---

# Turtle Soup

A **reversal pattern triggered by a liquidity sweep** — price trades through a swing point (high or low) and immediately reverses, trapping breakout traders ([[sources/how-to-trade-turtle-soups]] @ 2:35, @ 2:11).

## Status in this wiki

For Hermes-trading-analyst, Turtle Soup is the **default liquidity-sweep reversal family**. If the setup begins with a stop raid / sweep and immediate reclaim rather than a straightforward opening-session displacement, this page should usually outrank opening-session FVG models.

## Origin of the name

From the Turtle Traders' classic breakout system: buy-stops above swing highs, sell-stops below swing lows. Turtle Soup traps those breakout entries by sweeping their trigger level and immediately reversing. The trapped traders' stop-losses (at the opposite swing) become the Turtle Soup trader's take-profit ([[sources/how-to-trade-turtle-soups]] @ 1:12, @ 1:39, @ 6:26, @ 8:30).

## Three-way equivalence across sources

| Source | Equivalence |
|--------|-------------|
| [[sources/how-to-trade-turtle-soups]] (Arjo / MMC) @ 2:35 | Turtle Soup ≡ liquidity sweep (exact) |
| [[sources/simple-power-of-three]] (JadeCap) @ 6:22 | Turtle Soup ≡ swing failure pattern (SFP) |

Consistent — SFP is a specific flavor of liquidity sweep — but the framings differ in scope. Treat as synonyms in day-to-day usage; verify ICT's own terminology when an ICT-direct source on Turtle Soup is ingested.

The May 14, 2025 ICT review gives that direct confirmation: a presession buyside Turtle Soup is framed through the nearby FVG / IFVG context, the stop sits at half of the sweep wick, and the objective is the relative equal lows ([[sources/2025-lecture-series-nq-review-presession-buyside-turtle-soup-trade-may-14-2025]] @ 0:01, @ 2:43, @ 3:13, @ 3:22).

The "From Vision To Execution" lecture adds a continuation variant: after the sweep and displacement, the first presented FVG after the turtle-soup event is the standout array to project forward, and the trader should keep the draw in view until time either confirms or invalidates it ([[sources/from-vision-to-execution]]).
The June 24, 2024 and January 21, 2025 ICT executions add the practical stop logic: keep the stop above the working candle / imbalance and insist on strong follow-through away from the swept level ([[sources/june-24-2024-nq-turtle-soup-short]] @ 0:49, @ 1:44, @ 2:16, @ 4:34, [[sources/january-21-2025-live-execution-nq-premarket-turtle-soup-short]] @ 1:08, @ 1:42, @ 11:25).
The 04/21/2025 deferred-entry clip adds the rejection-block boundary explicitly: after the opening push, ICT labels the bearish rejection block as the close-price boundary and treats the pattern as a deferred Turtle Soup / false-breakout short once the market re-enters and fails to reclaim that level ([[sources/2025-lecture-series-turtle-soup-deferred-entry-with-rejection-block]] @ 10:25, @ 11:08, @ 12:10).

The 09/06/2024 OSOK execution and the 08/30/2024 PM-session clip both make Turtle Soup operational in live tape: sweep the high, accept the stop raid, and then let the bearish delivery leg unfold under the higher-time-frame sell-model context ([[sources/ict-nq-live-execution-september-6-2024-100k-osok]] @ 0:01, @ 3:00, @ 8:14; [[sources/nq-pm-session-turtle-soup-long-full-pull-august-30-2024]] @ 0:01, @ 2:04, @ 4:56, @ 8:14).

## Sweep vs Run (the core distinction)

- **Sweep** — through the swing, *immediate* reversal. Confirmation = "not comfortable above a high / below a low" — an aggressive expansion candle the opposite way, or a new FVG the opposite way ([[sources/how-to-trade-turtle-soups]] @ 8:30, @ 9:34, @ 9:54).
- **Run** — through the swing, *continuation* in the same direction. Lingering above the level implies a run.

If the leg into the swing point contains an FVG, **favor a run**, not a sweep ([[sources/how-to-trade-turtle-soups]] @ 11:47, @ 12:11).

## Last line of defense

Highest-quality Turtle Soup: the leg into the swing point is a "[[deferred/concepts/last-line-of-defense|last line of defense]]" — **no FVG** in the leg; price has no further PD array to lean on before the swing point ([[sources/how-to-trade-turtle-soups]] @ 11:25, @ 12:29).

## Two fractal variants

- **Order-flow sweep** — sweep of the current-TF swing high or low after a failed-rejection candle (no new FVG) ([[sources/how-to-trade-turtle-soups]] @ 13:28, @ 13:57).
- **Candle-science sweep** — sweep of a previous candle high (PCH) or previous candle low (PCL) on the current TF; equivalent to a swing sweep on the lower TF ([[sources/how-to-trade-turtle-soups]] @ 18:53, @ 19:13, @ 19:54).

## Asian-range variant

The derivative "insane winrate" framing uses the Asian session high/low as the working swing pair: mark the range after 2:00 a.m. New York time, wait for one side to be taken first, then require the opposite side to be taken as well before treating the setup as valid. The actual entry comes after acceptance back into the range or a double-sweep retest on the 15-minute chart ([[sources/best-ict-turtle-soup-trading-strategy-that-works-insane-winrate]] @ 2:25, @ 3:58, @ 6:46, @ 10:04, @ 10:28).

This is the clearest derivative example of the Asian-range scaffold inside a Turtle Soup-style reversal model.

## Stop-loss placement

The direct ICT executions now show the practical stop logic: place the stop above the working candle / imbalance that defines the sweep, not casually inside the reversal zone ([[sources/june-24-2024-nq-turtle-soup-short]] @ 0:49, @ 2:16, @ 4:34, [[sources/january-21-2025-live-execution-nq-premarket-turtle-soup-short]] @ 1:08, @ 1:42, @ 11:25).

## See also

- [[synthesis/how-to-trade-turtle-soups]]
- [[concepts/liquidity-sweep]]
- [[concepts/swing-failure-pattern]]
- [[concepts/buyside-liquidity]]
- [[concepts/sellside-liquidity]]
- [[concepts/candle-science]]
- [[concepts/candle-science]]
- [[deferred/concepts/last-line-of-defense]]
- [[deferred/concepts/rejection-block]]
- [[timing/asian-range]]
- [[models/power-of-three]]
- [[sources/2025-lecture-series-nq-review-presession-buyside-turtle-soup-trade-may-14-2025]]
- [[sources/june-24-2024-nq-turtle-soup-short]]
- [[sources/january-21-2025-live-execution-nq-premarket-turtle-soup-short]]
