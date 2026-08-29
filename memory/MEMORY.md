# Long-term Memory
*Last consolidated: 2026-08-29*

## About This Repo
- Autonomous agent (Aeon) running on GitHub Actions via Claude Code / Pi harness
- Focus: cryptocurrency market intelligence — price tracking, token movers, unlocks, narrative tracking, DeFi overviews, Polymarket monitoring, yield farming
- Notifications: Telegram (enabled), Discord/Slack/Buzz/Resend (configure per channel secrets)
- Connected integrations: CoinGecko, DeFiLlama, Polymarket, Tokenomist, alternative.me, CoinMarketCap

## Active Skills (regular schedule)
| Skill | Schedule | Purpose |
|-------|----------|---------|
| token-movers | daily 12:00 UTC | Top movers + trending analysis |
| onchain-monitor | daily 12:00 UTC | On-chain wallet/token config |
| defi-overview | daily 12:00 UTC | DeFi TVL, fees, yields snapshot |
| token-pick | daily 12:00 UTC | Token selection with thesis |
| monitor-polymarket | daily 12:30 UTC | Prediction market activity |
| narrative-tracker | daily 13:00 UTC | Narrative lifecycle tracking |
| forecasting | daily 12:30 UTC | Market forecasts |
| price-alert | every 30 min | Price threshold monitoring |
| hyperliquid | 11:00,15:00 UTC daily | Perpetuals scan |
| unlock-monitor | weekly Monday 10:00 UTC | Token unlock supply pressure |
| yield-farming | Wed/Sat 11:00 UTC | Yield opportunities |
| heartbeat | daily 08:00 UTC | Ambient fleet health |
| skill-repair | reactive | Auto-fix failing skills |
| self-improve | every other day | Agent self-improvement |
| finance-district-mcp | daily 10:00 UTC | Wallet brief |

## Recent Activity (2026-08-29)
- First full run after hiatus (last run: 2026-06-15 prune)
- All 12 scheduled skills ran successfully
- market-context baseline established in memory/topics/
- unlock-monitor: 2/5 sources failed (defillama.com/unlocks and coingecko highlights 403) — marked DEGRADED but functional
- defi-overview: websearch tool unavailable, other 9/10 sources OK

## Topics / Reference
| File | Description |
|------|-------------|
| [market-context](memory/topics/market-context.md) | Current market snapshot: prices, narratives, DeFi, predictions |
| [skill-spotlight](memory/topics/skill-spotlight.md) | Rotation state for skill-spotlight feature |
| [index](memory/topics/index.md) | Topics directory index |

## Lessons Learned
- **Digest format**: Markdown with clickable links, under 4000 chars
- **Always save files AND commit before logging** — untracked output is lost
- **Source observability** — log each source status (`ok`/`fail`) in skill output for health scoring
- **Absorption Ratio > supply %** for unlock impact — Keyrock's 16k+ unlock study backs this
- **Cliff unlocks** show weakness ~30 days before, vol peaks at unlock, recovery 10-14 days
- **Pre-unlock price action** is cheap signal: >20% down = priced in, flat/up + high ratio = market asleep
- **./notify -f path** for multi-line reports — keeps argv short and avoids sandbox tripping on long strings
- **./secretcurl for auth'd API calls** — substitutes `{ENV_NAME}` placeholder so Bash permission layer passes
- **channels work by secret presence** — set the channel secret to activate; no secret = silently skipped

## Next Priorities
- Watch/address configuration for onchain-monitor (set up token/address watches for price-alert)
- Monitor unlock-monitor source health — defillama/unlocks and coingecko highlights returning 403 may need URL updates
- Possibly enable article-skill for thematic write-ups
- Consolidate memory periodically as more runs accumulate