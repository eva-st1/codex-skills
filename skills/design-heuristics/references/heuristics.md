# Interface evaluation criteria

Use this reference as a menu, not a mandatory scorecard. Evaluate criteria only when the artifact provides evidence.

## Core usability heuristics

### 1. Visibility of system status

Keep users informed about location, state, progress, saving, success, failure, and the consequences of an action. Feedback should arrive close to the triggering control and at the right level of persistence.

### 2. Match with the user's mental model

Use domain language, familiar ordering, realistic units, and concepts users already understand. Organize around their task rather than the implementation or database structure.

### 3. User control and freedom

Provide clear exits, back paths, cancellation, undo where feasible, and protection from accidental state loss. Avoid traps, surprising redirects, and irreversible actions without confirmation.

### 4. Consistency and standards

Keep labels, control behavior, placement, status semantics, and visual patterns consistent within the product. Follow platform conventions unless a deliberate exception improves the task.

### 5. Error prevention

Constrain invalid input, show requirements before submission, choose safe defaults, preserve user work, and confirm destructive or costly actions. Prefer preventing errors to explaining them later.

### 6. Recognition over recall

Keep relevant choices, context, history, labels, and next steps visible. Do not make users remember values between screens or infer unlabeled icons.

### 7. Flexibility and efficiency

Support both new and frequent users through sensible defaults, search, filtering, shortcuts, bulk actions, and compact scanning where appropriate. Optimize common paths without hiding essential controls.

### 8. Aesthetic and minimalist design

Give each element a clear job. Reduce competing emphasis, redundant copy, decorative noise, and unnecessary steps. Minimalism means signal clarity, not removing useful information.

### 9. Error recognition and recovery

Use plain-language messages that identify what happened, preserve context, point to the affected field or action, and give a recovery path. Never blame the user or expose irrelevant implementation details.

### 10. Help and documentation

Make the interface self-explanatory for common tasks. Provide concise, contextual help for unfamiliar, risky, or infrequent work rather than relying on a separate manual.

## Visual and content quality

- Establish one dominant page purpose and a predictable reading order.
- Use type size, weight, spacing, and contrast consistently to express hierarchy.
- Keep labels adjacent to controls and values; avoid ambiguous icon-only actions.
- Write action labels that describe outcomes, not generic commands such as “Submit”.
- Use consistent date, currency, number, status, and capitalization formats.
- Test realistic localization and long-content expansion. Avoid single-character wrapping, clipping, overlap, and layout shifts.
- Preserve useful whitespace while avoiding distances that break relationships or push core work below the fold.

## Responsive behavior

- Identify the task priority at each viewport rather than merely shrinking desktop UI.
- Keep primary actions and current context visible early in the mobile viewport.
- Reflow intentionally: stack related content, use horizontal scrolling only for genuinely sequential or tabular structures, and signal when more content exists.
- Preserve minimum readable text and approximately 44 by 44 CSS-pixel touch targets for primary mobile controls.
- Test at narrow phone, wide phone, tablet, laptop, and large desktop widths, including 200% zoom where practical.
- Check long labels, virtual keyboards, safe areas, sticky elements, drawers, dialogs, and orientation changes.

## Accessibility

- Ensure keyboard access, logical focus order, visible focus, and an escape path from overlays.
- Move focus into dialogs and restore it to the trigger when they close.
- Provide programmatic names, labels, roles, states, and relationships.
- Maintain sufficient text and non-text contrast; inspect hover, focus, disabled, selected, and error states.
- Do not rely on color, motion, position, or icon shape alone to convey meaning.
- Support text resizing, zoom, reflow, reduced motion, and screen-reader announcements for dynamic status where applicable.
- Treat a screenshot review as preliminary; verify semantics and interaction in a runnable artifact before making compliance claims.

## Workflow and data-heavy interfaces

- Show the next action, owner, urgency, and status before secondary metadata.
- Keep filters reflected in summaries, counts, exports, and empty states unless the interface explicitly explains a different scope.
- Preserve stable column meaning and prevent important items from silently moving out of view.
- Use progressive disclosure: concise list or card for scanning, detail view for editing and history.
- Make destructive, archival, and reversible state transitions distinct.
- Retain search context and filters when users open and close details.
- For expert tools, measure density against scanability and throughput instead of defaulting to spacious consumer layouts.

## Trust, privacy, and safety

- Explain why sensitive data or permissions are requested and how they will be used.
- Display the actual scope and consequence of publishing, sending, deleting, billing, or changing access.
- Avoid dark patterns, hidden opt-ins, misleading urgency, and ambiguous consent.
- Mask or minimize sensitive information when the task does not require full exposure.
