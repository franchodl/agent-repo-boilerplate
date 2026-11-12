---
name: ponytail-audit
description: Perform an evidence-based review of a repository or named area for correctness, security, data loss, expected-load risks, missing tests, performance, and unnecessary complexity. Report findings without changing code.
---

# Repository audit

Return a one-shot report; do not modify files. Audit the requested area, or the whole repository if none is specified.

## Inspect

- Map the project from its documentation, dependency and deployment configuration, entry points, and tests.
- Trace high-risk flows end to end, especially user input, authentication, persistence, background work, and shared state.
- Consider expected usage and load; state assumptions and identify areas you did not inspect.
- In a large repository, focus on paths where defects would have the greatest impact rather than claiming exhaustive coverage.

## Report only verified findings

- Look for concrete bugs, security or data-loss risks, failures at expected load, risky untested logic, meaningful slow paths, and code that can safely be removed or simplified.
- Give each finding an example or condition that causes the problem. Verify callers and dynamic references before calling code unused.
- Distinguish proven issues from checks that cannot be confirmed statically. Do not present style preferences or vague possibilities as defects.
- Order findings by impact and provide the smallest useful fix. Do not make the fix unless the user asks.

## Output

Start with a short summary of what the repository does and the usage/load assumed. Group numbered findings into **Must fix**, **Should fix**, and **Nice to have**, omitting empty groups. For each, include the location, problem, concrete impact, and concise fix.

End with a one-line verdict and a **Not checked** note for significant gaps. If nothing actionable is found, say what was inspected and that no issues were found.

Inspired by [Ponytail](https://github.com/DietrichGebert/ponytail) (MIT).
