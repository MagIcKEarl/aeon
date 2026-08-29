ℹ️ Yield Farming Scan — 2026-08-29

## Yield Farming Landscape — 2026-08-29

**Market backdrop:** BTC $77,674 (−2%), ETH $2,437 (−2%), SOL $103 (−2%), Fear & Greed 68 (Greed). Broad risk-off today but yield markets remain liquid. DeFi TVL $286.7B.

### Yield Landscape Summary

| Chain | Best Lending APY | Top DEX APY (TVL>=$1M) | Risk Level | Best Protocol |
|-------|-----------------|----------------------|------------|--------------|
| Ethereum | 5.72% (USDG on Aave V3) | 257% (WETH-CBBTC, Aerodrome) | Low-Med | Aave V3 / Morpho Blue |
| Base | 3.48% (USDC on Aave V3) | 115% (WETH-USDC, Aerodrome) | Low-Med | Aerodrome / Aave V3 |
| Arbitrum | 3.19% (USDt on Aave V3) | 25% (WETH-USDC, Uniswap V3) | Low | Aave V3 / Compound V3 |
| Solana | 10.41% (USDC on Kamino Lend) | 126% (SOL-USDC, Orca) | Med-High | Kamino / Orca / Raydium |
| Optimism | 2.19% (USDC on Aave V3) | 170% (WETH-ZRO, Uniswap) | Med | Aave V3 |
| Polygon | 3.45% (USDT on Aave V3) | 3109% (USDC-USDT, Uniswap V4)* | Med | Aave V3 |
| Avalanche | 6.18% (USDC on Aave V4) | 5604% (WETH.E-USDC, Uniswap V4)* | Med | Aave V4 |

*\* Ultra-high APY on low-TVL volatile pools — not suitable for production farming.*

### Top 5 Picks (Risk-Adjusted)

**1. USDC Lending on Kamino Lend (Solana)**
- **APY:** 10.41% | **TVL:** $5.25M | **Score:** 4/5
- **IL risk:** None (single-asset lending)
- **Protocol risk:** Kamino is audited (OtterSec, Kudelski), battle-tested with $500M+ on Solana
- **Token risk:** USDC — blue chip stablecoin
- **$1k/mo expected:** $8.67
- **Key risk:** Solana network stability/solvency of USDC issuer
- **Exit condition:** APY drops below 5%, or Kamino TVL drops >30% in a week

**2. RLUSD / USDC Supply on Aave V3 (Ethereum)**
- **APY:** 4.99% | **TVL:** $68.9M RLUSD, + $57.2M USDC = $126M | **Score:** 4/5
- **IL risk:** None (single-asset lending)
- **Protocol risk:** Aave is the most battle-tested lending protocol, audited many times over
- **Token risk:** RLUSD (Paxos/stable) and USDC — both blue chip
- **$1k/mo expected:** $4.16
- **Key risk:** Stablecoin depeg; regulatory action
- **Exit condition:** Supply APY falls below 2.5%, or utilization spikes above 95%

**3. USDC-AERO on Aerodrome V1 (Base)**
- **APY:** 22.24% | **TVL:** $28.8M | **Score:** 3.5/5
- **IL risk:** Medium — AERO is volatile (up to −50% IL in sharp AERO moves)
- **Protocol risk:** Aerodrome is the dominant DEX on Base, forked from Velodrome — battle-tested
- **Token risk:** AERO is a blue-chip Base token but still protocol-native. 88% of yield comes from AERO emissions
- **$1k/mo expected:** $18.53
- **Key risk:** AERO token price depreciation (reward token down)
- **Exit condition:** AERO price loses >40% in a week, or emission rate drops

**4. WETH Supply on Aave V3 (Ethereum)**
- **APY:** 5.18% (isolated pool) / 1.49% (main pool) | **TVL:** $24.3M + $819.5M | **Score:** 3.5/5
- **IL risk:** None (single-asset lending)
- **Protocol risk:** Aave V3 — ultra-low
- **Token risk:** ETH — blue chip
- **$1k/mo expected:** $4.32 (isolated pool) / $1.24 (main pool)
- **Key risk:** ETH price decline (you hold the asset regardless)
- **Exit condition:** n/a — lending ETH for yield is a long-term strategy

**5. SOL-USDC on Orca (Solana)**
- **APY:** 126.52% | **TVL:** $25.1M | **Score:** 3/5
- **IL risk:** High — SOL is volatile vs USDC (potential −30-50% IL in a sharp SOL move)
- **Protocol risk:** Orca is audited, one of Solana's top DEXes
- **Token risk:** Rewards in ORCA and swap fees — ORCA is mid-cap
- **$1k/mo expected:** $105.43 (gross) / ~$50-70 after IL estimate
- **Key risk:** SOL drawdown — massive IL if SOL drops 20%+
- **Exit condition:** SOL drops below $90, or if ORCA liquidity halves

### Watch List (High Yield, High Risk)

| Pool | Chain | APY | TVL | Risk Factor |
|------|-------|-----|-----|-------------|
| WETH-CBBTC Aerodrome Slipstream | Base | 257% | $10.6M | IL risk on volatile pair; AERO emissions may be unsustainable |
| PUMP-SOL Orca | Solana | 290% | $2.7M | Memecoin reward token; extreme IL |
| USDC-NVDAC Aerodrome | Base | 338% | $1.9M | Single-asset correlated volatile (NVDAC = MicroStrategy-style leveraged BTC) |
| WETH-ZRO Uniswap V3 | OP Mainnet | 170% | $29K | Tiny TVL — one whale exit wrecks it |
| IDAI-IUSDC-IUSDT Curve | Ethereum | 121% | $1.8M | Iron Bank stablecoins — smart contract risk |

### Closed / Degen Positions to Monitor

- **Morpho Blue STEAKUSDT ($89.5M, 2.51% APY)** — large TVL but modest yield; watch for vault strategy changes
- **Aerodrome Slipstream WETH-USDC ($10.2M, 50% APY)** — stable mid-range yield, good IL-profile; set-and-forget
- **Raydium WSOL-USDC ($14M, 105% APY)** — Solana's deepest SOL-USDC pool; high yield but high IL
- **Curve CRVUSD-TBTC ($37M, 13% APY)** — btc-pegged stable vs TBTC; decent risk-adjusted yield with Curve's CRV+CVX flywheel
- **Pendle REUSD ($10.4M, 19% APY)** — yield tokenization; fixed-rate exposure. Watch the PT/YT spread
- **Compound V3 USDC Arbitrum ($3.6M, 2.75% APY)** — stable no-frills lending

### Notes & Strategy

- **Best risk-adjusted: USDC on Kamino Lend (Solana)** at 10.4% for single-asset stables. Process: deposit USDC, earn the lending APY + any KMNO incentives. No IL, pure yield.
- **For ETH holders:** Supply WETH on Aave V3 Ethereum isolated pool at 5.18% — this is the highest ETH lending rate since early 2024.
- **For LP farmers:** Aerodrome WETH-USDC on Base at 50% APY with $10M TVL is the sweet spot: decent TVL, moderate IL, Base gas costs near zero.
- **Pendle yield:** REUSD at 19.3% APY on $10.4M TVL is attractive — you're buying future yield at a discount via PT or earning boosted yield via YT.
- **Macro watch:** With Fed decision 30 days out and F&G at 68 (still Greed), crypto lending demand remains high. If sentiment turns, stablecoin yields could compress as users seek safety.

### Summary

- Fetched live yield data from DeFiLlama (17,346 pools across all chains)
- Analyzed 5,172 pools across Ethereum, Base, Arbitrum, Solana, Optimism, Polygon, and Avalanche
- Top protocols scanned: Aerodrome, Uniswap V3/V4, Curve, Balancer, Aave V3/V4, Compound V3, Morpho Blue, Kamino (Lend+Liquidity), Orca, Raydium, Pendle
- Produced ranked top-5 picks by risk-adjusted return with expected monthly returns on $1,000
- No notification sent (read-only mode — report captured as output)
- No files modified (read-only mode)
- Follow-up: nothing actionable — this is a scan and report