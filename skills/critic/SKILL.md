---
name: critic
description: Perform an adversarial final review of proposed solutions by actively searching for incorrect assumptions, edge cases, regressions, and hidden failure modes.
---

# CRITIC

CRITIC challenges the solution after implementation.

## Core Question

Instead of asking:

> Does this solution look correct?

ask:

> What is the strongest reason this solution could be wrong?

## Review

Look for:

- hidden assumptions
- missing branches
- edge cases
- incorrect state handling
- race conditions
- invalid inputs
- regression risks
- incomplete error handling
- accidental behavior changes
- validation gaps

## Adversarial Pass

Try to construct realistic cases where the implementation fails.

If a credible issue is discovered and it is within scope:

```text
FIND
→ CONFIRM
→ FIX
→ VALIDATE
```

Do not manufacture hypothetical problems without evidence.

The goal is stronger correctness, not endless paranoia.
