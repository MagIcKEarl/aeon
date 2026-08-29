# Strategy

Aeon's north-star. Every skill reads this — it's imported into `CLAUDE.md`, so it
sits in context on **every** run. Skills align their output to it: what to work on,
what to prioritise, what to flag, what to skip.

## North-star metric

Risk-adjusted, compounding edge on the markets Aeon can actually read. Signal
quality over trade count. Every run must move one of: a confirmed setup, a
de-risked position, or a sharper edge.

## Priorities

1. **BTC risk first.** BTC is the regime governor. Risk-off (red breadth, funding
   polarised like 2026-08-29) means cut exposure, not add. Don't catch falling
   knives in ETH or alts when BTC is weak.
2. **Capital-efficient setups over directional gambles.** Funding-arb carry
   (long DOT / short AZTEC-style), real yield (Kamino USDC 10.4%, Aave WETH),
   prediction-market edges (Fed no-change YES vs 43.5% hike pricing). These pay
   without betting on direction.
3. **High-beta, high-risk longs only on confirmed strength.** SPX/BRETT-style
   meme funding blowoffs + negative price = longs bleeding; avoid. TURBO-style
   (up on high OI while market red) is the profile to chase — relative strength.
4. **Supply pressure is a sell signal.** Track unlocks. $1.52B week = fade the
   pumped names near vesting (ENA +95% into unlock = exit). 
5. **Ignore concentrated/moneygrab chains.** Robinhood chain and similar where a
   handful of whales hold most of supply. Garnish filter — skip unless
   exceptional.

## Audience

Marius — technical, time-constrained, cost-first. Wants the high-signal summary,
not the raw dump. English.

## Hard constraints

- Never chase Robinhood-chain or similarly concentrated tokens.
- Stay capital-preservation-first: no sizing into thin, illiquid mcap.
- Never let a narrative (RWA, AI, Quantum) override on-chain funding and breadth.
- Stay within spend budget — no runaway model cost (OpenRouter harness, lean runs).
- Flag anything needing a decision immediately; don't sit on signal.

## Edge to defend

- **Reads:** funding polarisation (Hyperliquid), unlock calendar, real yield,
  prediction-market mispricing, live breadth.
- **Feeds that matter:** Hyperliquid funding/OI, unlock-monitor, yield scan,
  token-movers breadth, forecast F&G, Polymarket/Kalshi edges.
- **Feeds to tune/ignore:** Robinhood-chain movers, single-whale pumps.

## Improve automatically

Each cycle: log what setups ran, their outcome, and the edge they produced.
Prune sellers, double down on what pays. Update this file monthly or when the
regime flips.