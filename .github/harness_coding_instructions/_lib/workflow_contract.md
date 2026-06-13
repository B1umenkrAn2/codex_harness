# Lightweight Workflow Contract

Use this contract only as a fallback when no richer workflow is active.

If Superpowers is active, do not run a second harness workflow. Let Superpowers own planning, TDD, execution, review, and branch finishing. This file only adds local constraints.

## Local Constraints

- Prefer the smallest correct change.
- Do not modify unrelated files.
- Preserve existing architecture unless the task requires changing it.
- Do not introduce new dependencies unless explicitly justified.
- Do not claim correctness without evidence from repository files, command output, tests, user-provided documentation, or external research when needed.
- If uncertain, say what evidence is missing.

## Fallback Flow

For small coding tasks when no outer workflow is active:

1. Understand the requested scope.
2. Inspect only relevant files.
3. Make the minimal safe change.
4. Run the narrowest relevant validation available.
5. Report what changed, what was checked, and any remaining risk.

## Failure Handling

If validation fails:

1. inspect the failure
2. fix only the relevant cause
3. rerun the relevant check
4. stop after repeated failures and report the blocker

Do not enter an unbounded repair loop.
