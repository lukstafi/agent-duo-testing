# Task: Observe and Document Your Environment (Solo Mode - Single Task)

## Objective

Document what you observe about your working environment. This is a meta-task to test agent-solo coordination between coder and reviewer roles.

## Instructions

### For Coder:

1. **Observe your environment:**
   - What is your worktree path?
   - What branch are you on?
   - What files exist in `.peer-sync/`?
   - What is your role (coder)?

2. **Create a file `observations-coder.md`** in the repo root containing:
   - Your role name
   - Current timestamp
   - Working directory path
   - Branch name
   - List of files in `.peer-sync/`
   - Any status files you can read

3. **Commit your observations** with message: `docs: add observations from coder`

4. **Signal completion** and proceed through the workflow phases as instructed.

### For Reviewer:

1. When reviewing, check:
   - Does `observations-coder.md` exist?
   - Does it contain the required information?
   - Are the observations accurate?

2. **Create `review-notes.md`** documenting what you checked

3. Approve if observations are present; request changes only if file is missing

## Important

- Do NOT overthink this task
- Do NOT write any code
- Just document what you see and follow the phase instructions
- Create a PR when prompted
