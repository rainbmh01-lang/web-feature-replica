# Web Feature Replica — Antigravity Skill

An Antigravity Agent Skill for rebuilding web features from reference websites with high observable visual, interaction, and functional fidelity.

## Version

**v1.0.0**

## Overview

`web-feature-replica` is an Antigravity Agent Skill designed to help recreate an existing web feature inside the current project.

The reference website is treated as the source of truth for observable:

- Visual design
- Layout
- Typography
- Spacing
- Colors
- Components
- Interactions
- User flows
- UI states
- Loading and error states
- Responsive behavior
- Functional behavior

The goal is not to redesign the feature, but to reproduce the behavior and appearance that can be observed from the reference.

## Workflow

The skill follows a structured workflow:

1. **Reconnaissance**
   - Inspect the reference website.
   - Identify the complete user flow.
   - Record observable behavior and states.

2. **Visual Analysis**
   - Analyze layout, dimensions, spacing, typography, colors, borders, shadows, and responsive behavior.

3. **Interaction Analysis**
   - Identify interactive elements.
   - Analyze clicks, selections, inputs, dropdowns, navigation, and user flows.

4. **State Analysis**
   - Model the observable UI states and their transitions.
   - Keep independent state dimensions separate when appropriate.

5. **Feature Specification**
   - Convert observations into an implementation-ready specification.
   - Preserve evidence provenance.
   - Distinguish observed requirements from inferred implementation details.

6. **Implementation**
   - Inspect the existing project.
   - Implement the feature using the project's existing architecture and conventions.

7. **Testing**
   - Test the implemented feature functionally.
   - Test important edge cases and responsive layouts.

8. **Fidelity Audit**
   - Compare the implementation against the reference.
   - Identify observable differences.
   - Correct verified differences.
   - Re-test after corrections.

## Core Principles

### Observable behavior is authoritative

The reference website is the source of truth for behavior that can actually be observed.

### No unnecessary redesign

The skill should not:

- Add functionality that does not exist in the reference.
- Remove functionality that exists in the reference.
- Simplify the user flow.
- Redesign the interface without evidence.
- Replace observed behavior with assumptions.

### Evidence provenance

Important requirements should retain their evidence classification:

- `[Directly Observed]`
- `[Measured/Inspected]`
- `[Inferred]`

Inferred information must not be promoted into a verified requirement without evidence.

### Independent implementation

The skill recreates behavior and appearance based on observation.

It does not copy proprietary source code, credentials, secrets, private data, or protected content.

## Included Resources

```text
web-feature-replica/
├── SKILL.md
├── resources/
│   ├── reconnaissance.md
│   ├── visual-analysis.md
│   ├── interaction-analysis.md
│   ├── state-analysis.md
│   ├── implementation.md
│   └── fidelity-audit.md
└── examples/
    └── feature-specification.md