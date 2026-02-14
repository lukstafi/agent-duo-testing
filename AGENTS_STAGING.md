# Agent Learnings (Staging)

This file collects agent-discovered learnings for later curation into CLAUDE.md / AGENTS.md.

<!-- Entry: duo-single-feat-claude | 2026-02-14 -->
### Peer-sync directory structure and review file conventions

- The `.peer-sync/` directory uses pipe-delimited status files (e.g., `working|<timestamp>|<description>`) -- parse accordingly.
- Review files follow the naming convention `round-{N}-{reviewer}-reviews-{reviewee}.md` in `.peer-sync/reviews/`.
- The `agent-duo signal` and `agent-duo peer-status` commands are the primary coordination interface; avoid modifying `.peer-sync/` files directly.
- Peer worktrees are read-only -- use `git -C <peer-worktree>` commands to inspect peer progress without touching their files.

<!-- End entry -->


<!-- Entry: duo-single-feat-codex | 2026-02-14 -->
### Use .peer-sync as the source of truth for duo phase state

In agent-duo runs, read `.peer-sync` files (`phase`, `round`, `mode`, agent status, and `reviews/`) before acting. Workflow steps and allowed edits can change by round, so phase/round checks should gate whether you write files.

<!-- End entry -->
