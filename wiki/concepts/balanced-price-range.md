---
type: concept
aliases: [BPR, Balanced Price Range]
tags: [concept, pd-array, price-action]
---

# Balanced Price Range

A balanced price range is the **efficient half** of a [[concepts/fair-value-gap|FVG]] where price has already traded back and forth enough that the area no longer represents clean displacement. In this wiki’s current working definition, the balanced half is the side of the gap that has already been repriced and therefore should not be treated as the remaining imbalance ([[concepts/consequent-encroachment]], [[sources/2025-price-delivery-continuum]] @ 16:59, @ 27:09).

## Core idea

When studying a bearish FVG, the **upper half** is the balanced price range; when studying a bullish FVG, the **lower half** is the balanced price range. The opposite half is the true imbalance that still needs to be delivered to ([[concepts/fair-value-gap]], [[sources/2025-price-delivery-continuum]] @ 16:59, @ 22:09).

## Relationship to CE

The [[concepts/consequent-encroachment|consequent encroachment]] is the midpoint boundary of the balanced half. In practical terms:
- CE marks the inner edge of the balanced area,
- the balanced half is the portion that has already become efficient,
- and the unfilled half is the live imbalance ([[concepts/consequent-encroachment]], [[sources/2025-price-delivery-continuum]] @ 04:38, @ 16:59).

## Why it matters

Balanced price range language is useful because it prevents the trader from treating every part of a gap as equally actionable. The source framing suggests:
- one half has already been worked,
- the other half still has the stronger delivery claim,
- and stop placement / entry logic should respect that asymmetry ([[concepts/fair-value-gap]], [[concepts/order-block]], [[sources/2025-price-delivery-continuum]] @ 27:09).

The weekly summary also uses a daily gap / volume-imbalance hybrid as a balanced-price-range style structure that can be repriced and then left behind once buy-side is taken ([[sources/2025-lecture-series-nq-weekly-summary-02282025]] @ 3:39, @ 5:52, @ 6:30). The January 27, 2025 GBP/USD NWOG lecture uses the same distinction live: the worked half of the IFVG / NWOG is treated as balanced price range while the remaining half is the live imbalance ([[sources/2025-lecture-series-smc-new-york-nwog-with-forex-01272025]] @ 5:45, @ 6:25, @ 8:24). Lecture 16 of the 2024 mentorship reinforces the same structure on an NQ opening-day chart by describing a worked segment of the opening range as balanced price range and then leaving the remaining half as the live imbalance / draw ([[sources/2024-mentorship-lecture-16]] @ 13:59, @ 15:15, @ 18:23).

## Practical usage

Use balanced price range thinking when:
- you want to know which side of an FVG is already efficient,
- you need to distinguish the live imbalance from the worked half,
- or you are checking whether a gap-like area should still be expected to act as a draw.

## See also

- [[concepts/fair-value-gap]]
- [[concepts/consequent-encroachment]]
- [[concepts/volume-imbalance]]
- [[concepts/order-block]]
- [[concepts/pd-array]]
- [[sources/2025-price-delivery-continuum]]
- [[sources/2025-lecture-series-nq-weekly-summary-02282025]]
