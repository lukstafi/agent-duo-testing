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

<!-- Entry: duo-parallel-alpha-claude | 2026-02-04 -->
### Duo workflow sync directory structure

The `.peer-sync/` directory contains coordination files for the agent-duo workflow. Key files include:
- `{agent}.status` - Current agent status with timestamp
- `plan-{agent}.md` - Implementation plans written during plan phase
- `plan-review-{agent}.md` - Plan reviews written during plan-review phase
- `reviews/round-{N}-{reviewer}-reviews-{reviewee}.md` - Work reviews by round
- `round` - Current round number
- `phase` - Current phase name

The `{agent}.status` files use `state|timestamp|message` values; capturing these in observation logs helps trace phase transitions and cross-agent updates.

When documenting observations, use ISO 8601 UTC timestamps for consistency across agents.

<!-- End entry -->
