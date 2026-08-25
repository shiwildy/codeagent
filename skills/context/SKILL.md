---
name: context
description: Maintain structured project continuity so future requests can use compact, high-value state instead of repeatedly processing massive conversation history.
---

# CONTEXT

CONTEXT manages project knowledge across sessions.

## Preferred State

Maintain a structured project state containing:

```text
PROJECT
ARCHITECTURE
CURRENT STATE
REQUIREMENTS
CONSTRAINTS
IMPORTANT DECISIONS
KNOWN BUGS
RECENT CHANGES
TEST RESULTS
OPEN ISSUES
DO NOT CHANGE
```

## Principle

Prefer durable structured state over raw conversational history.

Do not repeatedly process:

- duplicate logs
- obsolete hypotheses
- superseded implementations
- irrelevant discussion

## Preserve

Never discard:

- explicit user constraints
- important architectural decisions
- current implementation state
- unresolved blockers
- latest validation results

## Update

After significant work, update the project state when the environment supports persistent state.

Keep it factual and concise.
