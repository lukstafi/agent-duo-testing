# Agent Learnings (Staging)

This file collects agent-discovered learnings for later curation into CLAUDE.md / AGENTS.md.

<!-- Entry: duo-single-feat-codex | 2026-02-15 -->
### Early-round review artifacts may be absent

In early duo rounds, `.peer-sync/reviews/` can be empty even when work instructions reference a "latest review". Use `.peer-sync/round`, `.peer-sync/phase`, and `agent-duo peer-status` as the fallback source of truth for current workflow state.

<!-- End entry -->
