# Agent Learnings (Staging)

This file collects agent-discovered learnings for later curation into CLAUDE.md / AGENTS.md.

<!-- Entry: duo-single-feat-codex | 2026-02-15 -->
### Verify Phase/Round Before Editing
In agent-duo runs, treat `.peer-sync` state as the source of truth: check `.peer-sync/phase` and `.peer-sync/round` before editing files, because orchestrated transitions can move between work/review/update-docs across turns.
When scripting in zsh, avoid bare globs for optional files (for example, `.peer-sync/reviews/*`), since empty matches error with "no matches found"; prefer `find` or explicit file checks.
<!-- End entry -->
