# e2e

This directory contains end-to-end (E2E) tests that validate the system from a user perspective.

## Contents

- **Test suites** – scenario-based tests covering critical user journeys
- **Page objects / helpers** – reusable abstractions over UI or API interactions
- **Fixtures & seed data** – test data required to set up scenarios
- **Reports** – generated test reports and screenshots (excluded from version control)

## Running the tests

```bash
# Install dependencies
npm install

# Run all E2E tests against the staging environment
npm test

# Run a specific suite
npm test -- --grep "checkout flow"
```

## Conventions

- Tests are written from the end-user's point of view – avoid testing implementation details.
- Each test must be independent and clean up after itself.
- Flaky tests must be fixed or quarantined immediately to keep the suite reliable.
- Screenshots and videos on failure are saved to `reports/` (git-ignored).
