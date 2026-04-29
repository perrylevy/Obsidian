---
type: concept
aliases: [Relative Equal Highs/Lows, Equal Highs and Lows]
tags: [concept, liquidity, structure]
---

# Relative Equal Highs & Lows

Relative equal highs and relative equal lows are mirrored liquidity-cluster concepts. The levels do not need to be perfectly equal; they only need to be close enough to advertise a smooth target side for price to reach ([[sources/2024-mentorship-lecture-1]] @ 57:42–58:06, @ 1:15:39–1:18:04, [[sources/internal-external-liquidity]] @ 11:16).

## Core idea

- nearby highs that look almost equal advertise **buyside liquidity**
- nearby lows that look almost equal advertise **sellside liquidity**
- the smoother side often becomes the next draw on liquidity

The 2022 mentorship Episode 13 adds a practical cue: relative equal highs are where **retail traders see "resistance"** and place sell orders, creating the short-side liquidity that the algorithm targets ([[sources/2022-ict-mentorship-episode-13]]). Episode 16 reinforces the same idea by treating nearby highs and lows as explicit liquidity pools that the algorithm is most likely to target in the session ([[sources/2022-ict-mentorship-episode-16]]).

The mirror applies to relative equal lows — retail sees "support," placing buys that create long-side liquidity.

Episode 36 shows the same concept as a practical entry filter: relative equal highs/lows sit inside the broader premium/discount and liquidity map, helping define where the session may probe before the final expansion ([[sources/2022-ict-mentorship-episode-36]]). Episode 37 keeps the same basket of buy-side targets in view: the short-term high and nearby relative equal highs are the obvious upside draw, and the stop run is the way price clears them once the session is ready to expand ([[sources/2022-ict-mentorship-episode-37]] @ 0:43, @ 23:09).

## Why this is now one page

The bullish and bearish versions are mirrored enough that keeping them as separate full doctrine pages was adding vocabulary density without adding much retrieval value.

## Practical use

- If price is below relative equal highs, treat them as an upside draw.
- If price is above relative equal lows, treat them as a downside draw.
- Use the surrounding session structure and PD-array context to decide whether the sweep is the destination or only the setup for the next move.

## See also

- [[concepts/liquidity]]
- [[concepts/draw-on-liquidity]]
- [[concepts/buyside-liquidity]]
- [[concepts/sellside-liquidity]]
- [[deferred/concepts/last-line-of-defense]]
