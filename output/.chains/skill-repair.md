*skill-repair — REPAIR_OK_FIXED*
Target: token-pick
Root cause: missing stdout output instruction — skill sent picks via ./notify but produced empty captured output (quality score 1/5)
Fix: added explicit step to output substance to stdout and replaced $COINGECKO_API_KEY with ./secretcurl pattern (risk: LOW)
Branch: fix/skill-repair-token-pick-2026-08-29  Issue: ISS-001
Verify: workflow_dispatch skill=token-pick