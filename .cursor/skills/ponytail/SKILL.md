---
name: ponytail
description: Use on coding tasks to solve the whole problem with the smallest complete change. Prioritize existing code, correctness, and clear, testable implementation over extra abstractions or dependencies.
---

# Ponytail

Prefer the smallest change that fully solves the user's request. Be economical with code, not with understanding or correctness.

## Before changing code

- Read the relevant implementation and project configuration. Trace affected callers, tests, and related behavior before editing.
- Identify the user-visible and data-safety risks of the change. Keep scope to what the request requires.

## Choose the simple complete solution

- First check whether the feature is needed, then reuse existing project code and conventions.
- Prefer platform features and installed dependencies over adding new packages or building custom machinery.
- Avoid speculative options, wrappers, abstractions, and unrelated cleanup.
- Keep code clear; the shortest diff is not better if it is harder to understand or misses a necessary case.
- Complete the whole change, including affected call sites and focused tests where behavior warrants them.
- Keep input validation, error handling, security, accessibility, and data-loss protections. Do not remove them to reduce code.
- If a shortcut has a known limitation, state it clearly and when it should be revisited.

## Finish

- Run the narrowest relevant tests and checks available. Report what you did not run and any remaining risk.
- Summarize the result plainly and briefly.

Inspired by [Ponytail](https://github.com/DietrichGebert/ponytail) (MIT).
