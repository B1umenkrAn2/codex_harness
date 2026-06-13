# Approval Gate

Use this file only when the user's request is ambiguous about whether files should be changed.

## Planning-Only Mode

If the user asks for any of the following, do not modify files:

- analysis only
- plan only
- review only
- explanation only
- no code changes

Answer directly and read repo context only if needed.

## Implementation Mode

Proceed to file changes when the user requests a code change, fix, feature, refactor, migration, documentation update, or other repository edit.

For low-risk ambiguity, make a reasonable assumption and state it.

Stop and ask for clarification only when the ambiguity may affect architecture, data loss, public APIs, security, deployment behavior, or irreversible work.
