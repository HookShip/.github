# Contributing to HookShip

Thank you for helping improve HookShip. The project is in pre-release
development, so interfaces and repository structure may change.

## Choose the right repository

Read the [repository placement policy](https://github.com/HookShip/.github/blob/main/REPOSITORY_PLACEMENT.md):

- use [`toolkit`](https://github.com/HookShip/toolkit) for public libraries,
  contracts, CLI, and adapter primitives;
- use [`hook-service`](https://github.com/HookShip/hook-service) for the public
  self-hostable reference service;
- use [`.github`](https://github.com/HookShip/.github) for organization-wide
  profile and community files;
- use [`platform`](https://github.com/HookShip/platform) for private managed
  control-plane work, if you have access.

Local contribution guidance in a repository overrides this shared document.

## Before opening an issue

1. Search existing issues.
2. Confirm the issue belongs in that repository.
3. Include the smallest reproducible example, expected behavior, actual
   behavior, and relevant environment details.
4. Remove secrets, credentials, private payloads, and personal data.

Do not disclose vulnerabilities in a public issue. Follow the
[security policy](https://github.com/HookShip/.github/blob/main/SECURITY.md).

## Pull requests

- Keep each pull request focused on one coherent change.
- Explain the problem, the approach, and any compatibility implications.
- Add or update tests and documentation when applicable.
- Describe how you validated the change without assuming shared commands across
  repositories.
- Link related issues when available.

By participating, you agree to follow the
[Code of Conduct](https://github.com/HookShip/.github/blob/main/CODE_OF_CONDUCT.md).
