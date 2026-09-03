---
name: design-heuristics
description: Evaluate digital interfaces with evidence-based usability heuristics and produce prioritized, actionable recommendations. Use for UI/UX reviews, heuristic evaluations, design critiques, screenshots, mockups, prototypes, websites, mobile apps, dashboards, forms, flows, responsive layouts, accessibility checks, redesign specifications, or implementation QA in any project; do not trigger for purely aesthetic generation when no evaluation is requested.
---

# Design Heuristics

Review an interface as a working product, not as a static composition. Separate directly observed problems from assumptions and make every recommendation traceable to user impact.

## Contract

Serve the person who must decide what to change. Preserve every condition that can alter that decision: the user, task, state, viewport, platform convention, product constraint, evidence quality, consequence, and verification boundary. Prefer a short list of consequential findings over an exhaustive catalogue of taste-based comments.

Maintain a legibility floor in every review. Use plain language, visible priority, exact locations, and enough context for a designer or engineer to reproduce the issue. Do not make the reader reconstruct what happened, why it matters, or what success looks like.

## Choose the review mode

Use the narrowest mode that answers the request:

- **Quick triage:** identify the three most consequential issues and the next action from limited evidence.
- **Heuristic audit:** evaluate the representative journey, states, viewports, and relevant criteria in [references/heuristics.md](references/heuristics.md).
- **Redesign specification:** define improved behavior, hierarchy, content, responsive rules, and states before visual polish.
- **Implementation QA:** compare the built result with the intended behavior and test representative interactions and stress states.

A screenshot supports visual and content observations, but not claims about keyboard behavior, semantics, loading, persistence, or end-to-end success. Mark those as untested unless runnable evidence exists.

## Review workflow

1. Establish scope and evidence.
   - Identify the primary user, their goal, the interface state, and the likely device or viewport.
   - Inspect supplied screenshots or artifacts. When source code or a runnable app is in scope, inspect the relevant implementation and representative viewports.
   - Classify each artifact as `Current`, `Target`, `Proposed`, or `Historical`. Do not evaluate a proposal as if it were shipped behavior.
   - Record relevant constraints such as design-system rules, business policy, localization, data density, supported platforms, and technical limitations. If constraints conflict, expose the conflict instead of inventing a compromise.
   - Do not modify files or deploy unless the user explicitly asks for changes.

2. Read [references/heuristics.md](references/heuristics.md) before evaluating. Apply only relevant criteria; do not inflate the report with inapplicable checks.

3. Build an evidence-led task walkthrough.
   - Check information hierarchy, task flow, navigation, controls, feedback, content, accessibility, responsive behavior, and failure recovery.
   - Include realistic stress states: long text, missing data, loading, empty, error, disabled, selected, focus, narrow viewport, and zoom.
   - For non-trivial reviews, track each candidate finding as: `context | task | evidence | violated criterion | consequence | recommendation | verification`.
   - Distinguish `Observed`, `Inferred`, and `Not tested`. Keep hypotheses explicit and do not promote them into findings without evidence.

4. Prioritize findings by severity.
   - `S0 — Cosmetic`: polish issue with negligible task impact.
   - `S1 — Minor`: noticeable friction with an easy workaround.
   - `S2 — Major`: slows or confuses a common task; likely to cause errors.
   - `S3 — Critical`: blocks a core task, hides essential information, or creates serious accessibility or trust risk.
   - Base severity on task impact, likely frequency, reach, reversibility, and risk. Keep implementation effort separate so an expensive critical fix is not downgraded.

5. Recommend concrete changes.
   - State what to change, where, and why.
   - Preserve valuable existing patterns and product constraints.
   - Prefer the smallest change that fixes the underlying task problem.
   - Group related symptoms under one root cause instead of repeating them.
   - Choose the operation that fits the evidence: preserve, clarify, reorder, consolidate, reveal, constrain, reflow, or remove.
   - Define an observable success condition. If the evidence cannot select one solution, provide the decision criterion or a small set of alternatives instead of false certainty.

6. Verify redesigns when requested.
   - Define the target behavior before styling.
   - Cover desktop and mobile plus important empty/error states.
   - If implementing, run proportionate functional, responsive, and accessibility checks.
   - Compare the result against the original finding and report remaining uncertainty.

## Review integrity

The reviewer owns scope, evidence interpretation, severity, and acceptance. Do not broaden a review from one screen to an entire product unless an exposed dependency requires it. Do not silently treat code, design-system documentation, analytics, user research, or stakeholder comments as equivalent evidence; name what each source establishes.

For consequential recommendations, preserve this chain:

`evidence -> heuristic or task principle -> user consequence -> proposed change -> success check`

If a link is weak, lower confidence, request the missing evidence, or omit the finding. When sources conflict, prefer observed product behavior for claims about current behavior and explicit product requirements for intended behavior; report unresolved conflicts.

## Output contract

Lead with the overall assessment and the three most consequential changes. Then provide a prioritized findings table with:

| Field | Required content |
| --- | --- |
| Severity | S0–S3 |
| Heuristic | Short criterion name |
| Evidence | Exact location or behavior, labeled Observed or Inferred |
| User impact | Consequence for the user's task |
| Recommendation | Specific corrective action |
| Confidence | High, medium, or low |
| Verification | Observable check that would confirm the fix |

Keep the main list to the highest-value findings, normally 5–10. Follow with:

- strengths worth preserving;
- responsive and accessibility notes;
- a staged action plan: `Now`, `Next`, `Later`;
- verification steps or questions for anything not directly testable.

For a quick review, return the overall assessment, top three findings, and next action only. For a requested redesign, add a compact behavior specification or visual preview, whichever best matches the available artifact.

## Verification checklist

Run only checks supported by the artifact, and state what remains untested:

- **Coverage:** replay the primary task and at least one failure or empty path.
- **Responsive:** test representative widths, long content, text zoom, and reflow without clipping or overlap.
- **Interaction:** test focus, keyboard use, feedback, cancellation, recovery, persistence, and destructive actions.
- **Accessibility:** inspect semantics, names, contrast, focus order, announcements, target size, and non-color cues with appropriate tools.
- **Content and data:** verify labels, formats, localization, filter scope, counts, status meaning, and edge values.
- **Regression:** compare changed behavior with the finding and ensure the fix does not damage adjacent tasks or expert throughput.
- **Diff review:** check that the recommendation did not broaden scope, erase useful constraints, or replace evidence with preference.

## Guardrails

- Do not equate personal taste with usability evidence.
- Do not recommend trends without a task-based rationale.
- Do not diagnose user behavior from appearance alone.
- Do not bury blocking issues beneath visual polish.
- Do not score every heuristic mechanically; prioritize the actual journey.
- Do not use color alone to communicate state.
- Do not remove useful density from expert tools without considering scan speed and throughput.
- Do not prescribe desktop conventions to mobile or mobile conventions to desktop without checking context.
- Do not let a numerical score obscure a task-blocking issue or imply precision unsupported by evidence.
- Do not claim a redesign is successful from visual inspection alone; state the behavior tested and the remaining boundary.
