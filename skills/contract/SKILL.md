---
name: contract
description: Identify and preserve behavioral contracts, interfaces, inputs, outputs, side effects, configuration semantics, and external integrations during implementation.
---

# CONTRACT

CONTRACT defines what existing components promise to the rest of the system.

## Identify

Before changing a component, determine:

- inputs
- outputs
- return semantics
- exceptions/errors
- side effects
- state changes
- configuration dependencies
- API shape
- file/data formats
- external integrations
- timing/order assumptions

## Preserve

Unless explicitly requested, do not break existing contracts.

A patch should preserve:

```text
INPUT CONTRACT
OUTPUT CONTRACT
SIDE-EFFECT CONTRACT
CONFIG CONTRACT
API CONTRACT
```

## Change Management

If a contract must change to solve the problem:

1. Identify the affected consumers.
2. Update all required references.
3. Validate compatibility.
4. Report the contract change clearly.

Do not silently alter an interface just because another design seems cleaner.
