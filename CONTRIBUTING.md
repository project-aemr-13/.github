# Contributing

Default contribution guidelines for NextProject13 repositories. Individual repos may
override these with their own `CONTRIBUTING.md`.

## Branching

- Branch from `staging` using `feature/<name>` or `bugfix/<name>`.
- Open pull requests against `staging`. `main` is the production branch and stays in sync
  with `staging` (no version skew).
- Production is updated only by merging the `staging` → `main` release PR. Urgent fixes may
  go straight to `main` from a `hotfix/<name>` branch; nothing else targets `main`.
- Repositories without a `staging` branch use `main` only: branch from `main` and open
  pull requests against `main`.

## Commits

- Follow [Conventional Commits](https://www.conventionalcommits.org/):
  `feat(scope): …`, `fix(scope): …`, `chore: …`, `docs: …`.
- Use a service or area scope where it applies, e.g. `feat(dpm): …`, `fix(frontend): …`.

## Pull requests

- Keep PRs focused and as small as the change allows.
- Make sure CI (lint, build, tests) passes before requesting review.
- Fill out the pull-request template.
- Self-review the diff before assigning reviewers.

## Internal conventions

Port ranges, deployment, and other internal conventions are documented for members in the
private [`.github-private`](https://github.com/project-aemr-13/.github-private) repo.
