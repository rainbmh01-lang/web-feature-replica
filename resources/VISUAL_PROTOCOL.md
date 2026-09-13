# Mandatory Visual Inspection Protocol for Feature Replication

## 1. Trigger Condition
Whenever a replication task begins for any web feature, this protocol is automatically active and non-negotiable.

## 2. Hard Exit Criteria for Phase 1 (Reconnaissance)
Phase 1 CANNOT be completed and NO plan or code may be produced without generating:
1. Local screenshot files of the isolated feature captured via headless browser (Puppeteer / Edge / Playwright):
   - `original_idle.png`
   - `original_hover.png`
   - `original_focused.png`
   - `original_typing.png`
2. Explicit tool calls to `view_file` on EVERY captured screenshot.
3. A visual analysis directly comparing observed pixels against the replica.

## 3. Strictly Forbidden Shortcuts
- Stating "I inspected the DOM/network, so screenshots are not needed" is an explicit policy violation.
- Creating an implementation plan before visually inspecting screenshots is forbidden.
