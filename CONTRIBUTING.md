# Contributing to homebrew-osf

This repository is the Homebrew tap for OSF CLI Go. Contributions should keep installation metadata, release URLs, platform selection and checksums consistent with verified upstream release artifacts.

## Before you start

Read [README.md](README.md) and the formula under [Formula](Formula). Check existing pull requests and the corresponding release in the OSF CLI Go repository before proposing a version update. Keep application source changes in the application repository and tap changes focused on distribution.

For bugs, provide the affected version or commit, environment, minimal reproduction, expected result and observed result. For a substantial proposal, describe the use case and compatibility impact before expanding implementation scope. Use existing issue templates when offered.

## Development and validation

The README documents the installation smoke path:

```sh
brew tap edithatogo/osf
brew install osf-cli-go
osf --version
```

Use a disposable or appropriate development installation and record the operating system, architecture and version actually installed. Do not report untested platforms as verified. For formula edits, use the relevant Homebrew validation available in your environment and record its exact command and result; this repository does not document a separate full test suite.

Verify each download URL and SHA-256 against the selected immutable release artifact. Preserve supported architecture mappings and explain any removed platform. A matching checksum establishes the downloaded bytes, not an independent source audit. Version changes should identify the release and include installation or upgrade evidence where available. Preserve the application's release and signing boundaries rather than producing replacement binaries through the tap.

## Pull requests

Create a focused branch from the current `main` branch and submit a pull request to this repository. Link the relevant issue or existing project task, explain the resulting behaviour, and update affected examples and documentation. Keep unrelated changes in separate pull requests.

Report executed commands, outcomes and the commit they validate. Identify unavailable checks and remaining limitations explicitly. Follow the repository's existing review and automated-check requirements; retain required gates and current ownership. Address findings and verify the final head before integration. Repository changes do not themselves authorise a release or external operational action.

## Security, rights and conduct

Follow the [security policy](https://github.com/edithatogo/.github/blob/main/SECURITY.md). Use private vulnerability reporting if available; otherwise request a private contact without publishing vulnerability details. Keep credentials, personal information and restricted source material out of issues, fixtures, logs and artifacts.

Preserve existing attribution and third-party terms. This guide does not grant a licence; clarify any unclear redistribution rights before contributing external material. Follow the [code of conduct](https://github.com/edithatogo/.github/blob/main/CODE_OF_CONDUCT.md) and keep technical discussions respectful.

## Basis for this guide

This guide follows [GitHub's contribution-guideline guidance](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors) and the contribution-process and testing principles in [OpenSSF Best Practices](https://www.bestpractices.dev/en/criteria). It does not assert certification.
