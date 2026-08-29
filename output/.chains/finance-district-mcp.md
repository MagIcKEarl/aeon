⚠️ Finance District: Not Connected

### finance-district-mcp
- **Task:** daily wallet brief
- **Spent:** none
- **Result:** FD_NOT_CONNECTED — Finance District MCP server is not connected. No `mcp__finance-district__*` tools are available in this run.
- **Action needed:** Go to dashboard → MCP panel → **Connect Finance District** via OAuth (requires `offline_access` scope). The OAuth token is stored as `MCP_FINANCE_DISTRICT_TOKEN` + `MCP_FINANCE_DISTRICT_OAUTH`, and `GH_SECRETS_PAT` must be set so refresh tokens persist (see [docs/mcp-oauth.md](docs/mcp-oauth.md) for details).
- **Advisory:** Auto-approve limits, transfer caps, and a destination denylist are enforced server-side — once connected, the agent can check balances, prices, yields, and move funds within those limits.