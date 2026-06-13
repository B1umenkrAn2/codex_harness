# Codex Harness Instructions

This harness is a **repo-specific thin layer**.

It should provide only durable project context, safety constraints, and a few local preferences. It should not duplicate a full coding-agent workflow such as Superpowers.

## Default Behavior

Use the active outer workflow. If `obra/superpowers` is active, follow Superpowers for general process:

- brainstorming and design approval
- implementation plans
- TDD
- subagent or inline execution
- review loops
- branch finishing

Do not also run a separate harness-level Plan / Correctness Check / Implementation / Documentation workflow.

## Conditional Files

Read these only when relevant:

- `_lib/safety_rules.md` — before file modifications, destructive commands, dependency changes, git operations, or secret-sensitive work.
- `_lib/approval_gate.md` — when it is unclear whether the user wants file changes or only analysis.
- `repo_info/STATE.md` — when durable project context is needed.
- `repo_info/KNOWN_ISSUES.md` — before non-trivial implementation, debugging, or validation work.
- `philosophy/philosophy.instructions.md` — only when local engineering preferences are ambiguous.

Do not read all of them by default.

## Coding Requests

When changing files:

1. Stay within the user's requested scope.
2. Apply the repo safety rules.
3. Prefer the smallest correct diff.
4. Validate with the narrowest relevant checks available.
5. Report exact validation commands and outcomes.

If Superpowers is active, these rules constrain the work; they do not replace Superpowers' workflow.

## Non-Coding Requests

For explanation, architecture analysis, review-only, or Q&A:

- do not modify files
- answer directly
- read repo context only if needed

## Memory Rules

Update durable repo memory only when it will help future sessions:

- `repo_info/STATE.md` for stable architecture facts, commands, conventions, or integration points.
- `repo_info/KNOWN_ISSUES.md` for real unresolved risks, flaky checks, or workarounds.

Do not duplicate Superpowers specs, plans, implementation reports, or task logs into repo memory.
