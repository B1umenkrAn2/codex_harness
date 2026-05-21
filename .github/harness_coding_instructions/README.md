# Codex Repo Harness

This is a trimmed repo-bound Codex harness.

## How Codex Loads It

Codex discovers the root `AGENTS.md` file. That root file instructs Codex to read this harness directory.

## Core Workflow

1. Plan
2. Correctness Check
3. Code Implementation
4. Documentation

## Directory Roles

- `AGENTS.md`: harness-level controller
- `_lib/`: shared safety and workflow contracts
- `philosophy/`: engineering behavior principles
- `workflow/codex_workflow/`: Codex-specific workflow instructions
- `modules/`: optional control modules such as Devils Advocate and Online Researcher
- `request_template/`: optional human/Hermes task input templates
- `repo_info/`: project-specific memory files
