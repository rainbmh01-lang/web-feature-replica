# Interaction Analysis

## Purpose

Analyze how the target feature behaves when the user interacts with it.

The objective is to reproduce the observable interaction model of the reference feature as accurately as possible.

Do not redesign interactions.

Do not simplify interaction flows.

Do not invent behavior that was not observed.

## 1. Interactive Element Inventory

Identify every interactive element belonging to the target feature.

For each element record:

- element name
- element type
- location
- initial state
- available interaction
- expected result

Examples:

- button
- text input
- number input
- select
- checkbox
- radio button
- switch
- tab
- link
- dropdown
- modal
- file picker
- drag-and-drop area
- thumbnail
- pagination control
- close button

## 2. Interaction Matrix

Create an interaction matrix.

For each interaction record:

| Element | Initial State | User Action | Result | New State |
| ------- | ------------- | ----------- | ------ | --------- |

Test each relevant interaction independently.

Do not assume that visually similar controls behave identically.

## 3. Click Behavior

For clickable elements determine:

- what happens on click
- whether the element changes state
- whether another element appears
- whether a dialog opens
- whether navigation occurs
- whether content changes
- whether the button becomes disabled
- whether a notification appears
- whether the action is reversible

Record the exact observable result.

## 4. Input Behavior

For every input determine:

- accepted input type
- default value
- placeholder
- minimum value
- maximum value
- decimal support
- negative value behavior
- empty value behavior
- invalid value behavior
- formatting behavior
- validation timing
- validation message
- whether changes occur immediately or after confirmation

Test realistic boundary values when possible.

## 5. Keyboard Behavior

When relevant, test:

- Tab
- Shift + Tab
- Enter
- Escape
- Space
- Arrow keys
- Backspace
- Delete
- relevant shortcuts

Record:

- focus order
- activation behavior
- menu navigation
- dialog closing
- input behavior
- shortcut behavior

Do not invent keyboard shortcuts.

## 6. Focus Behavior

Inspect:

- initial focus
- focus indicator
- focus movement
- focus trapping
- focus restoration
- behavior after closing dialogs
- behavior after submitting forms

Record only observable behavior.

## 7. Hover Behavior

When relevant, inspect hover states.

Record changes to:

- color
- background
- border
- shadow
- cursor
- tooltip
- icon
- text

Do not treat hover-only visual changes as functional behavior unless they affect interaction.

## 8. Selection Behavior

For selectable elements determine:

- single selection or multiple selection
- default selection
- selection indicator
- deselection behavior
- select-all behavior
- deselect-all behavior
- selection persistence
- selection limits

Record exactly what changes after selection.

## 9. Dropdowns and Menus

For every dropdown or menu determine:

- opening action
- position
- available options
- selected option
- keyboard behavior
- outside-click behavior
- Escape behavior
- closing behavior
- scrolling behavior
- disabled options

Record the complete observable flow.

## 10. Modal and Dialog Behavior

For every dialog determine:

- opening trigger
- position
- size
- overlay
- close button
- outside-click behavior
- Escape behavior
- confirmation behavior
- cancellation behavior
- focus behavior
- resulting state

## 11. File Interaction

When the feature involves files, determine:

- supported file types
- upload method
- drag-and-drop behavior
- upload progress
- loading state
- invalid-file behavior
- duplicate-file behavior
- file removal
- replacement behavior
- cancellation
- processing state
- completion state
- error state

Do not upload private or sensitive files to the reference website.

Use safe test files when testing upload behavior.

## 12. Drag and Drop

When relevant, test:

- draggable elements
- valid drop targets
- invalid drop targets
- drag-over appearance
- drop result
- cancellation
- ordering changes
- movement restrictions

Record observable behavior only.

## 13. Navigation

Determine whether an interaction causes:

- URL change
- route change
- modal navigation
- tab change
- page reload
- external navigation
- browser history change

Record the resulting URL or route when it is observable.

## 14. Loading Behavior

When an action requires processing, inspect:

- loading indicator
- disabled controls
- progress indicator
- placeholder state
- skeleton state
- text changes
- cancellation
- completion transition

Record the transition:

Idle
→ Loading
→ Success

or:

Idle
→ Loading
→ Error

## 15. Error Behavior

Test reasonable invalid actions and inputs.

Record:

- trigger
- error message
- error location
- visual appearance
- affected controls
- whether the user can correct the problem
- whether the error disappears automatically
- whether retry is available

Do not intentionally perform destructive actions.

## 16. Success Behavior

When an action succeeds, record:

- visual confirmation
- message
- changed controls
- navigation
- downloaded file
- updated content
- reset behavior
- ability to repeat the action

## 17. State Transitions

Represent important interactions as state transitions.

Example:

```text
Initial
  ↓
User enters valid value
  ↓
Value accepted
  ↓
User activates action
  ↓
Loading
  ↓
Success
```
