ℹ️ Hyperliquid Market Scan — 2026-08-29

## Hyperliquid Market Scan — 2026-08-29

Broad risk-off: BTC -2.5%, ETH -2.7%. 15/15 high-OI coins all red — bearish divergence across the board. Funding polarised: extreme positive on memes, deep negative on L1s.

### Funding Highlights

| Coin | Funding (1h) | Annualized APR | 24h Chg |
|------|-------------|---------------|---------|
| BTC  | +0.00125%   | +11.0% APR    | -2.5%  |
| ETH  | +0.00125%   | +11.0% APR    | -2.7%  |
| SOL  | +0.00125%   | +11.0% APR    | -2.5%  |
| **Most positive:** AZTEC | **+0.00582%** | **+51.0% APR** | -2.6% |
| SPX | +0.00459% | +40.2% APR | **-8.7%** |
| BRETT | +0.00458% | +40.1% APR | -5.0% |
| ZEC | +0.00389% | +34.1% APR | +0.9% |
| **Most negative:** DOT | **-0.00522%** | **-45.7% APR** | -4.0% |
| TIA | -0.00437% | -38.3% APR | -4.6% |
| MON | -0.00381% | -33.3% APR | -2.8% |

**Flagged (abs(funding) > 0.001%/h):** 140+ coins exceed threshold. BTC/ETH/majors all at +0.00125%/h base rate. Extreme outliers: AZTEC (+51% APR), SPX (+40%), DOT (-46% APR).

### Top Movers (24h)

**Gainers:**
1. NIL +16.1% (oi=21M)
2. TURBO +3.6% (oi=483M)
3. ICP +2.9% (oi=1.4M)
4. MINA +2.5% (oi=21M)
5. ZETA +2.5% (oi=34M)

**Losers:**
1. FOGO **-17.3%** (oi=59M)
2. PURR **-12.4%** (oi=99M, Hyperliquid native token)
3. STX **-9.8%** (oi=4.5M)
4. FET **-9.5%** (oi=38M)
5. JUP **-8.7%** (oi=45M)

### OI / Volume

- **BTC OI:** 36,992 BTC (~$2.87B) | depth: 4.42 BTC bid / 2.54 BTC ask @ $77,667 — tight 0.0013% spread
- **ETH OI:** 755,531 ETH (~$1.84B)
- **SOL OI:** 5.74M SOL (~$594M) | vol/OI ratio: 129x — high turnover

**OI divergence (all red):**
- PUMP: 44.9B OI, -3.0% — extreme OI for a memecoin, bearish divergence
- kPEPE: 6.4B OI, -5.0% — massive OI, negative funding (longs paying)
- ENA: 408.8M OI, -7.3% — significant OI + bearish price action
- FARTCOIN: 197M OI, -6.1% — high positive funding (31% APR), OI growing into weakness

**TURBO** is the only high-OI coin with positive price action (+3.6%, OI 483M) — bullish divergence.

### Basis / Arbitrage

Top premium/perpetual basis opportunities:

| Coin | Premium | Annualized | Funding |
|------|---------|-----------|---------|
| APEX | +0.179% | +65.5% | +0.0020% |
| BRETT | +0.121% | +44.3% | +0.00458% |
| W | -0.110% | -40.3% | -0.00139% |
| DOT | -0.106% | -38.6% | -0.00522% |
| TIA | -0.101% | -36.7% | -0.00437% |

Wide premiums suggest short-term funding/liquidation pressure rather than structural arb.

### Trade Ideas

1. **Funding arb pair: Long DOT / Short AZTEC or SPX**
   - DOT pays -45.7% APR to hold short (i.e. longs earn funding); AZTEC charges +51% APR to hold long
   - Potential carry trade: long DOT perp, short AZTEC perp → ~97% gross annualized differential
   - Risk: DOT -4% on the day, momentum unfavourable; need delta-neutral sizing

2. **Oversold bounce watch: PURR -12.4% in 24h**
   - Hyperliquid's native token, high OI (99M), cleanest L2 book
   - If BTC stabilises, mean-reversion candidates: PURR, FOGO (-17.3%)
   - Position sizing critical — low-market-cap tokens can gap

3. **Momentum: TURBO +3.6% on 483M OI (only high-OI gainer)**
   - Rallied while everything else dropped — relative strength
   - Low price ($0.001), memecoin dynamics, high volatility risk

### Risk Notes

- **Broad risk-off:** BTC -2.5% with 90%+ of altcoins in the red. Funding base rate elevated at +11% APR suggests persistent long bias.
- **kPEPE liquidation cascade risk:** 6.4B OI with -5% price and negative funding. A sharp move could trigger cascading liquidations. Monitor closely.
- **FARTCOIN & SPX warning:** Both have high positive funding (31-40% APR) while price is down. Longs are bleeding — if BTC drops further, forced selling accelerates.
- **PURR (-12.4%):** Hyperliquid spot token; large OI relative to market cap. Sharpest single-day drop suggests potential deleveraging event.
- **Liquidation cluster:** Medium conviction. BTC below $77k (currently $77,668) could accelerate the flush to $75k support — high-OI meme coins would compound the move.

## Summary

- **Source:** Hyperliquid public API
- **Data:** allMids, metaAndAssetCtxs (funding, OI, 24h vol, premiums), l2Book (BTC, DOT, AZTEC, SPX, FARTCOIN)
- **Market regime:** risk-off, broad selloff, bearish OI divergence
- **Top signal:** funding polarisation creating a rare ~97% APR differential carry opportunity (long DOT, short AZTEC/SPX)
- **Top risk:** kPEPE 6.4B OI liquidation cascade + memecoin deleveraging
- **Actionable:** funding arb pair setup; monitor PURR/FOGO for bounce entries