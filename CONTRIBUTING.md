# Contributing to Zenith

Thanks for your interest in contributing to Zenith! This document covers how to get started, our standards, and what to expect.

## Before You Start

- Contributions require agreeing to our [Contributor License Agreement](./CLA.md). The CLA Assistant bot will prompt you on your first pull request.
- Be respectful. All participation is governed by our [Code of Conduct](./CODE_OF_CONDUCT.md).
- For questions and discussion, join our [Discord](https://discord.zenithfivem.dev).

## Ways to Contribute

- **Report bugs** — open an issue using the Bug Report template. Include reproduction steps, your server artifact version, and relevant console output.
- **Request features** — open an issue using the Feature Request template. Explain the use case, not just the feature.
- **Submit code** — fix a bug or build a feature via a pull request (see below).
- **Improve docs** — documentation fixes are always welcome and are a great first contribution.

## Development Setup

1. Fork the relevant repository and clone your fork.
2. Ensure you have Zenith's dependencies installed (`ox_lib`, `oxmysql`, and any others noted in the repo's README).
3. Create a branch off `main` for your work: `git checkout -b fix/short-description`.

## Coding Standards

- **Lua formatting** is enforced with [StyLua](https://github.com/JohnnyMorganz/StyLua). Run it before committing, or let the formatter workflow handle it.
- **Linting** is enforced with [luacheck](https://github.com/mpeterv/luacheck). Your PR must pass the lint workflow.
- Keep the core platform-neutral where possible — shared logic should not hard-depend on FiveM-only natives so the codebase stays portable.
- Write clear, self-documenting code. Comment the _why_, not the _what_.

## Pull Request Process

1. Make sure your branch is up to date with `main`.
2. Ensure lint and formatting checks pass.
3. Fill out the pull request template completely.
4. Link any related issues (e.g. `Closes #123`).
5. A maintainer will review. Address feedback by pushing new commits to the same branch.
6. Once approved and checks pass, a maintainer will merge.

## Commit Messages

We follow [Conventional Commits](https://www.conventionalcommits.org/) where practical. Examples:

- `feat(economy): add dirty money support`
- `fix(jobs): correct grade lookup off-by-one`
- `docs(readme): clarify installation steps`

This keeps history readable and helps automate changelogs.

---

Thank you for helping make Zenith better!
