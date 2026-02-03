# Task: Parallel Session Test - Beta (Duo Mode)

## Objective

This is the BETA feature of a parallel session test. Run alongside `duo-parallel-alpha` to test multi-session coordination.

```bash
agent-duo start duo-parallel-alpha duo-parallel-beta --auto-run
```

## Instructions

1. **Create `beta-observations-{agent}.md`** with initial snapshot:
   - Your agent name
   - Feature name: "beta"
   - Worktree path
   - Branch name
   - Initial timestamp
   - List of files in `.peer-sync/`

2. **Append to `beta-observations-{agent}.md`** each time you enter a new phase:
   - Record timestamp and phase name
   - Note any status file changes you observe
   - Keep appending throughout the session

3. **Check for sibling sessions:**
   - Look for `../*-alpha-*` worktrees (note if visible)
   - Do NOT access the alpha session's worktrees

4. **Commit observations** with message: `docs: beta observations - {agent}`

5. **Create PR** when instructed

## Important

- Do NOT overthink - just observe and document
- Do NOT access the alpha session
- Follow phase instructions exactly
