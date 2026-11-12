---
name: react-best-practices
description: Write, refactor, or review React code for correctness, maintainability, and performance. Use for components, hooks, state, rendering, data fetching, and bundle changes.
---

# React code quality

Apply this skill when changing React code. First inspect the app's React version, framework, state/data libraries, TypeScript settings, and established patterns. Do not introduce Next.js-specific behavior into a non-Next.js app.

## Core practices

- Keep components focused and composable. Preserve clear ownership of state and derive values during render when possible rather than duplicating state.
- Follow the Rules of Hooks. Keep effects for synchronizing with external systems; put user-triggered work in event handlers.
- Use stable, meaningful keys for collections. Avoid defining component types inside another component's render.
- Keep data flow and async behavior explicit. Run independent requests concurrently when safe, handle failures, and avoid serial request chains that are not required.
- Avoid unnecessary renders and memoization. Measure or identify expensive work before adding `memo`, `useMemo`, or `useCallback`.
- Keep imports and dependencies narrow. Lazy-load genuinely large or infrequently used features when the app's bundler supports it.
- Preserve type safety and accessible behavior; performance changes must not break loading, error, empty, or interaction states.
- Follow existing tests and conventions. Add or adjust focused tests for behavior changed, and run the narrowest relevant checks.

## Performance review order

When optimizing, look first for avoidable request waterfalls and oversized initial bundles, then server/client data boundaries where applicable, redundant subscriptions and state updates, and expensive rendering or JavaScript work. Prefer a simple measured fix over speculative micro-optimization.

## Reference

For detailed React and Next.js performance rules and examples, consult Vercel's [react-best-practices skill](https://github.com/vercel-labs/agent-skills/tree/main/skills/react-best-practices). Treat framework-specific guidance as applicable only when the project uses that framework.
