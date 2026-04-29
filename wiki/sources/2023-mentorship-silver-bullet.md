---
type: source
title: "2023 ICT Mentorship - ICT Silver Bullet Time Based Trading Model"
source_type: youtube
raw: "[[Clippings/2023 ICT Mentorship - ICT Silver Bullet Time Based Trading Model]]"
date_ingested: 2026-04-15
key_concepts: [silver-bullet, fair-value-gap, liquidity, optimal-trade-entry, draw-on-liquidity, market-structure-shift, new-week-opening-gap, killzones, NQ, MNQ]
tags: [source, silver-bullet]
aliases: ["Silver Bullet 2023 Mentorship"]
---

# 2023 ICT Mentorship - ICT Silver Bullet Time Based Trading Model

## Summary

- Silver Bullet is a **time-based algorithmic trading model** for all asset classes, framed inside three specific 60-minute windows in NY local time (@ 0:06, @ 8:13).
- The three Silver Bullet windows are **3:00–4:00 AM (London Open SB)**, **10:00–11:00 AM (AM Session SB)**, and **2:00–3:00 PM (PM Session SB)**, all New York local time (@ 8:50, @ 12:18, @ 14:11).
- Minimum trade framework: **10 handles / 40 ticks for index futures**, or **15 pips for Forex** — this is the *potential* range the move should offer, not the entry-to-exit target (@ 0:22, @ 0:48, @ 1:52).
- The setup uses a **fair value gap** that forms inside the 60-minute window; entry is taken inside the window but the trade is often held beyond it (@ 9:38, @ 11:27, @ 13:39).
- The single most important skill is determining the **next draw on liquidity** — where price is trying to go — not entry/exit precision (@ 7:23, @ 7:48).
- Candidate draws on liquidity include: previous day high/low, previous session (London/NY) high/low, previous weekly high/low, current or old new week opening gap, classic OTE, and inefficiencies / fair value gaps above or below price (@ 3:47–6:41).
- One Silver Bullet setup forms **every single trading day** in some market; the user is encouraged to specialize in one market and wait for whichever of the three windows delivers (@ 17:15, @ 18:07).
- Charts must be **calibrated to New York local time** (with DST observed) for the windows to apply correctly (@ 9:06).

## Key quotes

- **@ 0:06** — "we're going to be talking about my ICT Silver Bullet trade setup which is a time-based algorithmic trading model for all asset classes"
- **@ 0:22** — "the minimum trade framework should be 10 points or 40 ticks for index futures"
- **@ 0:48** — "the minimum trade framework should be 15 Pips for Forex"
- **@ 1:13** — "this framework is the best case price delivery that you expect to see... not your actual trade entry to exit range"
- **@ 2:18** — "10 handles for indices is the same to me as 20 Pips in Forex; five handles for indices is the same to me as 10 Pips in Forex"
- **@ 3:47** — "the framework for many ICT Silver Bullet setups are as follows but they're not limited to: previous day high or low draw on liquidity..."
- **@ 5:31** — "a classic ICT optimal trade entry... I think the fair value Gap has taken the throne" as the flagship pattern
- **@ 7:23** — "the main emphasis is determining the next most likely draw in the price action — where is price likely to go to next; that's the number one goal"
- **@ 8:50** — "first setup time is 3:00 a.m. to 4:00 a.m." (London Open Silver Bullet)
- **@ 9:06** — "you have to have your charts calibrated to New York local time... if we're observing daylight savings time then you observe Daylight Saving"
- **@ 9:38** — "what we're looking for is a classic ICT fair value Gap that forms between 3:00 a.m. and 4:00 a.m. New York local time"
- **@ 11:27** — "the entry is taken inside of that 60-minute window between 3:00 a.m. and 4:00 a.m. it does not mean that the trade is entered and is exited in the same 60-minute window"
- **@ 12:18** — "the second one... is the am session... focusing on the 10:00 a.m. to 11:00 a.m. always New York local time"
- **@ 14:11** — "our last ICT Silver Bullet here which is framed on 2:00 p.m. to 3:00 p.m. New York local time and this is the PM session"
- **@ 14:48** — "the Wicks do the damage but the body's telling you the narrative — the story is told by the bodies"
- **@ 17:15** — "you can't get anything better than having a specific 60-minute window of opportunity that forms every single trading day"
- **@ 18:07** — "if you don't get this set up in London you wait for it in the AM session if you don't get it there you wait for it in the PM session"

## See also

- [[models/silver-bullet]]
- [[concepts/fair-value-gap]]
- [[concepts/liquidity]]
- [[concepts/draw-on-liquidity]]
- [[concepts/optimal-trade-entry]]
- [[concepts/market-structure-shift]]
- [[concepts/new-week-opening-gap]]
- [[timing/silver-bullet-windows]]
- [[timing/new-york-local-time]]
- [[synthesis/how-to-use-price-delivery-continuum]]
- [[synthesis/how-to-use-first-presented-fvg]]
- [[synthesis/how-to-trade-the-930-11am-window]]
- [[instruments/NQ]]
- [[instruments/MNQ]]
