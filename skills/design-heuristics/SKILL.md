---
name: design-heuristics
description: Evaluate digital interface designs with evidence-based usability heuristics and produce prioritized, actionable recommendations. Use for UI/UX reviews, heuristic evaluations, design critiques, screenshots, mockups, prototypes, websites, mobile apps, dashboards, forms, flows, responsive layouts, accessibility checks, or before-and-after redesign proposals in any project.
---

# Design Heuristics

Review an interface as a working product, not as a static composition. Separate directly observed problems from assumptions and make every recommendation traceable to user impact.

## Review workflow

1. Establish the surface and task.
   - Identify the primary user, their goal, the interface state, and the likely device or viewport.
   - Inspect supplied screenshots or artifacts. When source code or a runnable app is in scope, inspect the relevant implementation and representative viewports.
   - Do not modify files or deploy unless the user explicitly asks for changes.

2. Read [references/heuristics.md](references/heuristics.md) before evaluating. Apply only relevant criteria; do not inflate the report with inapplicable checks.

3. Review the full interaction, when evidence permits.
   - Check information hierarchy, task flow, navigation, controls, feedback, content, accessibility, responsive behavior, and failure recovery.
   - Include realistic stress states: long text, missing data, loading, empty, error, disabled, selected, focus, narrow viewport, and zoom.
   - Distinguish `Observed`, `Inferred`, and `Not tested`. Never claim accessibility or standards compliance from a screenshot alone.

4. Prioritize findings by severity.
   - `S0 — Cosmetic`: polish issue with negligible task impact.
   - `S1 — Minor`: noticeable friction with an easy workaround.
   - `S2 — Major`: slows or confuses a common task; likely to cause errors.
   - `S3 — Critical`: blocks a core task, hides essential information, or creates serious accessibility or trust risk.
   - Base severity on impact, frequency, and reach. Keep implementation effort separate.

5. Recommend concrete changes.
   - State what to change, where, and why.
   - Preserve valuable existing patterns and product constraints.
   - Prefer the smallest change that fixes the underlying task problem.
   - Group related symptoms under one root cause instead of repeating them.

6. Verify redesigns when requested.
   - Define the target behavior before styling.
   - Cover desktop and mobile plus important empty/error states.
   - If implementing, run proportionate functional, responsive, and accessibility checks.
   - Compare the result against the original finding and report remaining uncertainty.

## Output contract

Lead with the overall assessment and the three most consequential changes. Then provide a prioritized findings table with:

| Field | Required content |
| --- | --- |
| Severity | S0–S3 |
| Heuristic | Short criterion name |
| Evidence | Exact observed location or behavior |
| User impact | Consequence for the user's task |
| Recommendation | Specific corrective action |
| Confidence | High, medium, or low |

Keep the main list to the highest-value findings, normally 5–10. Follow with:

- strengths worth preserving;
- responsive and accessibility notes;
- a staged action plan: `Now`, `Next`, `Later`;
- verification steps or questions for anything not directly testable.

For a quick review, return the overall assessment, top three findings, and next action only. For a requested redesign, add a compact behavior specification or visual preview, whichever best matches the available artifact.

## Guardrails

- Do not equate personal taste with usability evidence.
- Do not recommend trends without a task-based rationale.
- Do not diagnose user behavior from appearance alone.
- Do not bury blocking issues beneath visual polish.
- Do not score every heuristic mechanically; prioritize the actual journey.
- Do not use color alone to communicate state.
- Do not remove useful density from expert tools without considering scan speed and throughput.
- Do not prescribe desktop conventions to mobile or mobile conventions to desktop without checking context.
