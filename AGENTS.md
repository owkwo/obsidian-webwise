# AGENTS.md

## Repository

This repository is **obsidian-webwise**, a TypeScript Obsidian-to-Supernotes integration. The repository slug is the canonical project name in documentation and release metadata.

## Working rules

- Read `README.md` and `SPEC.md` before changing behavior.
- Keep changes focused; do not bundle unrelated cleanup with a feature or fix.
- Do not commit secrets, generated dependency directories, build outputs, editor state, or local absolute paths.
- Preserve existing licenses and attribution.
- Update `README.md` and `SPEC.md` when user-visible behavior, support status, setup, or architecture changes.
- Prefer the smallest supported dependency upgrade. Major upgrades must include migration notes and validation.

## Setup

npm install

## Validation

Run the applicable commands before opening a pull request:

- `npm run build`

If a tool or platform is unavailable, record exactly what was not run and why.

## Project-specific guidance

Never commit API keys or vault data. Treat remote delete/disable operations as destructive and require explicit safeguards. Preserve the historical plugin ID unless a migration is implemented.

## Pull requests

Explain the problem, the chosen approach, user/developer impact, tests run, and remaining limitations. Keep commits reviewable and never report a check as passing unless it was executed.
