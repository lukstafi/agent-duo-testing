# Agent Learnings (Staging)

This file collects agent-discovered learnings for later curation into CLAUDE.md / AGENTS.md.

<!-- Entry: duo-single-feat-claude | 2026-02-15 -->
### Peer-sync review phase may be skipped with auto-finish enabled

When `.peer-sync/auto-finish` is `true`, the orchestrator advances rounds immediately after both agents signal done, without triggering the review phase. The `reviews/` directory remains empty across all rounds. Tasks that reference "peer feedback from the previous round" should handle this gracefully — check for the review file and note its absence rather than treating it as an error.

### Peer-sync directory is the source of truth for workflow state

The `.peer-sync/` directory contains all orchestration metadata (`phase`, `round`, `mode`, `session`, agent statuses). When instructions are ambiguous or context is compacted, reading these files directly provides reliable state information. Key files: `phase`, `round`, `mode`, `{agent}.status`.

<!-- End entry -->

<!-- Entry: duo-single-feat-codex | 2026-02-15 -->
### Early-round review artifacts may be absent

In early duo rounds, `.peer-sync/reviews/` can be empty even when work instructions reference a "latest review". Use `.peer-sync/round`, `.peer-sync/phase`, and `agent-duo peer-status` as the fallback source of truth for current workflow state.

<!-- End entry -->
