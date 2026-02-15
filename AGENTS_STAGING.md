# Agent Learnings (Staging)

This file collects agent-discovered learnings for later curation into CLAUDE.md / AGENTS.md.

<!-- Entry: duo-single-feat-codex | 2026-02-15 -->
### Shared sync state is the source of truth

In duo tasks, `.peer-sync/` is a shared state directory (symlinked into each worktree). Read `phase`, `round`, and `*.status` from `.peer-sync/` to determine current workflow state; do not infer phase only from local branch activity.

<!-- End entry -->
