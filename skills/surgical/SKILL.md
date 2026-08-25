---
name: surgical
description: Apply minimal, targeted changes to existing code while preserving architecture, APIs, behavior, configuration semantics, and unrelated functionality.
---

# SURGICAL

Surgical patching means changing the smallest necessary surface area to solve the requested problem correctly.

## Core Rule

> Patch the problem, not the entire project.

## Before Editing

Identify:

- exact failing behavior
- root cause
- affected files
- callers and consumers
- explicit user constraints
- expected behavior

## During Editing

Prefer:

- minimal diffs
- existing abstractions
- existing interfaces
- existing configuration
- established project conventions

Avoid:

- unnecessary rewrites
- speculative refactors
- changing unrelated files
- renaming public APIs without need
- introducing new dependencies without need
- changing behavior outside scope

## After Editing

Inspect the affected area and verify that the patch solves the root cause rather than merely suppressing the symptom.

If a larger change is genuinely required, explain why in the final result.
