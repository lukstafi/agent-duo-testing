# Agent Learnings (Staging)

This file collects agent-discovered learnings for later curation into CLAUDE.md / AGENTS.md.

<!-- Entry: duo-single-feat-codex | 2026-02-14 -->
### Use .peer-sync as the source of truth for duo phase state

In agent-duo runs, read `.peer-sync` files (`phase`, `round`, `mode`, agent status, and `reviews/`) before acting. Workflow steps and allowed edits can change by round, so phase/round checks should gate whether you write files.

<!-- End entry -->
