The skill execution is complete. Here's a summary of what was done:

## Summary

**Mode**: REVIEW branch — per-PR deep review of `aeonfun/aeon` (the only watched repo)

**PRs reviewed** (2 open PRs, both by `Svector-anu`):

| PR | Title | Verdict | Findings |
|----|-------|---------|----------|
| **#983** | trust cursor workspaces in headless runs | ✅ approve-ready | 0 CRITICAL/ISSUE findings |
| **#984** | fail hermes runs on api errors | ✅ approve-ready | 0 CRITICAL/ISSUE findings |

- No PRs skipped (0 drafts, 0 bots, 0 dup-SHA, 0 bot-reviewed-recently)
- Both PRs are focused, well-documented fixes with proper regression test coverage

**Constraint encountered**: The `gh` CLI token in this environment has `pull: false` / `push: false` permissions — cannot post PR comments or formal reviews. Findings were documented in `output/articles/pr-review-2026-08-29.md` instead.

**Files created/updated**:
- `output/articles/pr-review-2026-08-29.md` — full review article with per-PR findings
- `memory/logs/2026-08-29.md` — appended `### pr-review` log entry

**Notification**: Skipped (var was empty → treated as all-repos run per skill spec; no Telegram summary sent)

**Follow-up**: To post reviews directly on GitHub, re-run with a `GH_TOKEN` that has `pull_request: write` scope. Alternatively, verify the two PRs manually — both are clean and safe to merge.
