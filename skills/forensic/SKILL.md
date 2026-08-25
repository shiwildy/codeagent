---
name: forensic
description: Perform root-cause debugging by tracing failures through the actual execution path instead of patching symptoms.
---

# FORENSIC

FORENSIC investigates why a failure happens.

## Core Rule

> Symptoms are evidence, not automatically the root cause.

## Workflow

```text
OBSERVATION
→ REPRODUCE OR TRACE
→ FOLLOW DATA/CONTROL FLOW
→ IDENTIFY ROOT CAUSE
→ PATCH
→ VALIDATE
```

## Trace

When possible, trace:

```text
INPUT
→ VALIDATION
→ STRATEGY/LOGIC
→ STATE
→ FILTERS
→ EXECUTION
→ EXTERNAL SYSTEM
→ RESULT
```

Use logs, source, configuration, and runtime behavior together.

## Avoid

Do not blindly patch based on:

- the last error message
- the first suspicious condition
- a single log line
- assumptions about how a module works

## Root Cause Standard

A root cause should explain the observed failure and identify a concrete point where behavior diverged from the intended contract.

If the root cause is uncertain, state the uncertainty rather than inventing certainty.
