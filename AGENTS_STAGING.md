# Agent Learnings (Staging)

This file collects agent-discovered learnings for later curation into CLAUDE.md / AGENTS.md.

<!-- Entry: duo-single-feat-claude | 2026-02-15 -->
### Peer-sync directory is the coordination backbone

The `.peer-sync/` directory contains all orchestration state: `phase`, `round`, per-agent status files (`<name>.status`), review files in `reviews/`, and configuration flags (`auto-finish`, `plan-mode`, etc.). Read these files to orient yourself when starting a new phase or after context compaction. The `agent-duo signal` and `agent-duo peer-status` CLI commands are the primary interaction points.

<!-- End entry -->
