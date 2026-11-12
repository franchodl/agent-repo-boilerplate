# Project guidance

This repository is a full-stack application starter centered on React and Django. Follow the existing structure and conventions as they are established; do not assume frontend or backend directory names.

## Working in this repository

- Read the relevant code and project configuration before changing files. Keep changes focused and consistent with existing patterns.
- For React work, preserve the current component, styling, state-management, and API-client conventions. Keep interfaces responsive and accessible.
- For Django work, use the project's existing app, model, view, serializer, and URL patterns. Make schema changes with migrations and validate them with the relevant tests.
- Keep frontend and backend API changes aligned. Handle loading, empty, validation, and error states explicitly.
- Prefer the smallest complete change: reuse existing code and platform features, and avoid speculative abstractions or dependencies without cutting validation, error handling, security, accessibility, or necessary tests.
- Do not commit credentials, local configuration, or generated artifacts. Use the project's established environment-variable approach for secrets.
- Add or update focused tests for behavior changes. Run the narrowest relevant tests, lint, type-check, or build commands available in the repository, and report any checks that could not be run.

## Commands

Discover the available commands from the repository's package scripts, Django configuration, and documentation. Do not invent commands or modify dependencies unless the task requires it.
