# Visual Analysis

## Purpose

Analyze the visual appearance of the target feature from the reference website before implementation.

The objective is high observable visual fidelity.

Do not redesign the feature.

Do not modernize the feature.

Do not substitute a different visual style.

The reference is the visual source of truth.

## 1. Overall Composition

Analyze the complete visible composition.

Record:

- viewport dimensions
- page background
- main content width
- content alignment
- major sections
- vertical and horizontal structure
- spacing between major sections
- fixed elements
- sticky elements
- overlays
- visible borders
- visible separators

Determine whether the layout is:

- centered
- full width
- constrained
- grid-based
- flex-based
- sidebar-based
- multi-column
- stacked

Record only observable characteristics.

## 2. Component Inventory

Identify every visually relevant component belonging to the target feature.

For each component record:

- component type
- position
- dimensions
- alignment
- spacing
- background
- border
- border radius
- shadow
- opacity
- icon
- text
- interactive appearance
- disabled appearance
- selected appearance

Do not omit small visible elements when they contribute to the feature's appearance.

## 3. Typography

Analyze all visible text belonging to the feature.

Record:

- font family when identifiable
- font size
- font weight
- line height
- letter spacing when noticeable
- text color
- text alignment
- capitalization
- wrapping behavior
- truncation behavior

Separate typography by semantic role:

- page title
- section title
- label
- body text
- helper text
- placeholder
- button text
- warning
- error
- success message

If the exact font cannot be verified, record the closest observable characteristics rather than inventing an exact font name.

## 4. Colors

Record observable colors for:

- page background
- component background
- primary text
- secondary text
- borders
- buttons
- links
- hover states
- focus states
- selected states
- disabled states
- warnings
- errors
- success messages

Prefer measured or inspected values when available.

Do not invent color values from memory.

## 5. Spacing

Analyze spacing systematically.

Record:

- outer margins
- section spacing
- component padding
- input padding
- button padding
- gaps between controls
- text-to-icon spacing
- label-to-input spacing
- row spacing
- column spacing

Pay particular attention to repeated spacing patterns.

## 6. Dimensions

Record important dimensions when they can be measured or reliably estimated.

Examples:

- container width
- input height
- button height
- icon size
- card width
- card height
- dialog width
- sidebar width
- thumbnail size
- gap sizes
- border thickness
- corner radius

Use relative measurements when exact pixel measurement is unavailable.

## 7. Icons and Graphics

For every icon or graphic belonging to the feature, record:

- type
- approximate size
- position
- visual style
- stroke/fill appearance
- surrounding spacing
- interaction state

Determine whether the icon is:

- text glyph
- SVG
- image
- CSS-generated
- icon library element

Do not copy proprietary graphic assets unless they are explicitly provided for reuse.

When an exact asset cannot legally or technically be reused, reproduce the observable visual role using an independent implementation.

## 8. Interactive Visual States

Inspect visual changes caused by interaction.

Analyze:

- default
- hover
- focus
- active
- selected
- disabled
- loading
- success
- warning
- error

For each state record exactly what changes:

- color
- border
- background
- shadow
- opacity
- icon
- text
- size
- position
- visibility

Do not assume that a state exists unless it is observable or required by an observed interaction.

## 9. Responsive Appearance

Compare relevant viewport sizes.

Record changes in:

- layout
- widths
- heights
- spacing
- typography
- visibility
- navigation
- controls
- wrapping
- stacking
- scrolling
- mobile-specific UI

Do not force desktop dimensions onto mobile layouts.

## 10. Visual Hierarchy

Describe the visual hierarchy of the feature.

Identify:

1. primary element
2. secondary elements
3. supporting information
4. warnings or important notices
5. tertiary controls

Record how hierarchy is created through:

- size
- weight
- contrast
- spacing
- position
- color
- borders
- shadows

## 11. Visual Evidence

For every major visual conclusion, prefer evidence from:

- screenshots
- browser inspection
- computed styles
- measured dimensions
- direct observation

Avoid subjective descriptions such as:

"looks modern"

"looks nice"

"looks professional"

Replace them with measurable or observable descriptions.

## 12. Visual Analysis Output

Produce a structured visual specification.

### Layout

- viewport:
- main container:
- alignment:
- columns/rows:
- major spacing:

### Components

For each component:

- name:
- type:
- dimensions:
- position:
- spacing:
- background:
- border:
- radius:
- shadow:

### Typography

For each text role:

- role:
- size:
- weight:
- line height:
- color:
- alignment:

### Colors

- background:
- primary text:
- secondary text:
- border:
- primary action:
- warning:
- error:
- success:

### Icons

For each icon:

- location:
- size:
- style:
- purpose:

### States

For each verified state:

- state:
- visual changes:

### Responsive Behavior

Record verified differences by viewport.

## Completion Condition

The visual analysis is complete only when the appearance of the target feature can be described precisely enough for another agent to implement it without relying primarily on visual guessing.
