Done. Since `memory/on-chain-watches.yml` doesn't exist (no watches configured) and the `add-address` force-reply prompt was already offered earlier today (per `memory/logs/2026-08-29.md`), the dedup rule applied — the prompt was not re-sent. I logged `ON_CHAIN_NO_CONFIG` in the log and exited cleanly with no alert.

**Summary:**
- Read `memory/on-chain-watches.yml` → missing (no config)
- Checked dedup: `add-address` force-reply offered earlier today → skip reprompt
- Logged `ON_CHAIN_NO_CONFIG` status under `### onchain-monitor` in `memory/logs/2026-08-29.md`
- Exited cleanly — no alert sent, no notification fired
