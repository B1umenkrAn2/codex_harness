# Documentation Workflow

## Goal

Update durable project memory after meaningful work.

## Required Updates

Update:

- `repo_info/CHANGELOG.md` for completed changes
- `repo_info/STATE.md` when architecture, commands, workflows, or important project facts changed
- `repo_info/KNOWN_ISSUES.md` when new issues, limitations, flaky checks, or workarounds are found

## CHANGELOG Format

```md
## YYYY-MM-DD - Short Title

### Summary
...

### Files Changed
- ...

### Validation
- ...

### Notes
...
```

## STATE Format

Keep this file concise.

Record:

- architecture facts
- important commands
- recurring conventions
- active systems
- integration points

Do not turn STATE into a verbose task log.

## KNOWN_ISSUES Format

```md
## Issue Title

- Status:
- Area:
- Symptoms:
- Workaround:
- Next Action:
```

## Rules

- Do not document noise.
- Do not duplicate the full implementation report.
- Record facts that help future Codex sessions.
