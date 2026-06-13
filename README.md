# Codex Repo Harness

This is a trimmed repo-bound Codex harness.

It is designed to coexist with `obra/superpowers` without duplicating Superpowers' general development methodology.

## How Codex Loads It

Codex discovers the root `AGENTS.md` file. That file points to the harness controller at:

`.github/harness_coding_instructions/AGENTS.md`

The controller then explains which additional files should be read conditionally.

## Role

This harness provides:

- repo-specific safety constraints
- durable project context
- known issue memory
- lightweight fallback rules when no richer workflow is active

It does **not** provide a second mandatory Plan / Correctness Check / Implementation / Documentation workflow.

## Directory Roles

- `AGENTS.md`: root entry point
- `.github/harness_coding_instructions/AGENTS.md`: thin harness controller
- `.github/harness_coding_instructions/_lib/`: safety, approval, and fallback workflow constraints
- `.github/harness_coding_instructions/philosophy/`: local engineering preferences
- `.github/harness_coding_instructions/repo_info/`: durable project memory

## Superpowers Compatibility

When Superpowers is installed or active, let it own:

- brainstorming and design
- implementation planning
- TDD
- subagent or inline execution
- review workflows
- branch finishing

Use this harness only to add local repo constraints and context.
