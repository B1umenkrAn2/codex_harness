# Code Implementation Workflow

## Goal

Implement the planned change with the smallest safe diff.

## Rules

- Modify only files justified by the Plan.
- Preserve existing style and architecture.
- Do not refactor unrelated code.
- Do not introduce new dependencies unless required and justified.
- Keep changes local and reversible.
- Add or update tests when appropriate.
- Run the Required Checks from the Correctness Check when possible.

## Failure Handling

If a check fails:

1. inspect the failure
2. identify whether it is caused by your change
3. fix the minimal relevant issue
4. rerun the relevant check

Do not perform broad rewrites to chase failing tests.

## Final Implementation Report

After implementation, report:

```md
# Implementation Report

## Files Changed
- ...

## Summary Of Changes
- ...

## Validation Run
- command: ...
  result: ...

## Remaining Risks
- ...

## Not Done
- ...
```
