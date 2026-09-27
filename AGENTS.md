# Repository instructions

## Git workflow for Linux port

- Work on the `linux-port` branch unless explicitly instructed otherwise.
- Preserve upstream compatibility whenever reasonably possible.
- Do not rewrite history.
- Do not use destructive Git commands without explicit authorization.
- At the beginning of each work pass, inspect `git status`.
- At the end of each work pass:
  1. run the relevant build/tests;
  2. inspect the resulting diff;
  3. commit all intentional changes from that pass;
  4. use a concise conventional commit message describing the actual change.
- Do not commit generated build artifacts, temporary diagnostics, binaries, `bin/`, `obj/`, logs or local secrets.
- If a pass makes no source/configuration/documentation changes, do not create an empty commit.
- Keep commits atomic enough that individual porting steps can be reverted or bisected.
- Do not push unless explicitly requested, except for the initial publication of the `linux-port` branch.
