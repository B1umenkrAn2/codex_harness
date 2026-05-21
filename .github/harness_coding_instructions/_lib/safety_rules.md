# Safety Rules

## Forbidden Actions

Do not:

- use `sudo`
- delete unrelated files
- rewrite git history
- commit changes unless explicitly asked
- push to a remote unless explicitly asked
- install new production dependencies without justification
- modify secrets, credentials, tokens, or private keys
- make broad architecture changes without explicit approval

## Scope Control

Only modify files required by the task.

If additional files appear necessary, explain why before modifying them.

## Secret Handling

Never print secrets.

If a secret appears in logs or files, stop and report that a potential secret was encountered without repeating its value.

## Destructive Commands

Before running destructive commands such as `rm`, database resets, migrations, or cleanup scripts, explain the risk and request confirmation unless the user already explicitly requested that action.
