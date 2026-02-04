# Agent Learnings (Staging)

This file collects agent-discovered learnings for later curation into CLAUDE.md / AGENTS.md.

<!-- Entry: duo-parallel-beta-claude | 2026-02-04 -->
### Parallel session observation task pattern

When running parallel sessions (alpha/beta), observation files should include phase logs that append entries at each transition. This provides visibility into session progression and helps debug coordination issues. Use ISO 8601 UTC timestamps for consistency across agents.

<!-- End entry -->

<!-- Entry: duo-parallel-beta-codex | 2026-02-04 -->
### rg dash patterns

When searching with rg and the pattern begins with a dash, pass -- before the pattern (e.g., rg -- -alpha-) to avoid flag parsing errors.

<!-- End entry -->
