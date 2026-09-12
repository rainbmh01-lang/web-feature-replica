# Implementation

## Purpose

Implement the analyzed reference feature inside the current project while preserving the project's existing architecture, conventions, and unrelated functionality.

Implementation must be based on the completed feature specification.

Do not begin implementation before the reference analysis and feature specification are sufficiently complete.

---

# 1. Inspect the Current Project

Before modifying anything, inspect the existing project.

Determine:

- framework
- language
- package manager
- application entry point
- routing
- component structure
- styling system
- state management
- data layer
- existing reusable components
- existing dependencies
- build system
- development commands
- testing setup

Do not assume the project uses a particular framework.

---

# 2. Identify the Correct Integration Point

Determine where the feature belongs.

Inspect:

- relevant routes
- relevant pages
- relevant components
- existing layouts
- existing state
- existing APIs
- existing utilities
- existing styles

Prefer integrating with existing structures instead of creating duplicate systems.

---

# 3. Preserve Existing Architecture

Follow the architecture already used by the project.

Do not:

- replace the framework
- replace the routing system
- replace the styling system
- replace the state management system
- rewrite unrelated components
- reorganize the entire project
- introduce a new dependency without a clear implementation requirement

Only change architecture when the requested feature genuinely requires it.

---

# 4. Map the Specification to the Project

Before coding, create an implementation mapping.

Example:

```text
Reference Component
        ↓
Current Project Component

Reference Interaction
        ↓
Current Project Event Handler

Reference State
        ↓
Current Project State

Reference Style
        ↓
Current Project Styling System
```
