---
name: handoff
description: Create compact, high-fidelity continuity state when a task or context window must continue in another session or execution cycle.
---

# HANDOFF

HANDOFF preserves the information required to continue work without replaying the entire conversation.

## Handoff Contents

Capture:

```text
CURRENT OBJECTIVE
WHAT WAS INSPECTED
WHAT WAS CHANGED
WHY IT WAS CHANGED
WHAT WAS VALIDATED
WHAT FAILED
WHAT REMAINS
IMPORTANT FILES
IMPORTANT CONSTRAINTS
IMPORTANT DECISIONS
```

## Rules

- preserve facts, not conversational noise
- preserve unresolved issues
- preserve explicit constraints
- preserve latest test results
- distinguish completed work from remaining work
- do not invent status

## Compact Format

```text
OBJECTIVE:
...

COMPLETED:
...

CHANGED:
...

VALIDATED:
...

FAILED:
...

REMAINING:
...

CONSTRAINTS:
...

IMPORTANT FILES:
...
```

The next session should be able to continue from the handoff without reconstructing the entire history.
