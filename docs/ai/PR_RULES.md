# AI PR Rules (OpenClaw / coding agent)

These rules exist to keep automated changes safe and reviewable.

## Non-negotiables

- **Never push to `develop` (or any default branch) directly.**
- All changes must go through a **Pull Request**.
- Each run uses a fresh branch named:
  - `feat/agent/YYYY-MM-DD-<slug>`

## Required PR contents

- Clear description of **what changed** and **why**.
- A short list of **commands run** (lint/test/build) and the results.
- Call out any **risks**, **unknowns**, or follow-ups.

## Quality bar

- Keep PRs small and reviewable.
- Prefer adding/adjusting tests when changing behavior.
- Do not introduce secrets. Use env vars and document them.

## Safety

- If requirements are ambiguous, stop and ask for clarification.
- If a change could be breaking, call it out explicitly in the PR.
