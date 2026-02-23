# CLAUDE.md — Holesome

This file provides guidance for AI assistants (Claude Code and others) working in this repository.

---

## Project Overview

**Holesome** is a new project in its initial stage. As of the last update to this file, no technology stack, framework, or application code has been committed. This document will grow as the project evolves.

- **Repository:** jbaumtana/Holesome
- **Default branch:** `main`
- **Feature branch convention:** `claude/<description>-<session-id>`

---

## Repository Structure

```
Holesome/
├── CLAUDE.md      # This file — AI assistant guidance
└── README.md      # Project overview (minimal, to be expanded)
```

As source code, tests, and configuration are added, this section should be updated to reflect the new structure.

---

## Git Workflow

### Branching

- Production-ready code lives on `main`.
- Feature and AI-assisted development branches follow the pattern:
  `claude/<short-description>-<session-id>`
- Never push directly to `main` without a pull request.

### Committing

Write clear, descriptive commit messages:

```
<type>: <short summary>

<optional longer explanation of why, not what>
```

Common types: `feat`, `fix`, `docs`, `refactor`, `test`, `chore`.

### Pushing

Always push with tracking:

```bash
git push -u origin <branch-name>
```

If a push fails due to a network error, retry with exponential backoff (2 s, 4 s, 8 s, 16 s) before giving up.

---

## Development Setup

_No setup steps are defined yet. When the stack is chosen, add instructions here covering:_

- Prerequisites (runtime versions, package managers, etc.)
- Dependency installation command
- Environment variable setup (reference an `.env.example` file if one exists)
- How to start the development server / run the application

---

## Running Tests

_No test framework has been configured yet. When tests are added, document:_

- The test runner command (e.g., `npm test`, `pytest`, `cargo test`)
- How to run a single test or test file
- How to run tests in watch mode

Always run the full test suite before committing and ensure it passes.

---

## Linting & Formatting

_No linter or formatter is configured yet. When tooling is added, document:_

- The lint command and auto-fix command
- The format command
- Any pre-commit hook setup

Code should be lint-clean before every commit.

---

## Building

_No build system is configured yet. When one is added, document:_

- The build command
- Output directory / artifact location
- Any environment-specific build flags

---

## Key Conventions

These conventions apply regardless of the stack chosen:

1. **Read before editing.** Never propose changes to code you have not read.
2. **Minimal diff.** Only change what is required by the task. Avoid formatting
   unrelated lines, adding unsolicited comments, or refactoring bystander code.
3. **No over-engineering.** Prefer the simplest solution that satisfies the
   requirement. Avoid premature abstractions or hypothetical extensibility.
4. **Delete dead code.** Remove unused variables, imports, and functions rather
   than commenting them out or renaming with underscores.
5. **Security first.** Never introduce SQL injection, XSS, command injection, or
   other OWASP Top 10 vulnerabilities. Validate at system boundaries (user
   input, external APIs) and trust internal guarantees.
6. **No hardcoded secrets.** Credentials, API keys, and tokens must come from
   environment variables or a secrets manager — never committed to source.

---

## Updating This File

When making significant changes to the project (adding a framework, configuring
CI, establishing a new convention), update this file in the same pull request.
This keeps AI assistant context accurate and reduces misunderstandings in future
sessions.
