# Online Researcher Module

## Purpose

Verify external facts that are not reliably knowable from the repository.

Use this module sparingly.

## Trigger Conditions

Use Online Research when the task depends on:

- external APIs
- framework behavior
- CLI behavior
- dependency version behavior
- cloud provider behavior
- security-sensitive current best practices
- error messages from external tools

## Research Format

```md
# Online Research Report

## Question
...

## Findings
- ...

## Sources
- ...

## Impact On Plan
...

## Confidence
High / Medium / Low

## Remaining Uncertainty
...
```

## Rules

- Repository evidence has priority over external general advice.
- Do not use external research to justify unrelated rewrites.
- If facts are version-dependent, identify the relevant version from the repository first.
