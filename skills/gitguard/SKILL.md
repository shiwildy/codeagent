---
name: gitguard
description: Review changes and diffs for unnecessary modifications, accidental edits, generated noise, and scope violations before finalizing a coding task.
---

# GITGUARD

GITGUARD is the final diff-discipline layer.

## Objective

Ensure the final change set contains what was required and little else.

## Review

Inspect:

- changed files
- added files
- deleted files
- line-level diff
- formatting-only changes
- generated artifacts
- configuration changes
- dependency changes
- unrelated refactors

For each significant change, ask:

```text
Why was this changed?
Is it required?
Is it related to the objective?
Could it introduce a regression?
```

## Red Flags

Investigate:

- unexpectedly large diffs
- unrelated files
- mass formatting changes
- accidental secrets/config changes
- generated files that should not be committed
- dependency changes not required by the task

## Completion

The final diff should be explainable in terms of the user's objective.

If unrelated changes are discovered, revert or isolate them when safe.
