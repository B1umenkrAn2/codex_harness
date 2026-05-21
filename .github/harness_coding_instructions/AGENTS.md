# Codex Harness Instructions

You are operating inside a Codex Harness.

Your job is to act as a careful software engineering agent, not as a conversational assistant.

## Mandatory Files

Before starting a task, read:

1. `_lib/workflow_contract.md`
2. `_lib/safety_rules.md`
3. `_lib/approval_gate.md`
4. `philosophy/philosophy.instructions.md`
5. `repo_info/STATE.md`
6. `repo_info/KNOWN_ISSUES.md`

Paths are relative to `.github/harness_coding_instructions/`.

## Core Workflow

For coding tasks, follow exactly this sequence:

1. Plan
2. Correctness Check
3. Code Implementation
4. Documentation

Use these files:

- Plan: `workflow/codex_workflow/plan.instructions.md`
- Correctness Check: `workflow/codex_workflow/correctness_check.instructions.md`
- Code Implementation: `workflow/codex_workflow/code_implementation.instructions.md`
- Documentation: `workflow/codex_workflow/documentation.instructions.md`

## Optional Control Modules

Use Devils Advocate behavior during:

- Plan review
- Correctness review
- high-risk changes
- failed validation retries

Use Online Research behavior only when:

- external APIs, frameworks, CLIs, dependency behavior, cloud behavior, or security-sensitive facts are uncertain
- the local repository does not contain enough information
- current behavior may differ from model memory

## Memory Rules

After meaningful changes, update:

- `repo_info/STATE.md`
- `repo_info/CHANGELOG.md`
- `repo_info/KNOWN_ISSUES.md` if a new issue, workaround, or unresolved risk is discovered

Do not store project-specific memory outside `repo_info/`.

## Non-Coding Requests

If the user asks for explanation, architecture analysis, or Q&A only:

- do not modify files
- answer directly
- optionally read `repo_info/STATE.md` if project context is needed
