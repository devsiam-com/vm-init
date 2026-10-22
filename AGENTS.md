# AGENTS.md — vm-init

Public kit repo: one-command setup scripts for fresh Linux, macOS and Windows machines. Read `README.md` first.
Full standard: https://github.com/devsiam-com/.github/blob/main/docs/github-standard.md

## Git
- Never push directly to `main`. Every change goes through a PR. Squash merge only; Post merges.
- Branch: `<type>/<monday-id>-<slug>` (types: feat, fix, infra, docs, chore, hotfix).
- Commits: Conventional Commits, `type(scope): summary`.
- Releases: SemVer tags `vX.Y.Z` only.
- CI must be green before merge. Run `pre-commit run --all-files` (shellcheck, shfmt) before pushing.

## Secrets
- This repo is public. Never commit secrets, `.env`, keys, tokens, client data, hostnames or IP addresses.
- Scripts must not embed credentials; read them from the environment or prompt the user.

## Scripts
- Keep `install.sh` / `install.ps1` and `verify.sh` / `verify.ps1` in sync when adding a tool.
- Pin tool and action versions where possible; never use `latest`.
