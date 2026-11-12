---
name: web-design-guidelines
description: Review web UI changes for usability, accessibility, responsive behavior, and interface consistency. Use for UX or accessibility audits and before shipping substantial UI work.
---

# Web design and accessibility review

Review the requested files or UI changes. If the scope is not specified, inspect the files changed for the current task; ask only when the target cannot be determined.

## Review method

1. Inspect the implementation and its surrounding components. Check behavior as well as markup and styles.
2. For a formal interface-guidelines review, fetch the current rules from:
   `https://raw.githubusercontent.com/vercel-labs/web-interface-guidelines/main/command.md`
   Apply the retrieved rules rather than relying on an outdated local copy. If the source cannot be reached, say so and continue with the checks below.
3. Check applicable items:
   - Semantic structure, meaningful headings, labels, accessible names, and alternative text.
   - Keyboard access, logical focus order, visible focus, and usable dialogs or menus.
   - Text and control contrast, zoom/reflow, reduced motion, and non-color status cues.
   - Touch target usability, responsive overflow, and readable content hierarchy.
   - Clear navigation and actions, understandable validation and errors, and useful loading/empty states.
   - Consistent interaction behavior and avoidance of redundant or misleading controls.
4. Report only actionable issues supported by the code. Give each finding a severity and a precise file and line; state the user impact and a concise fix. Do not report speculative issues as confirmed.
5. If no issues are found, say so and mention any relevant checks that could not be verified from code alone.

This checklist is a practical review aid, not a claim of full WCAG conformance. Recommend manual or automated assistive-technology testing when the task requires a conformance claim.

## Reference

The interface review workflow is based on Vercel's [web-design-guidelines skill](https://github.com/vercel-labs/agent-skills/tree/main/skills/web-design-guidelines). The live guideline source is maintained in [vercel-labs/web-interface-guidelines](https://github.com/vercel-labs/web-interface-guidelines).
