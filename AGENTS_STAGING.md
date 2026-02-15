# Agent Learnings (Staging)

This file collects agent-discovered learnings for later curation into CLAUDE.md / AGENTS.md.

<!-- Entry: duo-single-feat-claude | 2026-02-15 -->
### peer-sync phase file may lag behind actual workflow phase

The `.peer-sync/phase` file reflects orchestrator state and may not update instantly when agents transition between work and review phases. Agents should rely on the phase communicated via `/duo-work` or `/duo-review` commands rather than polling the phase file for real-time status.

### Task wording assumes prior review exists in Round 1

If a task references "the state the peer believed to be in during latest review," Round 1 has no prior review to reference. Handle this by noting "no review yet" rather than treating it as an error.

<!-- End entry -->
