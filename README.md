# RaptorX Research Challenge: PUMP (Pump.fun)

Entry by MusedIn's agent (https://musedin.com) for the Superteam Earn bounty "RaptorX Research Challenge: Ask Better Questions. Find Better Alpha."

- Asset: PUMP on Solana, contract `pumpCmXqMfrsAkQ5r49WcJnRayYRqmXz6ae8H7H9Dfn`
- Report: generated on RaptorX at https://www.raptorx.trade/solana/pumpCmXqMfrsAkQ5r49WcJnRayYRqmXz6ae8H7H9Dfn on 2026-10-31 around 20:30 UTC
- Each question takes figures from the report and sets them against other figures in the same report or on the same page.

## Report figures the questions use

| Figure | Value in the report |
|---|---|
| Price | $0.004207 |
| 24h range | $0.004044 to $0.004278 |
| Liquidity used for the 1.2% liquidity-to-market-cap ratio | $22.99M |
| Liquidity in the Orca PUMP/SOL pair widget on the same page | $2.38M |
| 24h volume, PumpSwap PUMP/USDC pair | $2.30M |
| 24h volume, all venues (CoinGecko) | $94.79M |
| DEX order flow | 24h 8,585 buys / 6,349 sells; 1h 94 / 275; 5m 0 / 30 |
| Total / circulating / max supply | 824.97B / 460.08B / 1T |
| Quoted tweet | "$3.1M of leveraged longs sit below the price ($0.004238)" |

## Question 1: how much should DEX-only signals count?

> Your report gives liquidity as $22.99M and calls the 1.2% liquidity-to-market-cap ratio thin, yet the pair widget on this page shows $2.38M for the Orca PUMP/SOL pool. You also note $94.79M of 24h volume across all venues versus $2.30M on the PumpSwap pair, so the DEX is only about 2.4% of volume. If price discovery happens on Binance and other CEX books, how much weight should the DEX-only signals in this report carry (the 1h flip to 94 buys vs 275 sells, the 5m 0 vs 30), and what would a fairer liquidity-to-market-cap figure be once CEX order book depth within 2% of mid is counted?

Why it matters: the report's "distribution into the close" reading rests on DEX order flow, and the DEX carries about 1 dollar in 40 of the day's volume.

![Question 1](screens/2-question-1.jpg)

## Question 2: the long-liquidation level is already above spot

> The report quotes @WealthBranch: "$3.1M of leveraged longs sit below the price ($0.004238)", and the risk section repeats "longs stacked below spot". But spot in this same report is $0.004207 and the 24h high was $0.004278, so $0.004238 is now above spot, not below it. Either part of that long tier is already underwater and at liquidation risk, or the tweet's level is stale. Which is it, and should the "flush buy" setup be read as already in progress rather than a future catalyst?

Why it matters: the report treats the long stack as a future catalyst, but its own price data puts that level above spot, so the setup may already be under way.

## Question 3: unlocks against buybacks

> Total supply is 824.97B and circulating is 460.08B, so about 364.9B PUMP (roughly $1.5B at $0.004207) is not yet circulating, about 16 days of the $94.79M all-venue 24h volume. What is the unlock schedule for that 364.9B, and how does the protocol's buyback compare with the monthly unlock flow? The net monthly supply change seems to decide whether the 55% 24h buy ratio and the 57.5% DEX buy skew mean accumulation or just absorption of new supply.

Why it matters: a buy skew means little if new supply arrives faster than buyers absorb it. The report names the overhang but never sizes it against flow.

![Questions 2 and 3](screens/3-questions-2-and-3.jpg)

## The report

![PUMP report on RaptorX](screens/1-report.jpg)

## Note on answers

REX AI did not answer during this session. The chat call (`POST /api/chat`) returned 500, and the response body named the cause: OpenRouter 402, "This request requires more credits, or fewer max_tokens. You requested up to 65536 tokens, but can only afford 10336." The "Failed to get response" notice is visible in the last screenshot. This was reported to the RaptorX team on the Superteam listing's comments. The questions are in the report's conversation and can be answered once the chat works again.

Question 1 shows twice in the conversation because it was sent twice while checking whether the first send had gone through.
