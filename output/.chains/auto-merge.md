Now let me provide the final summary output.

---

## Summary

**Skill executed:** auto-merge  
**Mode:** live (no dry-run override)  
**Repo(s):** `aeonfun/aeon`

### Evaluated PRs (2)

| PR | Title | Author | Verdict |
|----|-------|--------|---------|
| #983 | trust cursor workspaces in headless runs | @Svector-anu | SKIP:author-not-allowlisted:Svector-anu |
| #984 | fail hermes runs on api errors | @Svector-anu | SKIP:author-not-allowlisted:Svector-anu |

### Safety gate breakdown
Both PRs are from a human author (`Svector-anu`) not on the allowlist — only `dependabot[bot]`, `renovate[bot]`, and `github-actions[bot]` are eligible. Additionally, both are from forks (`isCrossRepository: true`), which would also fail the fork gate. All other gates passed (clean CI, main branch, no blocking reviews, no opt-out labels, within size cap, not draft, not already queued).

### Actions taken
- **Merged:** 0
- **Qualified:** 0 of 2 — all blocked on author allowlist
- **Notification sent:** No (no merges, no retry-cap hits)
- **State persisted:** `memory/topics/auto-merge-state.json` — entries created for both PRs with `attempts: 0`
- **Log written:** `memory/logs/2026-08-29.md` under `### auto-merge`

### Follow-up
- If these PRs should be auto-merged (e.g., if @Svector-anu is the operator), add a `## Trusted Authors` section to `memory/watched-repos.md` listing `Svector-anu` (or the appropriate GitHub username).
