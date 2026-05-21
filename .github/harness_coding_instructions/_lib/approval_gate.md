# Approval Gate

## Planning-Only Mode

If the user asks for:

- analysis only
- plan only
- review only
- explanation only
- no code changes

then do not modify files.

## Implementation Mode

Proceed to implementation only when:

- the user requested a code change, fix, feature, refactor, migration, or documentation update
- the plan and correctness criteria are clear enough
- the required file scope is reasonably bounded

## Ambiguity

If the task is ambiguous but low-risk, make a reasonable assumption and state it.

If the ambiguity may affect architecture, data loss, public APIs, security, or deployment behavior, stop and ask for clarification.
