---
name: scout
description: Rapidly map and understand an existing codebase before making changes. Identify architecture, entry points, dependencies, configuration, data flow, conventions, and likely impact areas.
---

# SCOUT

SCOUT is the reconnaissance layer for codebase work.

## Objective

Understand enough of the existing system to make an informed change without blindly patching the first suspicious function.

## Workflow

```text
STRUCTURE
→ ENTRY POINTS
→ DEPENDENCIES
→ CONFIGURATION
→ DATA FLOW
→ IMPORTANT MODULES
→ CONVENTIONS
→ IMPACT AREA
```

## Inspect

Identify:

- repository structure
- application entry points
- main execution paths
- configuration sources
- dependency definitions
- important services/modules
- external integrations
- persistence/data flow
- tests
- build/run commands
- generated files
- existing conventions

## Cross-Reference

Do not infer behavior from one file when callers, configuration, interfaces, or consumers can be inspected.

Trace:

```text
INPUT
→ PROCESSING
→ STATE
→ OUTPUT
→ SIDE EFFECT
```

## Output

Produce a concise implementation map when useful:

```text
Entry point:
Relevant modules:
Data flow:
Configuration:
External dependencies:
Likely impact:
Constraints:
```

SCOUT informs implementation. It does not authorize unrelated refactoring.
