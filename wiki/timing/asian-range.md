---
type: timing
aliases: [Asian Range, Asian session range]
tags: [timing, session]
---

# Asian Range

The Asian session range is the completed range defined after the 2:00 a.m. New York close used in these derivative lessons. Its high and low become the first liquidity scaffold for the rest of the day, especially on index products like NAS100 / NQ, US30, and S&P 500 ([[sources/best-ict-turtle-soup-trading-strategy-that-works-insane-winrate]] @ 2:25, @ 2:42, @ 12:51; [[sources/calubs-model-conceptually-variant-1]] @ 2:25, @ 2:42, [[sources/2024-mentorship-lecture-1]] @ 1:42:45–1:43:01, @ 1:51:44–1:52:32). Lecture 5 of the 2024 mentorship adds a stricter NY-local activation window: the Asian session is treated as the 7:00–9:00 p.m. NY window after the 6:00 p.m. reopen, where the NDOG, short-term liquidity pools, and the initial breakaway / displacement sequence define the tradeable structure ([[sources/2024-mentorship-lecture-5]]).


## Core rule

- If the Asian low is taken first, the day is initially framed bearish; the model then waits for the Asian high to be taken as well before looking for a short ([[sources/best-ict-turtle-soup-trading-strategy-that-works-insane-winrate]] @ 3:58, @ 4:30).
- If the Asian high is taken first, the day is initially framed bullish; the model then waits for the Asian low to be taken as well before looking for a long ([[sources/best-ict-turtle-soup-trading-strategy-that-works-insane-winrate]] @ 5:28, @ 7:20).
- In Calub's variant, that range logic is then traded only during the **first 30 minutes of each hour from 7:00 to 11:00 a.m. ET**, with 9:30–10:00 treated as the opening-range centerpiece ([[sources/calubs-model-conceptually-variant-1]] @ 3:29, @ 9:05).
- Acceptable entries come only after acceptance back into the range, a market-structure shift, or a double-sweep retest on the 15-minute chart ([[sources/best-ict-turtle-soup-trading-strategy-that-works-insane-winrate]] @ 6:14, @ 6:46, @ 10:04, @ 10:28, [[sources/calubs-model-conceptually-variant-1]] @ 6:14, @ 6:46, @ 7:38).

## Practical use

In the clipped examples the Asian range is used as a session-bias scaffold, not as a standalone signal. Its main role is to define which side of the day has already been raided and whether the follow-through setup is still pending.

## See also

- [[models/turtle-soup]]
- [[models/market-maker-buy-model]]
- [[timing/macros]]
- [[concepts/liquidity-sweep]]
