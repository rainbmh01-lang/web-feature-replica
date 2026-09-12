---
name: web-feature-replica
description: Rebuilds a web feature from a reference website with high observable visual, interaction, and functional fidelity. Use when recreating an existing website feature inside the current project without adding, removing, redesigning, or simplifying its functionality.
---

# Web Feature Replica

## Objective

Recreate the requested feature from the reference website inside the current project with the highest possible fidelity to the observable reference.

The reference website is the source of truth for:

- visual appearance
- layout
- typography
- spacing
- colors
- components
- interactions
- user flows
- visible states
- responsive behavior
- error and loading states
- functional behavior

Do not invent behavior that was not observed.

## Workflow

Follow these phases in order:

1. Inspect the reference website.
2. Analyze its visual structure.
3. Analyze its interactions and user flows.
4. Analyze its states and edge cases.
5. Create a structured feature specification.
6. Inspect the current project before implementation.
7. Implement the feature using the project's existing architecture and conventions.
8. Test the implementation.
9. Compare the implementation against the reference.
10. Correct verified differences.
11. Perform a final fidelity audit.

## Fidelity Rules

- Do not add functionality that does not exist in the reference.
- Do not remove functionality that exists in the reference.
- Do not redesign the feature.
- Do not simplify the user flow.
- Do not replace observed behavior with assumptions.
- Do not copy proprietary source code.
- Do not copy credentials, secrets, private data, or protected content.
- Prefer independent implementation based on observable behavior.
- Preserve the current project's architecture unless a change is required to implement the feature.

## Supporting Resources

Before executing each phase, read the corresponding resource file from this skill:

- `resources/reconnaissance.md`
- `resources/visual-analysis.md`
- `resources/interaction-analysis.md`
- `resources/state-analysis.md`
- `examples/feature-specification.md`
- `resources/implementation.md`
- `resources/fidelity-audit.md`

Do not skip a phase unless the resource explicitly determines that the phase is not applicable.

## Final Requirement

The task is not complete when the feature merely works.

The task is complete only after the implementation has been compared with the reference and all observable, verified differences that matter to the requested feature have been corrected.
