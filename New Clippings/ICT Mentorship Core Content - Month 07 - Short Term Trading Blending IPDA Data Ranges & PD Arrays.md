---
title: "ICT Mentorship Core Content - Month 07 - Short Term Trading Blending IPDA Data Ranges & PD Arrays"
source: "https://www.youtube.com/watch?v=YV4fEF4d2wA&list=PLVgHx4Z63paYWV_3PDkYajv_oNznvK2aR&index=4"
author:
  - "[[The Inner Circle Trader]]"
published: 2022-09-28
created: 2026-05-05
description: "2017 Premium ICT Mentorship Core Content Video LecturesAudio and visuals are exactly as they were distributed in March 2017. CFTC RULE 4.41 – HYPOTHETICAL OR SIMULATED PERFORMANCE RESULTS HAVE CERT"
tags:
  - "clippings"
---
![](https://www.youtube.com/watch?v=YV4fEF4d2wA)

2017 Premium ICT Mentorship Core Content Video Lectures  
Audio and visuals are exactly as they were distributed in March 2017.  
  
CFTC RULE 4.41 – HYPOTHETICAL OR SIMULATED PERFORMANCE RESULTS HAVE CERTAIN LIMITATIONS. UNLIKE AN ACTUAL PERFORMANCE RECORD, SIMULATED RESULTS DO NOT REPRESENT ACTUAL TRADING. ALSO, SINCE THE TRADES HAVE NOT BEEN EXECUTED, THE RESULTS MAY HAVE UNDER-OR-OVER COMPENSATED FOR THE IMPACT, IF ANY, OF CERTAIN MARKET FACTORS, SUCH AS LACK OF LIQUIDITY. SIMULATED TRADING PROGRAMS IN GENERAL ARE ALSO SUBJECT TO THE FACT THAT THEY ARE DESIGNED WITH THE BENEFIT OF HINDSIGHT. NO REPRESENTATION IS BEING MADE THAT ANY ACCOUNT WILL OR IS LIKELY TO ACHIEVE PROFIT OR LOSSES SIMILAR TO THOSE SHOWN  
  
Trading performance displayed herein is hypothetical. Hypothetical performance results have many inherent limitations, some of which are described below. No representation is being made that any account will or is likely to achieve profits or losses similar to those shown. In fact, there are frequently sharp differences between hypothetical performance results and the actual results subsequently achieved by any particular trading program. One of the limitations of hypothetical performance trading results is that they are generally prepared with the benefit of hindsight. In addition, hypothetical trading does not involve financial risk, and no hypothetical trading record can completely account for the impact of financial risk in actual trading. For example, the ability to withstand losses or to adhere to a particular trading program in spite of trading losses are material points which can also adversely affect actual trading results. There are numerous other factors related to the markets in general or to the implementation of any specific trading program which cannot be fully accounted for in the preparation of hypothetical performance results and all of which can adversely affect actual trading results.  
  
U.S. Government Required Disclaimer – Commodity Futures Trading Commission Futures and Options trading has large potential rewards, but also large potential risk. You must be aware of the risks and be willing to accept them in order to invest in the futures and options markets. Don’t trade with money you can’t afford to lose. This is neither a solicitation nor an offer to Buy/Sell futures or options. No representation is being made that any account will or is likely to achieve profits or losses similar to those discussed on this web site. The past performance of any trading system or methodology is not necessarily indicative of future results.  
  
Trade at your own risk. The information provided here is of the nature of a general comment only and neither purports nor intends to be, specific trading advice. It has been prepared without regard to any particular person’s investment objectives, financial situation and particular needs. Information should not be considered as an offer or enticement to buy, sell or trade.  
  
You should seek appropriate advice from your broker, or licensed investment advisor, before taking any action. Past performance does not guarantee future results. Simulated performance results contain inherent limitations. Unlike actual performance records the results may under or over compensate for such factors such as lack of liquidity. No representation is being made that any account will or is likely to achieve profits or losses to those shown.  
  
The risk of loss in trading can be substantial. You should therefore carefully consider whether such trading is suitable for you in light of your financial condition.  
  
If you purchase or sell Equities, Futures, Currencies or Options you may sustain a total loss of the initial margin funds and any additional funds that you deposit with your broker to establish or maintain your position. If the market moves against your position, you may be called upon by your broker to deposit a substantial amount of additional margin funds, on short notice in order to maintain your position. If you do not provide the required funds within the prescribed time, your position may be liquidated at a loss, and you may be liable for any resulting deficit in your account.  
  
Under certain market conditions, you may find it difficult or impossible to liquidate a position. This can occur, for example, when the market makes a “limit move.” The placement of contingent orders by you, such as a “stop-loss” or “stop-limit” order, will not necessarily limit your losses to the intended amounts, since market conditions may make it impossible to execute such orders.

## Transcript

**0:09** · welcome back folks this is Lesson Four short-term Trading blending Gupta data ranges and PD arrays for liquidity runs

**0:26** · okay when we're looking at if the data ranges we're referring to specifically time and PD arrays are dealing specifically with price so blending the two elements together you're blending time and price theoretically if the data ranges provide you a context to look back the last 20 days the last 40 days in the last 60 days

**0:56** · As you move forward you're casting forward for a new set of 20 40 and 60 each new day you shift that range forward the look back period gives you the context of frame the PD arrays with a reference point in time the enter Bank price delivery algorithm will reach back in to data arrays

**1:23** · between the last 20 days the last 40 days and the last 60 days which data array they use or refer to is respective to the PD array in reference to price if price is in a premium Market obviously working for the market price up we would be looking for a bearish mitigation block a bearish breaker

**1:51** · liquidity void fair value Gap a bearish order block a rejection block an old high or an old low for the market price and below for a discount Market we would be looking for a bullish mitigation block a bullish breaker liquidity void

**2:16** · fair value Gap bullish order block rejection block old low or old High moving from the market price up in the order that's listed in the premium data arrays that's the order in which the algorithm will seek those respective price reference points they're not in any different order this is the order for the hierarchy in the way that they're set up there is not always a void or Gap or

**2:49** · mitigation block it may just simply need to go all the way up to a bearish order block or a rejection block and the same thing is said in opposite terms for when the Market's in a discount it's not ambiguous when we look at price in the form of the PD array Matrix

**3:11** · a good practice this is always to Simply go through your price charts and just look for where price is right now at the market price and above you okay looking back last 20 days and 40 days and 60 days which PD arrays in the form of a premium

**3:29** · Market exist again not all of these bearish or premium arrays will exist in your price there may be a selection of three or four or maybe as little as two

**3:45** · rarely we have all of them to choose from so what you're doing is you're looking back over the last 20 days and you're looking to see above us in terms of the market price what would be deemed as a premium Market the last 20 days which PD array exists in price action looking back 20 days which discount PD array exists below us

**4:14** · there may be a PD array above and or below us that's already been used by Price action for instance you know maybe a bullish order block price is already traded down into and responded and reacted accordingly and had higher prices that PD array has now been exhausted so you'd have to look for another discount PD array

**4:39** · when we refer to time and price what we're doing is we're blending both the components just like the algorithm does the algorithm has to go back a specific number of time so what we do is we break it into 20 trading days which is essentially one month 40 trading days which is essentially two months and 60 trading days which is essentially three trading months by combining both time and price we get

**5:11** · the closest thing we can arrive at in terms of what the algorithm will seek to do in terms of trading to the next level liquidity when the markets are bearish we work from a premium Market down to a discount based on whatever premium PD array discount PD array exist in your current market action when it's bearish those premium PD arrays will be your resistance points or

**5:40** · where cell signals or sell-offs will occur or new cell setups the objective for price to reach down into will be the discount PD arrays that exist in your price action we don't force the idea of any of these PD arrays they're either in the chart or they're not if there's an absence of any one of them it doesn't negate or increase or lessen

**6:10** · the validity of a ideal setup it just means that you have far less to choose from in terms of targets or setups all right let's take a look at an example we're going to use the Australian dollar this is the daily chart and the first thing you want to do is you want to break your market up in reference to time

**6:38** · so now we have the look back of 20 trading days 40 trading days and 60 trading days we can go back all the way to the 60 trading days and you can see that the lowest point with the old load noted and the highest high formed in the last 20 trading days that is our total 60-day trading range

**7:09** · splitting that market in half in reference to its old High and it's old low we can see where the premium and discount Market ranges exist if this old Woe Is violated we would have to go back and look at the old low formed in the 60-day look back period

**7:35** · the arrow delineating the the lowest low in the last 20 trading days if that is violated and traded below we would go back not to the 40 trading days because there's no lower low the next lower low or discount PD array exists in the 60-day look back and those levels are noted respectively

**8:00** · the last 40 trading days you can see the range is defined by the highest high and the lowest low in the last 20 trading days

**8:16** · so when we look at the last 20 trading days what we do is we think in terms of the PD array Matrix now what I've done here is I've overlaid the actual Matrix now you don't need to have this much information or try to have this in your price action but I'm giving you a graphic depiction on how I internalize and I interpret price action so if we see where price is right now at

**8:45** · Friday's close of the week of this recording market price is defined as Friday's close and we would be looking at the highest high and the lowest low in the last 20 trading days that's our first look back period of 20 trading days we start looking for bearish mitigation blocks in the premium range a bearish breaker liquidity void fair value Gap bearish order block rejection blocks and or on Old high or old low

**9:18** · the low market price we identify any bullish mitigation blocks a bullish breaker liquidity void a fair value Gap bullish order block rejection block or an old low and or high

**9:39** · with that in mind what I've noted is in the last 20 trading days these are the respective premium and discount PD arrays in the last 20 trading days working our way from the top down we have an old High a rejection block a bearish order block mean threshold

**10:02** · that's the three of candles the ranges of their bodies highs high and lowest low in terms of the bodies not the wicks that's the mean threshold or Midway point then we have the bearish order block and then we trade down into the discount area we see a bullish order block bullish order box mean threshold the rejection block and then finally the old blow

**10:36** · if we move down into a four hour chart you can see how these PD arrays give you much more detail you can start to see how price moves from one PD array to the next the market for the Australian dollar made a higher high on Tuesday failed to make a higher high and trade higher into a monthly range as I had

**11:02** · expected in my analysis you're going to learn that having these understandings of short-term Trading it's not required for you to know all the time exactly where the Market's going to go if you fail in your analysis it'll give you an immediate reason to maybe reverse your analysis and take the

**11:24** · trades in the opposite direction this was the case this week in our mentorship originally I was long or bullish on the Australian dollar but the expectation of a larger price move it failed to do so on Tuesday once Tuesday broke down as you'll see in the later slides in this presentation we have a lot more analysis to suggest the price was going to trade down and close the liquidity void now again this is a four hour chart so if we saw price fail on Tuesday

**11:58** · and break down lower during Tuesday we start looking for bearish ideas inside of the premium range so we look for all the premium PD arrays to start keying off all potential cell scenarios when we sell short on The Daily PD arrays in the premium range we would be looking for a lesser time frame to Target our exit

**12:28** · that would be in the form of a four hour or one hour chart the four hour here shows a clear liquidity void as outlined here price also trades back up into a

**12:43** · mitigation and breaker trades up to an Institutional price level 76.80 and while we're not necessarily needing the actual high of the week we can still take participation in the market move because we understand that the shift in order flow has now been moved to bearish so we were looking for discount PD arrays the low Market action at 76.80 we were in the premium range

**13:17** · the void closes and takes us into the discount range notice that in the Shaded green area if we further refine this into the days of the week on a four hour chart you can see how this clearly came down and closed in the liquidity void right to the PIP

**13:47** · if we add our Market maker manipulation template forming the high of the week on Tuesday trading at an old monthly weekly and or daily High liquidity pool that's what we saw on Tuesday it traded slightly above Monday's high rejected it once Tuesday broke down the likelihood that we would see lower prices was in effect why I said we could start looking for shorts at 76.80 with

**14:16** · the objective of 7605 as our downside objective that was framed as we see on our Market maker manipulation template the discount Market PD array is going to be used on a

**14:31** · time frame lesser than the premium liquidity pool that was used so the daily high on Monday was violated on Tuesday that's a liquidity pool raid on a daily High if that's the context we're going to drop down to a four hour and or a one hour chart to look for a discount PD array

**14:56** · it comes in the form of liquidity void taking us down into 7605 was our objective everything tied together we get a combination of elements of time and price blending and using the market maker manipulation templates in accordance to our market

**15:20** · profiles that we used and learned in lesson two we get a symmetry in the marketplace that would otherwise probably Escape everyone else so hopefully this is an example and understanding and using an example we used in live analysis this week while we were initially wrong and our expectation of a higher breakout on Aussie dollar that failure swing on Tuesday

**15:50** · gave us Insight on how we can change gears and get short on Aussie dollar even while it traded in sympathy with the weaker dollar which isn't typical blending the two time and price it gives

**16:06** · us the ability to work within the same parameters that the algorithm will at the interbank level hopefully this has been insightful to you we'll build more on these ideas as we go through and trade with more insights using the ifta data ranges and PD array Matrix