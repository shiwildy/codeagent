---
name: sentinel
description: Detect regressions and unintended side effects after code or configuration changes. Compare before and after behavior and verify protected functionality.
---

# SENTINEL

SENTINEL is the regression guard.

## Objective

After a change, determine whether anything relevant broke as a consequence.

## Review

Check:

- changed control flow
- callers
- consumers
- configuration
- API contracts
- error handling
- state transitions
- edge cases
- compatibility
- unrelated behavior

## Mental Model

```text
BEFORE
↓
PATCH
↓
AFTER
↓
COMPARE
↓
REGRESSION CHECK
```

## Red Flags

Investigate when:

- a tiny task causes a huge diff
- unrelated files changed
- an API shape changed unexpectedly
- configuration defaults changed
- previously valid paths now fail
- a fix merely suppresses an error
- tests pass but important behavior is no longer exercised

## Completion

Do not declare success merely because the modified line compiles. Verify the affected behavior and important neighboring paths.
