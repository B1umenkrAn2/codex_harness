# Workflow Contract

## Execution Contract

For every coding task, Codex must follow:

1. Plan
2. Correctness Check
3. Code Implementation
4. Documentation

Do not jump directly into implementation unless the user explicitly requests a trivial change and the change is low risk.

## Evidence Rule

Do not claim something is true unless it is supported by one of:

- repository files
- command output
- test output
- documentation explicitly provided by the user
- external research when needed

If uncertain, say so and identify the missing evidence.

## Minimal Diff Rule

Prefer the smallest correct change.

Do not:

- rewrite unrelated files
- refactor unrelated code
- rename public APIs unless required
- change formatting across untouched files
- introduce new dependencies unless explicitly justified

## Validation Rule

Before declaring the task complete:

- identify the relevant checks
- run them when possible
- report exact commands and outcomes
- if checks cannot be run, explain why

## Failure Rule

If validation fails:

1. inspect the failure
2. fix only the relevant cause
3. rerun the relevant check
4. stop after repeated failures and report the blocker

Do not enter an unbounded repair loop.
