# cicd

This directory contains CI/CD pipeline definitions and automation scripts.

## Contents

- **Pipeline definitions** – workflow files for the chosen CI platform (e.g. GitHub Actions, GitLab CI)
- **Build scripts** – reusable scripts for building, testing, and packaging artefacts
- **Release automation** – versioning, changelog generation, and artefact publishing

## Pipeline overview

| Pipeline | Trigger | Purpose |
|----------|---------|---------|
| `build` | push / pull request | Compile, lint, and run unit tests |
| `integration` | merge to main | Run integration and e2e test suites |
| `release` | version tag | Build release artefacts and publish |
| `deploy` | successful release | Deploy to the target environment |

## Conventions

- Pipelines must be idempotent and reproducible.
- Secrets are stored in the CI platform's secret store – never hard-coded.
- Every pipeline step that produces an artefact should upload it for traceability.
