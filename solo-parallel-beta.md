# Task: Parallel Session Test - Beta (Solo Mode)

## Objective

This is the BETA feature of a parallel solo session test. Run alongside `solo-parallel-alpha` to test multi-session coordination.

```bash
agent-solo start solo-parallel-alpha solo-parallel-beta --auto-run
```

## Instructions

### For Coder:

1. **Create `beta-observations-coder.md`** with initial snapshot:
   - Your role: coder
   - Feature name: "beta"
   - Worktree path
   - Branch name
   - Initial timestamp
   - List of files in `.peer-sync/`

2. **Append to `beta-observations-coder.md`** each time you enter a new phase:
   - Record timestamp and phase name
   - Note any status file changes you observe

3. **Check for sibling sessions:**
   - Look for `../*-alpha*` worktrees (note if visible)
   - Do NOT access the alpha session's worktree

4. **Commit** with message: `docs: beta coder observations`

### For Reviewer:

1. **Verify coder's work:**
   - Check `beta-observations-coder.md` exists
   - Verify it contains required fields
   - Verify feature name is "beta"
   - Check for phase entries

2. **Create `beta-review.md`** documenting your review

3. **Approve** if observations are present and correct

## Important

- Do NOT overthink - just observe and document
- Do NOT access the alpha session
- Follow phase instructions exactly
