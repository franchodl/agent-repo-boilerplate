---
name: ui-design-brain
description: Design and implement polished, consistent, accessible web interfaces in this React + Django application. Use for pages, components, forms, dashboards, navigation, and visual refinements.
---

# UI design

Use this skill whenever changing the user interface.

## Before implementation

- Inspect the existing React app, shared components, styling approach, and design tokens. Extend the established system instead of introducing a competing one.
- Identify the user goal, information hierarchy, and component patterns the screen needs. Prefer familiar, semantically appropriate patterns over novelty.
- If the request leaves visual direction open, choose one that suits the product and existing UI; do not make every screen look like a generic SaaS template.

## Implementation quality

- Keep layouts purposeful and scannable. Use spacing, type, and alignment to communicate hierarchy; avoid decorative elements that do not help users.
- Use semantic HTML and the existing component and styling libraries. Add ARIA only when native semantics are insufficient.
- Provide visible labels, clear action names, keyboard-operable controls, visible focus, and sufficient text and control contrast.
- Design responsive layouts for narrow and wide screens. Check that content, navigation, tables, and controls remain usable at small widths.
- Account for meaningful loading, empty, error, success, disabled, and validation states where relevant.
- Keep interactions predictable: buttons perform actions, links navigate, and destructive or irreversible actions are clearly distinguished.
- Follow the repository's existing conventions and avoid unnecessary dependencies or custom UI primitives.

## Review

Before finishing, inspect the changed interface for consistency with nearby screens, keyboard and focus behavior, responsive overflow, and incomplete states. Run the available frontend checks when practical.

## Reference

This project skill is an adaptation for this repository. For the upstream component-pattern catalog and additional examples, see [UI Design Brain](https://github.com/carmahhawwari/ui-design-brain). Its component data is sourced from [component.gallery](https://component.gallery).
