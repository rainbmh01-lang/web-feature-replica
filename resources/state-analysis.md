# State Analysis

## Purpose

Identify and document the observable states of the target feature.

The goal is to reproduce the feature's state model, including normal, transitional, exceptional, and boundary states.

Do not invent states that cannot be observed or logically required by verified behavior.

## 1. State Inventory

Identify every observable state belonging to the target feature.

Possible states include:

- initial
- empty
- populated
- selected
- unselected
- focused
- disabled
- enabled
- loading
- processing
- success
- error
- warning
- validation error
- completed
- cancelled
- partially completed
- unavailable

Only include states that are relevant to the feature.

## 2. Initial State

Document the state when the feature is first opened.

Record:

- visible elements
- hidden elements
- default values
- selected options
- enabled controls
- disabled controls
- placeholders
- instructional text
- available actions

## 3. Empty State

If the feature can contain no data, document:

- visible message
- available actions
- disabled controls
- placeholders
- empty containers
- visual treatment

Determine how the empty state differs from the initial state.

## 4. Populated State

When data is present, record:

- displayed content
- available controls
- changed labels
- enabled actions
- selected values
- thumbnails or previews
- additional information

## 5. Loading State

When processing occurs, inspect:

- loading indicator
- progress indicator
- changed text
- disabled controls
- hidden controls
- animation
- cancellation options
- background behavior

Document the transition into and out of loading.

## 6. Processing State

If processing is visually different from loading, document it separately.

Record:

- progress
- current operation
- affected controls
- user actions still allowed
- user actions blocked
- visual feedback

## 7. Success State

Document what happens after successful completion.

Record:

- success message
- changed interface
- new controls
- downloaded or generated result
- navigation
- reset behavior
- ability to repeat the operation

## 8. Error State

Document every verified error state.

For each error record:

- trigger
- message
- location
- visual appearance
- affected controls
- recovery action
- retry behavior
- whether previous input is preserved
- whether the interface returns to a previous state

## 9. Validation States

For inputs with validation, document:

- valid
- invalid
- empty
- partially valid
- boundary value
- corrected value

For each state record:

- input appearance
- message
- button state
- validation timing
- recovery behavior

## 10. Disabled State

Identify all controls that can become disabled.

For each one record:

- trigger
- visual appearance
- opacity
- cursor behavior
- whether tooltip or explanation exists
- condition for becoming enabled again

## 11. Selection States

For selectable elements document:

- unselected
- selected
- partially selected
- disabled selection
- select-all
- deselect-all

Record the visual and functional difference between each state.

## 12. Modal States

For dialogs and overlays document:

- closed
- opening
- open
- confirmation
- error
- loading
- closing

Record:

- overlay
- focus
- available actions
- close behavior
- background interaction

## 13. Navigation States

When the feature changes routes or views, record:

- previous location
- transition
- destination
- URL or route
- preserved state
- reset state

## 14. Responsive States

If the feature changes according to viewport size, document the relevant layouts separately.

For each viewport category record:

- layout
- visible controls
- hidden controls
- stacking
- scrolling
- typography
- spacing
- interaction differences

## 15. State Transition Matrix

Create a matrix:

| Current State | Trigger | Next State | Observable Changes |
| ------------- | ------- | ---------- | ------------------ |

Every important transition should be documented.

## 16. State Machine

Represent the main state flow when useful.

Example:

```text
Initial
  │
  ├── valid action ──→ Processing
  │                       │
  │                       ├── success ──→ Success
  │                       │
  │                       └── failure ──→ Error
  │
  └── invalid action ──→ Validation Error
```
