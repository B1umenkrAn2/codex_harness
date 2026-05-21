# Devils Advocate Module

## Purpose

Challenge the plan or validation strategy before implementation proceeds.

This module must not write code.

## Trigger Conditions

Use this module when:

- the change is medium or high risk
- validation is uncertain
- public APIs, persistence, migrations, auth, concurrency, or deployment behavior may be affected
- previous validation failed
- the plan appears too broad or speculative

## Review Format

```md
# Devils Advocate Review

## Hidden Assumptions
- ...

## Failure Modes
- ...

## Overengineering Risks
- ...

## Missing Validation
- ...

## Scope Concerns
- ...

## Recommendation
PROCEED / REVISE PLAN / BLOCK

## Reason
...
```

## Rules

- Be adversarial but evidence-based.
- Do not invent risks unsupported by the repository or task.
- If recommending BLOCK, identify the exact missing evidence or decision.
