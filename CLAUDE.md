# CLAUDE.md

This file provides guidance for AI assistants (Claude and others) working in the `qip-json-analyze` repository.

## Project Overview

**Repository:** `jscala-partneresi/qip-json-analyze`
**Purpose:** JSON analysis tooling (exact scope to be defined as the project evolves).

> **Note:** This repository was initialized empty. Update this file as code is added.

## Repository Status

This repository is currently in its initial state. As code is committed, update the sections below to reflect:
- The chosen language and runtime
- The build system and dependency manager
- Test framework and how to run tests
- Linting and formatting tools
- CI/CD pipeline details

## Development Setup

Once source files exist, document setup steps here. A typical pattern:

```bash
# Clone the repository
git clone <repo-url>
cd qip-json-analyze

# Install dependencies (update command based on chosen toolchain)
# npm install / pip install -e . / cargo build / etc.

# Run tests
# npm test / pytest / cargo test / etc.
```

## Branch Conventions

- The main integration branch is `main` (or `master` — update once established).
- Feature branches follow the pattern: `claude/<description>-<session-id>` for AI-driven work.
- Human-driven work branches: `feat/<short-description>`, `fix/<short-description>`.

## Commit Message Style

Use concise, imperative-mood commit messages:

```
Add JSON schema validation for nested arrays
Fix off-by-one error in key depth counter
Refactor parser to use streaming input
```

Avoid vague messages like "fix stuff" or "update code".

## Code Conventions

Update this section once the language and style guide are decided. Common things to document:
- Naming conventions (snake_case, camelCase, PascalCase)
- File and directory naming patterns
- How public API surface is organized vs internal helpers
- Error handling philosophy (exceptions vs result types vs error codes)
- Logging conventions

## Testing

Document the testing approach here when tests are added:
- Unit test location and naming pattern
- Integration/end-to-end test location
- How to run a subset of tests
- Coverage requirements (if any)

## JSON Analysis Conventions

Since this project deals with JSON analysis, consider documenting:
- Supported JSON dialects (JSON5, NDJSON, JSON Lines, etc.)
- How large payloads are handled (streaming vs in-memory)
- Schema validation approach (JSON Schema, custom, etc.)
- Output format conventions for analysis results

## AI Assistant Guidelines

When working in this repository, AI assistants should:

1. **Read before editing** — always read a file fully before modifying it.
2. **Minimal changes** — make only the changes necessary to fulfil the task; do not refactor unrelated code.
3. **No speculative features** — do not add error handling, abstractions, or capabilities that are not explicitly requested.
4. **Update this file** — if you discover important conventions, project structure details, or workflow steps not documented here, add them.
5. **Branch discipline** — develop on the designated `claude/` branch; never push directly to `main`/`master` without explicit permission.
6. **Commit incrementally** — commit logical units of work with clear messages; do not batch unrelated changes.
7. **No secrets in commits** — never commit API keys, tokens, credentials, or `.env` files.

## Useful Git Commands

```bash
# Check current branch and status
git status

# See recent history once commits exist
git log --oneline -20

# Push feature branch
git push -u origin <branch-name>
```

## Updating This File

This file should be kept current. Update it whenever:
- A new tool, dependency, or framework is adopted
- A new convention is established by the team
- The build or test workflow changes
- CI/CD is configured or modified
