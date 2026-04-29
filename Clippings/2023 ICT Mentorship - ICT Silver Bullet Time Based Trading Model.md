---
title: "2023 ICT Mentorship - ICT Silver Bullet Time Based Trading Model"
source: "https://www.youtube.com/watch?si=BpSgDAk-56v8Ovxt&v=tRq1hyGGtl4&feature=youtu.be"
author:
  - "[[The Inner Circle Trader]]"
published: 2023-05-14
created: 2026-04-15
description: "CFTC RULE 4.41 – HYPOTHETICAL OR SIMULATED PERFORMANCE RESULTS HAVE CERTAIN LIMITATIONS. UNLIKE AN ACTUAL PERFORMANCE RECORD, SIMULATED RESULTS DO NOT REPRESENT ACTUAL TRADING. ALSO, SINCE THE TRADES"
tags:
  - "clippings"
---
![](https://www.youtube.com/watch?v=tRq1hyGGtl4)

CFTC RULE 4.41 – HYPOTHETICAL OR SIMULATED PERFORMANCE RESULTS HAVE CERTAIN LIMITATIONS. UNLIKE AN ACTUAL PERFORMANCE RECORD, SIMULATED RESULTS DO NOT REPRESENT ACTUAL TRADING. ALSO, SINCE THE TRADES HAVE NOT BEEN EXECUTED, THE RESULTS MAY HAVE UNDER-OR-OVER COMPENSATED FOR THE IMPACT, IF ANY, OF CERTAIN MARKET FACTORS, SUCH AS LACK OF LIQUIDITY. SIMULATED TRADING PROGRAMS IN GENERAL ARE ALSO SUBJECT TO THE FACT THAT THEY ARE DESIGNED WITH THE BENEFIT OF HINDSIGHT. NO REPRESENTATION IS BEING MADE THAT ANY ACCOUNT WILL OR IS LIKELY TO ACHIEVE PROFIT OR LOSSES SIMILAR TO THOSE SHOWN  
  
Trading performance displayed herein is hypothetical. Hypothetical performance results have many inherent limitations, some of which are described below. No representation is being made that any account will or is likely to achieve profits or losses similar to those shown. In fact, there are frequently sharp differences between hypothetical performance results and the actual results subsequently achieved by any particular trading program. One of the limitations of hypothetical performance trading results is that they are generally prepared with the benefit of hindsight. In addition, hypothetical trading does not involve financial risk, and no hypothetical trading record can completely account for the impact of financial risk in actual trading. For example, the ability to withstand losses or to adhere to a particular trading program in spite of trading losses are material points which can also adversely affect actual trading results. There are numerous other factors related to the markets in general or to the implementation of any specific trading program which cannot be fully accounted for in the preparation of hypothetical performance results and all of which can adversely affect actual trading results.  
  
U.S. Government Required Disclaimer – Commodity Futures Trading Commission Futures and Options trading has large potential rewards, but also large potential risk. You must be aware of the risks and be willing to accept them in order to invest in the futures and options markets. Don’t trade with money you can’t afford to lose. This is neither a solicitation nor an offer to Buy/Sell futures or options. No representation is being made that any account will or is likely to achieve profits or losses similar to those discussed on this web site. The past performance of any trading system or methodology is not necessarily indicative of future results.  
  
Trade at your own risk. The information provided here is of the nature of a general comment only and neither purports nor intends to be, specific trading advice. It has been prepared without regard to any particular person’s investment objectives, financial situation and particular needs. Information should not be considered as an offer or enticement to buy, sell or trade.  
  
You should seek appropriate advice from your broker, or licensed investment advisor, before taking any action. Past performance does not guarantee future results. Simulated performance results contain inherent limitations. Unlike actual performance records the results may under or over compensate for such factors such as lack of liquidity. No representation is being made that any account will or is likely to achieve profits or losses to those shown.  
  
The risk of loss in trading can be substantial. You should therefore carefully consider whether such trading is suitable for you in light of your financial condition.  
  
If you purchase or sell Equities, Futures, Currencies or Options you may sustain a total loss of the initial margin funds and any additional funds that you deposit with your broker to establish or maintain your position. If the market moves against your position, you may be called upon by your broker to deposit a substantial amount of additional margin funds, on short notice in order to maintain your position. If you do not provide the required funds within the prescribed time, your position may be liquidated at a loss, and you may be liable for any resulting deficit in your account.  
  
Under certain market conditions, you may find it difficult or impossible to liquidate a position. This can occur, for example, when the market makes a “limit move.” The placement of contingent orders by you, such as a “stop-loss” or “stop-limit” order, will not necessarily limit your losses to the intended amounts, since market conditions may make it impossible to execute such orders.

## Transcript

**0:06** · well welcome back books all right so we're going to be talking about my ICT Silver Bullet trade setup which is a time-based algorithmic trading model for all asset

**0:22** · classes all right before I get into it uh let's discuss ticks points and Pips and the relationship to Forex to futures for an ICT Silver Bullet trade and the minimum trade framework should be 10 points or 40 ticks for index futures or

**0:48** · indices the minimum trade framework should be 15 Pips for Forex payers for Forex Traders now an amplification of that is this framework is the best case price delivery that you expect to see not underscore not your actual trade entry to exit range so in other words if

**1:13** · everything were to be perfect and you're not trying to be perfect with your entry you're not trying to be perfect with your exit if the entirety of the move that you foresee is likely to unfold next in whatever asset class you're trading that range

**1:30** · is the framework but you're going to be looking for a trade within that framework that doesn't demand you to have the highest degree of Entry Precision or exit Precision over time you'll get better with both of those entry and exit but now using a model you want to have something that's a little bit more forgiving so for index Futures if you're

**1:52** · trading indices the minimum framework is it has to at least offer the potential for 10 points or 10 handles which is equivalent to 4 tick the same would be said for Forex the framework should be a minimum of 15 Pips for the pair you're trying to trade so if you can't work out a range move at least 15 Pips the trade is

**2:18** · probably not high probability it would be better suited to be left alone and let it pass or look look elsewhere 10 handles for indices is the same to me as 20 Pips in Forex five handles for indices is the same to me as 10 Pips in Forex so many

**2:36** · times with my tweets or comments in my videos and whatnot uh folks that reach out to me through trading view little messaging system they have there um I ignore majority of everyone that sends me messages trading I just get too many of them and the question keeps popping up recently is if I'm teaching predominantly presently at the time in 2023 in the YouTube mentorship which is Free by the way the question is if I'm looking for

**3:08** · five handles of price movement in the E mini S&amp;P what would that translate for those that are trading forx U that would be the equivalent of 10 Pips if I'm looking for 10 Handles in

**3:24** · indices or trading stock index features uh if you're a Forex Trader you would be looking for the equiv of 20 Pips in your Forex pair so that way there's the the relationship between the two these are essential Frameworks to what I deem high probability ICT silverbolt trade

**3:47** · setups all right so let's talk about this is really the gem of this presentation really uh types of ICT Silver Bullet setups now the framework for many ICT Silver Bullet setups are as follows but they're not limited to previous day high or low draw on

**4:06** · liquidity meaning yesterday's high if we're bullish there's going to be buy stops or buy side liquidity resting above that we would be looking for a run to previous day's high that expansion is the draw in liquidity for buy side uh vice versa if we are bearish we're expecting lower prices throughout the week and we see the previous days low as having sells

**4:32** · side liquidity or self stops below it so we would look for potential setups that would expand down into that liquidity previous session highs and lows as draws on liquidity meaning that let's say you're sitting down in front of the charts and it's the am session in New York you would look at the high end or low of the London session that just passed and looked to a run on liquidity

**4:58** · or retest of those old lows or highs previous weekly high or low as a draw in liquidity if we're bullish we would look for a run above the previous week's high or if we bearish we would look for a run below the previous week's low another would be returning to a current or old new week opening Gap so that would be treated as a draw on liquidity or an expansion away from the current or old new week opening Gap

**5:31** · and a classic ICT optimal trade entry which has been for the longest time while doing this YouTube channel that's always been the classic Flagship pattern but now we've seen many more models and approaches so it can't be referred to as the flagship pattern anymore I think the fair value Gap has uh taken the throne there Confluence of the 2022 ICT

**5:55** · mentorship YouTube model which I taught for free on this YouTube channel uh me meaning that your draw on liquidity could be a inefficiency above the marketplace when we're bullish or a inefficiency below the price when we're bearish which means that if we're bearish we could be aiming for a discount buy c b sell sign efficiency or

**6:14** · some measure of fair value Gap that would be below current price action that would be your draw when bearish or if you're bullish you would be looking for a inefficiency above current price action which would be many times in the form of a civvy or sell side imbalance buy s def efficiency or variant of fair value Gap above current price action so you can treat that or as I mentioned all the previous ones above number seven here all of them being equally available

**6:41** · in terms of probability if it is in the Market at the time not all of these are going to be a factor you there will be times where the previous week's High has already been rated that morning and looking at it

**6:57** · again may not be the ideal scenario so it might require you to look at a higher time frame liquidity pool or inefficiency above price if you know if you're if you're bullish so I could list a myriad of different scenarios but I think this list is good enough to give the students of my YouTube channel a great deal of latitude so that way you can look at

**7:23** · the potential for any one of these situations not all of them will exist on any given day not all of these will be in the charts but most days one of these criteria will be in play don't take my word before I go back through your price action you'll see what I'm saying here is in fact truth obviously the main emphasis is determining the next most likely draw in

**7:48** · the price action so where is Price likely to go to next that's the number one goal for all of my students is to focus on that skill set first because all the entries and the exens and such that is the least important thing because if you don't know where price is trying to go to from the time you're sitting in looking at your charts whatever anoun this concept you use is probably going to fail

**8:13** · you all right let's talk about our first ICT Silver Bullet setup and the time at which it forms now again this is a Time based model that means these things are linked to a specific 60-minute interval

**8:30** · or window in time every single trading day this pattern will form it may not be in the Forex Peri that you're trading it may not be in the Futures Contract that you're trading it may not be in the asset that you specifically looking at but it does form every single

**8:50** · day first setup time is 3:00 a.m. to 4:00 a.m. now we're always referring to New York local time so whenever ever I'm referring to a specific time whether it be a window of time or a very specific time of the day you have to have your

**9:06** · charts calibrated to New York local time wherever that is whenever that is in your area if we're observing daylight savings time then you observe Daylight Saving signs that way it removes all the uncertainty the confusion whatever it is in New York that local time that's what you're using when you're charting this is the London open Silver Bullet so what we're looking for is a classic ICT fair value Gap the form between 3:00 a.m. and 400 a.m.

**9:38** · New York local time the factor that which you are going to lean heavily on is the skill set of knowing where price is going to go to okay and it's not necessarily the bias

**9:56** · you just predominantly have to consider where the next draw on liquidity is is it going to go above the marketplace for buy stops or trade into inefficiency above current price action if you're bullish in this case the market was bearish it was looking to go lower and there was an obvious sell-side liquidity pool resting below that old swing low and between 3:00 and 4 the market created a fair value Gap we had a shift in Market structure

**10:24** · below this low here so this is your classic what optimal trade entry fair value Gap here the market shows the willingness to support this idea with the bodies staying inside that Gap see that now at 4:00 a.m. it does pump one more time just above it but that's fine it would have never sto you out with the rules I teach with all of my models here especially the op trade entry the idea for this would be to look for a minimum of what Market is this

**10:57** · it's a Futures Contract set means does it offer the potential for 10 handles so from here down to here trading below this low not just to the low but to it and through it so it's it's reasonable to anticipate a potential run of 10 handles we don't require that but going short inside that fair value Gap the formation of the ICT Silver Bullet the entry is

**11:27** · taken inside of that 60-minute window between 3:00 a.m. and 4:00 a.m. it does not mean that the trade is entered and is exited in the same 60-minute window in other words your trade many times will be held over the 4:00 hour and into 5:00

**11:45** · in the morning and maybe even rolling over into the New York session opening at 7 8:00 New York local time but in this instance we would be aiming for this low and the cell side liqu resting below it so does it offer from this entry here down to here at least five handles for you to book in profit it does so the framework was

**12:09** · could it get to 10 it could do 10 we don't require that shorting into the fair value Gap covering at the old low allows for at least five handles and that's what the IC Silver Bullet is this is my actual model for my son Cameron all right the second one in our continuing list of I Silver Bullet setups is the am session now this one is focusing on the 10:00 a.m. to 11:00 a.m.

**12:44** · always New York local time and let's take a closer look at this one now okay so we are looking at the E mini S&amp;P once more and the idea is between 10:00 a.m. New York local time and 11: a.m. we wait for when the Market's

**13:04** · bearish relative equal lows they sell side resting below that we have a fair value Gap bearish fair value Gap it trades up into it between 10:00 and 11 o' we can sell short there does it offer 10 handles well from 4146 or thereabouts

**13:19** · to 4136 that range doesn't even get us down into this low let alone below that one so it obviously meets the criteria of a minimum of 10 Handles in framework it does not mean you're trying to get 10 handles it just means that it offers 10 handles so going short here collecting

**13:39** · five handles that could have been done inside of the scope of that 60-minute window not that you're trying to do that as I mentioned briefly moments ago the trade is many times held in duration longer than the window that the framework and entry is derived from so it's not a in and out within the same hour it means that you're looking for the setup to form to get you into the trade within the scope of 10:00 to 11 o' near y local

**14:11** · time all right and finally we have our last ICT Silver Bullet here which is framed on 2:00 p.m. to 300 p.m. New York local time and this is the PM session ICT Silver Bullet

**14:26** · setup in this one here we can see that we traded down into a higher time frame 15minute discount fair value Gap and you're encouraged to go into your charts and see that is in fact what we have here Market trades down into it shifts higher a swing has been broken to the upside so we have a shift in Market structure and a fair value Gap so any

**14:48** · retracements back down into that look at the bodies staying inside that the Wicks do the damage but the body's telling you the narrative the story is told by the bodies so it's telling you it's respecting this body balance efficiency or fair value Gap going into 2:00 we

**15:04** · rallied and we created a small little fair value Gap there the market drops down into that before taking out the relative equal highs buy side liquidity and or returning back to a premium sell side and balance buy side and efficiency or fair value Gap that would be above the market here and here so if it's going to Rally here the framework could be on the optimal trade entry here and taking the first fair value Gap that forms inside of and reprices to between 2:00 and 3:00 that's happening right there so from here all the way up to

**15:38** · here does that offer 10 handles yes it's actually offering 12 or more so this entry here is a high probability condition that lends well to a run into inefficiency in the premium and to take bide out as well so

**15:54** · that is a very handsome run there and trading between 2:00 and 3:00 now some closing thoughts if you're new to my channel and you're seeing this you don't have enough to trade this pattern so you have to back test it while you're learning how to reprice action and determine where the next draw on liquidity is going to be for the next price swing for whatever

**16:18** · asset class you're trading so don't be discouraged if it seems like it's this Cherry Picked and there it is because I actually traded many of these types of setups either with calling it out on Twitter or mentioning it in passing while actually doing executions and recording it so these patterns these things form and I called a few of them real time on Twitter last week and many of you much to my uh disapproval because

**16:46** · I don't like when you take the setups as a trade setup signal I don't want you to view it like that but many of the followers on my Twitter feed actually showed that they took the trade I called out with using Silver Bullet so the pattern works it's highly highly consistent it's extremely high probability when you have all these factors in mind and they are present in price action it gives you a rule-based idea to look for a time-based model so

**17:15** · time and price is being utilized here which is where the focus of my analysis Concepts and teaching as a mentor teaching my students how to find something that repeats you can't get anything better than having a specific 60-minute window of opportunity that forms every single trading day every single trading day one of these setups are going to form now if you don't have

**17:37** · a plethora of markets to follow ideally one or two at best while you're first learning how to do it even if you grow to a point of Interest where you have a lot of markets that you're traing a lot of pairs or a lot of Futures markets and such uh you'll find that over time the longer your career will be you'll your list will will reduce down to one or two at worst maybe three if you want to be a deviant but my advice is for you to be a specialist try to focus on one market because if you can do that one of these

**18:07** · specific ICT Silver Bullet setups will form every single day meaning that if you just follow One Market just one market you can get your setups there you can make your bread and butter you can make your ends meat you'll have losing trades okay it's going to happen but by far and large you can do things with one market and if you don't get this set up in London you wait for it in the AM session if you don't get it there you wait for it in the PM session but every single Market every single trading day will offer one of these so you have to be disciplined you have to focus and

**18:38** · look for these ideas to form in price action and should you do that you'll need to look at nothing further than this you don't need to go into any other models you don't need to go into any other teachings you don't have to come back to my YouTube channel you'll never have to do any of that stuff anymore because you be independently minded and your analysis will be and Uniquely Yours you won't have to look at external sources like me or someone else to provide that to you you'll trust yourself which is a very empowering state of mind and that's always been my Target and goal with all of my students

**19:11** · so hopefully you found this one insightful and until I'll talk to you next time be safe