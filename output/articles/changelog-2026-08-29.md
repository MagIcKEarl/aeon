# Changelog — Week of 2026-08-29

*Window: 2026-08-22 11:57 UTC → 2026-08-29 11:57 UTC · Sources: aeonfun/aeon=ok*

## aeonfun/aeon

> **Highlights:** Vercel's `fx` CLI joins as a 7th run-harness, a new `skill-article` skill generates receipts-first launch articles, and 9 infrastructure fixes landed — including closing a credential-argv leak and adding a Telegram webhook replay guard.

### Added

- New `skill-article` skill turns any skill in the instance into a publish-ready launch article: receipts-first headline mined from real run history, one-thesis structure, the target SKILL.md embedded verbatim. ([#945](https://github.com/aeonfun/aeon/pull/945))
- Vercel's `fx` coding agent (native Zig binary, v0.0.5) added as a 7th run-harness — full native MCP support, no OpenRouter fallback, permission-auto mode instead of --yolo. ([#941](https://github.com/aeonfun/aeon/pull/941))

### Changed

- Memory-flush bookkeeping moved from LLM-driven to deterministic `scripts/memory_prep.py` with a structured watermark file — no more silent 3-day window fallback. ([#938](https://github.com/aeonfun/aeon/pull/938))

### Fixed

- Scorer now grades the sent notify card instead of the harness `.result` summary, fixing `unverifiable_claim` score-2 on notify-first skills. ([#949](https://github.com/aeonfun/aeon/pull/949))
- Dashboard aeon.yml writes locked with an in-process mutex (`withFileLock`) so concurrent model/harness picker clicks no longer race and silently clobber each other's changes. ([#944](https://github.com/aeonfun/aeon/pull/944))
- Dashboard harness picker now actually includes `fx` — the type unions `lib/types.ts` and `lib/constants.ts` were missed when the backend harness was added. ([#943](https://github.com/aeonfun/aeon/pull/943))
- Telegram webhook now deduplicates updates by `update_id` before dispatch — so a retransmitted message or button tap never runs twice. ([#937](https://github.com/aeonfun/aeon/pull/937))
- Issue-store ensures (`state_store.sh`, `health_issue.sh`) now converge on the lowest matching issue number after creation, preventing the ledger or vote count from silently forking across duplicate issues. ([#936](https://github.com/aeonfun/aeon/pull/936))
- Secretcurl.sh substituted secrets no longer leak into curl's process argv — routed through `-K --config` on stdin instead. ([#935](https://github.com/aeonfun/aeon/pull/935))
- Skill-runner concurrency groups now scoped by target (`inputs.var`) so dispatching the same skill at different explicit targets no longer silently cancels all but the first and last. ([#934](https://github.com/aeonfun/aeon/pull/934))
- `Bash(cd:*)` now granted in skill mode permissions — compound `cd` + real-work bash calls were being silently denied, causing weeks of intermittent failures on data-fetch skills. ([#933](https://github.com/aeonfun/aeon/pull/933))
- Harness diagnostic output no longer truncated to 160–300 chars across 7 logging sites — full 4000-char dumps preserve the actual failure reason. ([#932](https://github.com/aeonfun/aeon/pull/932))

### Security

- Optional per-run egress firewall + audit via iron-proxy (opt-in): blocks link-local/cloud-metadata (SSRF class), logs every host via an allowlist proxy, and has an enforce mode. ([#947](https://github.com/aeonfun/aeon/pull/947))

*Internal: 5 commits hidden (docs sync, docs ecosystem, tests, chore images). Bots filtered: 0.*

---

## Summary

- **Repos scanned:** 1 (aeonfun/aeon)
- **User-facing changes:** 13 (0 breaking, 2 added, 1 changed, 9 fixed, 1 security)
- **Internal/bot commits filtered:** 5
- **Article saved to:** `output/articles/changelog-2026-08-29.md`