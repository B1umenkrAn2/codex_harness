# Correctness Check Workflow

## Goal

Define what must remain true before implementation begins.

## Required Analysis

Identify:

- relevant tests
- build commands
- lint/typecheck commands
- integration points
- runtime risks
- backward compatibility constraints
- data or migration risks

## Output Format

```md
# Correctness Check

## Required Checks
- ...

## Optional Checks
- ...

## Invariants To Preserve
- ...

## Risk Areas
- ...

## Expected Success Criteria
- ...

## Checks That Cannot Be Run
- ...
```

## Rules

- Prefer repository-defined commands over guessed commands.
- Look for scripts in package files, Makefiles, task runners, CI config, or docs.
- Do not claim correctness without command evidence or clear reasoning.
- For high-risk changes, run a Devils Advocate review against the validation plan.
