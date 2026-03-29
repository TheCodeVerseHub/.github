# Contributing to The CodeVerse Hub

Thanks for helping build projects under the **TheCodeVerseHub** organization.
This file is the default contribution guide for all repositories in this org.

## Quick start

1. Pick a repo and read its `README` + `SECURITY` (if present).
2. Find an issue labeled **good first issue** / **help wanted** (or open a new one).
3. Fork the repo, create a branch, implement the change, open a PR.

## Ways to contribute

- Fix bugs, improve tests, refactor safely
- Write docs (setup guides, troubleshooting, architecture notes)
- Improve UX (web), config defaults (Linux), commands/features (bots)
- Triage issues: reproduce, add logs, minimal repro steps

## Project coordination

- **Issues** are the source of truth for planned work.
- If you’re starting work, comment “I’m taking this” to avoid duplication.
- For larger changes, open a short **proposal issue** first.

## Development workflow

### 1) Fork + branch naming

- Fork the repository to your account.
- Create a branch from the default branch:
  - `fix/<short-topic>`
  - `feat/<short-topic>`
  - `docs/<short-topic>`
  - `chore/<short-topic>`

Examples:

- `fix/starboard-video-preview`
- `feat/installer-preflight-checks`

### 2) Keep PRs small

- Prefer focused PRs that do one thing well.
- Large PRs should be split (or discussed before implementation).

### 3) Commit messages

Use clear, imperative messages:

- `Fix crash when config is missing`
- `Add docs for local dev setup`

### 4) Quality bar (applies to all repos)

- No secrets (tokens, `.env`, API keys) committed
- Update docs when behavior changes
- Add/adjust tests when practical
- Avoid formatting-only diffs unless required

## Repository-specific expectations

### Python bots (Eigen Bot, Miku, CodeVerse-Bot)

- Prefer `python -m venv .venv` (or the repo’s toolchain if specified)
- Keep config in environment variables (see `.env.example`)
- Run (when present):
  - lint: `python -m ruff check .` / `flake8` (repo dependent)
  - tests: `pytest`
- Never commit `.env` files

### Web apps (CodeverseHubWebsite, archived site-v2/v3)

- Use the repo’s package manager (`npm`, `pnpm`, `yarn`)
- Run:
  - `npm test` (if present)
  - `npm run lint`
  - `npm run build`

### Linux / systems projects (CodeVerseLinuxDistro, Codeverse-compositor)

- Provide reproducible steps in PR description (distro, kernel, hardware/VM)
- Prefer scripts under `scripts/` and document how to run them
- For Rust:
  - `cargo fmt --all`
  - `cargo clippy --workspace --all-targets -- -D warnings`
  - `cargo test --workspace`

## Pull request checklist

Before opening a PR:

- [ ] Linked an issue (or explained why it’s not needed)
- [ ] Added tests or explained why not
- [ ] Updated docs / README if user-facing
- [ ] Verified CI locally where possible

## Reporting bugs

- Use the **Bug report** issue template.
- Include:
  - exact steps to reproduce
  - expected vs actual
  - logs / screenshots (remove tokens)

## Code of Conduct

By participating in this org, you agree to follow our Code of Conduct:
see [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
