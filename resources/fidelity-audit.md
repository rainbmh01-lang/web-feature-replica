# Fidelity Audit

## Purpose

Compare the implemented feature against the reference feature after implementation.

The objective is to identify and correct observable differences in:

- appearance
- layout
- interactions
- states
- behavior
- responsive behavior

The audit must be based on direct comparison and evidence.

Do not declare the implementation equivalent based only on source-code inspection.

---

# 1. Audit Principle

The reference is the source of truth for observable behavior and appearance.

Compare equivalent states of:

- reference
- implementation

Do not compare unrelated parts of either application.

---

# 2. Prepare Equivalent Conditions

Before comparison, make the reference and implementation as comparable as possible.

Match:

- viewport dimensions
- zoom level
- browser environment when relevant
- initial state
- input values
- selected options
- uploaded test data
- interaction sequence

Use equivalent test data whenever possible.

---

# 3. Visual Comparison

Compare:

## Layout

- overall structure
- content width
- alignment
- positioning
- spacing
- section heights
- columns
- rows
- responsive layout

## Components

Compare:

- dimensions
- padding
- margins
- borders
- radius
- shadows
- backgrounds
- icons
- visibility

## Typography

Compare:

- font appearance
- size
- weight
- line height
- alignment
- wrapping
- truncation
- text spacing

## Colors

Compare:

- backgrounds
- text
- borders
- buttons
- links
- warnings
- errors
- success states

Do not rely solely on subjective judgment.

Use screenshots, browser inspection, measurements, or computed styles when available.

---

# 4. Interaction Comparison

Execute equivalent user actions on both versions.

For each action compare:

- starting state
- action
- immediate result
- resulting state
- visible feedback
- navigation
- enabled/disabled controls

Example:

```text
Reference:
Click button
→ loading
→ processing
→ success

Implementation:
Click button
→ loading
→ processing
→ success
```
