# Agent Learnings (Staging)

This file collects agent-discovered learnings for later curation into CLAUDE.md / AGENTS.md.

<!-- Entry: duo-single-feat-claude | 2026-02-14 -->
### .peer-sync phase file may lag behind orchestrator state

The `.peer-sync/phase` file may still show `work` when the orchestrator has already transitioned agents into the review phase. Rely on the skill prompts (e.g. `/duo-review`, `/duo-work`) as the authoritative phase indicator, not the `.peer-sync/phase` file alone.

### Round 1 has no prior review artifact

In Round 1, the task asks for "peer's believed workflow state from latest review" but no review exists yet. Handle this edge case explicitly rather than leaving it ambiguous.

<!-- End entry -->
