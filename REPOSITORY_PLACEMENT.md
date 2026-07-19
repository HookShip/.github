# Repository Placement Policy

HookShip uses four repositories with distinct responsibilities. Put issues,
changes, and documentation in the repository that owns the affected behavior.

| Repository                                                 | Belongs here                                                                                                                    | Does not belong here                                                     |
| ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| [`.github`](https://github.com/HookShip/.github)           | Organization profile, shared issue and pull request templates, and community-health defaults                                    | Product code or repository-specific implementation guidance              |
| [`toolkit`](https://github.com/HookShip/toolkit)           | Public libraries, CLI, adapters, webhook contracts, validation and compatibility logic, fixtures, types, and signing primitives | Reference-service deployment or private managed-platform implementation  |
| [`hook-service`](https://github.com/HookShip/hook-service) | Portable outbound webhook delivery data plane, protocol, deployment surface, and service-specific documentation                 | General-purpose toolkit primitives or private hosted-product engineering |
| [`platform`](https://github.com/HookShip/platform)         | Private managed control-plane and hosted-product engineering                                                                    | Public foundation changes that belong in `toolkit` or `hook-service`     |

The public `toolkit` and `hook-service` repositories are pre-release and have no
public releases. The private `platform` repository is not an operated public
service.

## Issues

- Report a bug where the affected code is owned.
- Request a feature where its public interface or implementation would live.
- Use `.github` only for organization-wide community files and profile content.
- Use `platform` for private managed control-plane work if you have access.
- For cross-repository work, open the primary issue where most implementation
  belongs and link any follow-up issues in other repositories.
- Never place confidential platform details in a public repository.
- Report vulnerabilities through the affected repository's private
  vulnerability reporting flow, as described in the
  [security policy](https://github.com/HookShip/.github/blob/main/SECURITY.md).

## Changes

Keep pull requests within one repository whenever practical. If a change
requires coordinated updates, explain the dependency and link the related pull
requests without duplicating ownership.

Repository-local contribution, security, support, issue-template, and pull
request guidance overrides the shared defaults provided by `.github`.
