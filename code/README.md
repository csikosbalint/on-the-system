# code

This directory contains the source code of the system.

## Contents

- **Services / modules** – individual deployable units or libraries
- **Shared libraries** – common utilities, types, and helpers reused across services
- **Configuration** – environment-specific application configuration

## Development guidelines

- Follow the coding standards defined in each service's own README.
- Write unit and integration tests alongside the production code.
- Keep dependencies up-to-date and pin versions in lock files.
- Use feature branches and submit changes via pull requests.

## Getting started

1. Install the required runtime and toolchain for the service you are working on.
2. Copy `.env.example` to `.env` and populate the values.
3. Run `make install` (or the equivalent package-manager command) to install dependencies.
4. Run `make dev` to start a local development server.
