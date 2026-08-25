---
name: testsmith
description: Automatically derive and execute practical validation for code changes. Create targeted tests or temporary checks when needed, diagnose failures, and rerun validation after fixes.
---

# TESTSMITH

TESTSMITH turns implementation into verified implementation.

## Core Rule

> A patch is not complete merely because it looks correct.

## Workflow

```text
UNDERSTAND EXPECTED BEHAVIOR
→ SELECT VALIDATION
→ RUN
→ INSPECT FAILURE
→ FIX
→ RUN AGAIN
```

## Validation Options

Use the strongest practical validation available:

- existing unit tests
- integration tests
- type checking
- compilation
- linting
- static analysis
- targeted runtime checks
- reproducible command-line checks
- temporary focused validation

Do not create an enormous testing framework for a small patch.

## Failure Handling

When validation fails:

1. Determine whether the failure is caused by the patch.
2. Identify the actual cause.
3. Fix within scope.
4. Rerun validation.

Do not simply report a failing test if the failure is clearly actionable within the current task.
