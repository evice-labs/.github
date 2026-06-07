# Contributing to Evice Labs

Thank you for your interest in contributing to Evice Labs! This document outlines how to get involved and what to expect.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Workflow](#development-workflow)
- [Pull Request Process](#pull-request-process)
- [Commit Message Convention](#commit-message-convention)
- [Style Guidelines](#style-guidelines)

---

## Code of Conduct

By participating, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md). Please read it first.

---

## How Can I Contribute?

### 🐛 Reporting Bugs

1. Search [existing issues](../../issues) to avoid duplicates
2. Gather relevant info: OS, version, steps to reproduce, expected vs. actual behavior
3. Open a new issue using the **Bug Report** template

### 💡 Suggesting Features

Open a **Feature Request** issue and include:
- The problem you're solving
- Your proposed solution
- Any alternatives you've considered

### 🛠 Contributing Code

1. Browse issues labeled [`good first issue`](../../issues?q=label%3A"good+first+issue") or [`help wanted`](../../issues?q=label%3A"help+wanted")
2. Comment on the issue to signal you're working on it
3. Fork the repository and create a branch from `main`

### 📚 Improving Documentation

Typos, clarifications, new examples, and translations are all welcome.

---

## Development Workflow

### Prerequisites

Repositories in this organization use one or more of the following. Check each repo's `README.md` for specific setup instructions.

- **Rust** — stable toolchain via `rustup`
- **C++ / Qt** — Qt 6.x recommended
- **Node.js** — LTS version
- **RISC0 toolchain** — for ZK circuit repositories

### Setup

```bash
# 1. Fork the repository on GitHub, then clone your fork
git clone https://github.com/YOUR_USERNAME/REPO_NAME.git
cd REPO_NAME

# 2. Add the upstream remote
git remote add upstream https://github.com/evice-labs/REPO_NAME.git

# 3. Create a feature branch
git checkout -b feat/your-feature-name

# 4. Make your changes and run tests
# (see each repo's README for test commands)
```

### Keeping Your Fork Up to Date

```bash
git fetch upstream
git rebase upstream/main
```

---

## Pull Request Process

1. Ensure **all tests pass** before opening a PR
2. **Update documentation** if your change affects public APIs or behavior
3. Fill out the **PR template** completely
4. Link the related issue using `Closes #123` or `Fixes #123`
5. Request a review from at least one maintainer

### Review Expectations

- Maintainers aim to review PRs within **5 business days**
- Address all review comments before requesting re-review
- PRs with no activity for **14 days** may be closed (and can be reopened)

### Merge Policy

- At least **1 approving review** required
- Branch must be up to date with `main`
- Maintainers will merge using **squash and merge** to keep history clean

---

## Commit Message Convention

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <short summary>

[optional body]

[optional footer(s)]
```

| Type | When to use |
|------|-------------|
| `feat` | New feature |
| `fix` | Bug fix |
| `docs` | Documentation only |
| `refactor` | Code change, no new feature or bug fix |
| `test` | Adding or updating tests |
| `chore` | Build process, dependency updates |
| `perf` | Performance improvements |

**Examples:**

```
feat(zk-circuit): add nullifier generation for membership proof
fix(ffi): resolve segfault on cbindgen header mismatch
docs(readme): update build instructions for RISC0 v1.1
```

---

## Style Guidelines

### Rust
- Run `cargo fmt` before committing
- Run `cargo clippy -- -D warnings` — no warnings allowed
- Write doc comments (`///`) for all public items

### C++ / Qt
- Follow [Qt coding conventions](https://wiki.qt.io/Coding_Conventions)
- Use `clang-format` with the project's `.clang-format` config
- Prefer RAII patterns over raw `new`/`delete`

### General
- Keep lines under 100 characters where possible
- Write tests for new functionality
- Prefer explicit over implicit

---

## Questions?

Open a [Discussion](../../discussions) or reach out on [Logos Discord](https://discord.gg/logos).

We appreciate every contribution, no matter how small. 🙏
