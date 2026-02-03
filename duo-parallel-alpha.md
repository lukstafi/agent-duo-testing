# Task: Parallel Session Test - Alpha (Duo Mode)

## Objective

This is the ALPHA feature of a parallel session test. Run alongside `duo-parallel-beta` to test multi-session coordination.

```bash
agent-duo start duo-parallel-alpha duo-parallel-beta --auto-run
```

## Instructions

1. **Create `alpha-observations-{agent}.md`** with initial snapshot:
   - Your agent name
   - Feature name: "alpha"
   - Worktree path
   - Branch name
   - Initial timestamp
   - List of files in `.peer-sync/`

2. **Append to `alpha-observations-{agent}.md`** each time you enter a new phase:
   - Record timestamp and phase name
   - Note any status file changes you observe
   - Keep appending throughout the session

3. **Check for sibling sessions:**
   - Look for `../*-beta-*` worktrees (note if visible)
   - Do NOT access the beta session's worktrees

4. **Commit observations** with message: `docs: alpha observations - {agent}`

5. **Create PR** when instructed

## Important

- Do NOT overthink - just observe and document
- Do NOT access the beta session
- Follow phase instructions exactly
