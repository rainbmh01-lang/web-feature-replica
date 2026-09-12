# Reference Website Reconnaissance

## Purpose

Inspect the reference website before implementation.

The goal is to determine what the requested feature actually does and how it behaves from the user's perspective.

Do not begin implementation during this phase.

Do not infer behavior when it can be observed directly.

## 1. Identify the Target

Record:

- Reference URL
- Page URL
- Target feature
- Feature entry point
- What the user must do to reach the feature
- Whether the feature depends on authentication, uploaded data, or another prerequisite

Clearly define the exact feature being reproduced.

Do not inspect unrelated features unless they affect the target feature.

## 2. Inspect the Initial State

Open the reference page and record the initial visible state.

Inspect:

- page structure
- navigation
- headers
- buttons
- inputs
- selectors
- cards
- dialogs
- menus
- tooltips
- notifications
- upload areas
- visible text
- disabled controls
- default values
- selected values
- placeholders
- icons
- visible warnings
- visible informational messages

Record what is actually visible.

Do not assume hidden functionality exists.

## 3. Explore the Feature

Interact with the feature systematically.

For every interactive element:

1. Identify the element.
2. Perform the available interaction.
3. Observe what changes.
4. Record the resulting state.
5. Record any navigation or side effect.
6. Return to the previous state when necessary.
7. Test the next interaction.

Test relevant interactions such as:

- click
- double click
- hover
- focus
- blur
- typing
- clearing input
- selecting options
- opening menus
- closing menus
- dragging
- dropping
- scrolling
- keyboard input
- keyboard shortcuts
- upload
- removal
- confirmation
- cancellation
- navigation

Do not modify the reference account or submit destructive actions.

## 4. Inspect Browser-Observable Behavior

Use browser inspection when available.

Inspect:

- DOM structure
- visible element hierarchy
- element roles
- labels
- accessible names
- input types
- button states
- selected states
- disabled states
- dialogs
- menus
- validation messages
- loading indicators
- navigation changes

Use browser inspection to verify observations, not to copy proprietary implementation code.

## 5. Record User Flow

Describe the complete observable flow:

Initial state
→ user action
→ resulting state
→ next action
→ resulting state
→ completion or error

Include alternative paths when they are observable.

## 6. Test Important Edge Cases

Test reasonable user inputs and boundary conditions when the reference makes them observable.

Examples:

- empty input
- invalid input
- minimum value
- maximum value
- decimal value
- extremely large value
- clearing a value
- missing required input
- invalid file
- unsupported file
- cancelled action
- repeated action
- slow/loading state
- error state

Only record behavior that can actually be verified.

## 7. Responsive Inspection

If the feature is intended to work across screen sizes, inspect it at relevant viewport sizes.

Record:

- layout changes
- element repositioning
- hidden elements
- collapsed controls
- changed spacing
- changed typography
- mobile-specific interactions
- horizontal scrolling
- responsive menus

Do not assume desktop and mobile behavior are identical.

## 8. Screenshots and Evidence

Capture screenshots of important states when possible.

At minimum capture:

- initial state
- main feature state
- important interaction states
- loading state
- error state
- completion state
- responsive states when relevant

Use screenshots as visual evidence during later implementation and fidelity auditing.

## 9. Evidence Rule

Every important behavior recorded in the feature specification should have an observable basis.

Evidence can come from:

- direct interaction
- browser inspection
- visible UI
- screenshots
- accessible labels
- documented behavior that is explicitly relevant to the feature

Do not convert assumptions into requirements.

## 10. Reconnaissance Output

At the end of this phase, produce a concise reconnaissance report containing:

### Reference

- URL:
- Page:
- Target feature:

### Entry Point

- How the feature is reached:

### Initial State

- Visible elements:
- Default values:
- Disabled elements:

### Interactions

For each interaction:

- Element:
- Action:
- Result:

### User Flow

Describe the complete observable flow.

### States

List all observed states.

### Edge Cases

List all verified edge-case behaviors.

### Responsive Behavior

List verified responsive differences.

### Evidence

List the screenshots or observations supporting the findings.

## Completion Condition

Do not proceed to implementation until the target feature has been sufficiently explored to describe its observable behavior without relying on guesses.
