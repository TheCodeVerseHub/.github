# TheCodeVerseHub `.github`

This repository powers **organization-wide defaults** for TheCodeVerseHub on GitHub.

GitHub automatically uses certain files from this repo to provide consistent:

- Contribution guidelines
- Security policy
- Code of Conduct
- Pull request template
- Issue templates

## What’s inside

- `CONTRIBUTING.md` — default contributing guide for all repos
- `SECURITY.md` — default vulnerability reporting policy
- `CODE_OF_CONDUCT.md` — default community behavior expectations
- `PULL_REQUEST_TEMPLATE.md` — default PR template
- `.github/ISSUE_TEMPLATE/` — issue forms (bug report, feature request)
- `profile/README.md` — the organization profile page content

## How GitHub uses this repo

- If an individual repository **does not** define its own `CONTRIBUTING.md`, `SECURITY.md`, etc., GitHub will fall back to the versions in this repo.
- If a repository **does** define its own files, the repo-specific ones take precedence.

## When to edit this repo

Edit this repo when you want to change org-wide defaults, for example:

- Update the security contact email
- Adjust the PR checklist
- Improve issue intake quality (bug report / feature request)

## For maintainers

- Keep these templates **generic** and repo-agnostic.
- Put repo-specific setup/testing instructions in each repository’s `README.md` and/or `docs/`.

