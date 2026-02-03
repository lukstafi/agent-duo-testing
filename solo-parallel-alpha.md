# Task: Parallel Session Test - Alpha (Solo Mode)

## Objective

This is the ALPHA feature of a parallel solo session test. Run alongside `solo-parallel-beta` to test multi-session coordination.

```bash
agent-solo start solo-parallel-alpha solo-parallel-beta --auto-run
```

## Instructions

### For Coder:

1. **Create `alpha-observations-coder.md`** with initial snapshot:
   - Your role: coder
   - Feature name: "alpha"
   - Worktree path
   - Branch name
   - Initial timestamp
   - List of files in `.peer-sync/`

2. **Append to `alpha-observations-coder.md`** each time you enter a new phase:
   - Record timestamp and phase name
   - Note any status file changes you observe

3. **Check for sibling sessions:**
   - Look for `../*-beta*` worktrees (note if visible)
   - Do NOT access the beta session's worktree

4. **Commit** with message: `docs: alpha coder observations`

### For Reviewer:

1. **Verify coder's work:**
   - Check `alpha-observations-coder.md` exists
   - Verify it contains required fields
   - Verify feature name is "alpha"
   - Check for phase entries

2. **Create `alpha-review.md`** documenting your review

3. **Approve** if observations are present and correct

## Important

- Do NOT overthink - just observe and document
- Do NOT access the beta session
- Follow phase instructions exactly
