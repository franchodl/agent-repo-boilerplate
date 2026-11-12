# Agent Repo Boilerplate

A starting point for building full-stack applications with **React** and
**Django**, with project guidance and reusable AI-agent skills to support
consistent, accessible, maintainable development.

## What this repository provides

- **React + Django focus** for full-stack application development.
- **[MIT licensing](./LICENSE)** so you can use, modify, and fork the starter.
- **Project-specific guidance** in [`CLAUDE.md`](./CLAUDE.md), covering
  implementation, testing, API coordination, and use of environment variables
  for secrets.
- **Cursor rules and skills** for UI design, accessibility and UX reviews,
  React quality, and small, complete changes.
- **An on-demand repository audit skill** for evidence-based codebase reviews.
- **Contribution and security guidance** for people collaborating on the
  project.

## Agent skills

The Cursor skills are in [`.cursor/skills/`](./.cursor/skills/):

| Skill | Purpose |
| --- | --- |
| `ui-design-brain` | Build consistent, responsive, accessible interfaces. |
| `web-design-guidelines` | Review UI changes for usability and accessibility. |
| `react-best-practices` | Guide React component, state, and performance work. |
| `ponytail` | Prefer the smallest complete solution without sacrificing correctness. |
| `ponytail-audit` | Audit a repository or area and report actionable findings without changing code. |

The always-on Cursor rule in [`.cursor/rules/`](./.cursor/rules/) reinforces
focused, safe changes and relevant verification.

See [Third-party notices](./THIRD_PARTY_NOTICES.md) for attribution and
licensing information about referenced skill projects.

## Getting started

1. Use this repository as a template or create a copy for your application.
2. Add the React frontend and Django backend using the structure and tooling
   that best fit your application.
3. Configure local settings and credentials through environment variables;
   never commit secrets.
4. Document the actual install, run, test, and build commands once the
   application tooling is in place.

The current checkout contains the project guidance and agent skills; it does
not yet include application source code, dependency manifests, or runnable
development and test commands. Those depend on the scaffold added for your
application, so this README intentionally avoids prescribing unverified paths
or commands.

## Development principles

- Follow the structure and conventions established by the application.
- Keep frontend and backend API contracts aligned.
- Handle loading, empty, validation, and error states explicitly.
- Add focused tests for behavior changes and run the narrowest relevant checks.
- Prefer the smallest complete change; do not trade away validation, security,
  accessibility, or data safety for brevity.

## Contributing

Read [CONTRIBUTING.md](./CONTRIBUTING.md) before opening a pull request.
Community expectations are in the [Code of Conduct](./CODE_OF_CONDUCT.md), and
security issues should be reported according to [SECURITY.md](./SECURITY.md).

## Publishing checklist

Before sharing this repository:

- Confirm the repository description, topics, and default branch on GitHub.
- Enable GitHub private vulnerability reporting if you want to receive
  confidential security reports through the Security tab.
- Mark the repository as a template in GitHub settings if you want users to
  create new repositories from it with **Use this template**.
- Add CI checks when the application scaffold and its test commands are in
  place; require those checks before merging if appropriate.

This repository includes no application source or CI workflow yet, so those
checks and GitHub settings must be added or enabled when the project is ready.
