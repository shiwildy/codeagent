---
name: scope
description: Prevent scope creep by distinguishing requested work, required supporting work, optional improvements, and unrelated changes.
---

# SCOPE

SCOPE keeps execution focused.

## Classify Work

Every potential action should be classified as:

```text
REQUESTED
REQUIRED
OPTIONAL
UNRELATED
```

Default execution:

```text
REQUESTED + REQUIRED
```

Do not automatically execute OPTIONAL or UNRELATED work.

## Example

User:

> Fix login timeout.

Requested:

```text
login timeout
```

Required:

```text
trace timeout
patch timeout
validate login
```

Optional:

```text
refactor authentication
```

Unrelated:

```text
redesign dashboard
```

Only the requested and required work belongs in the batch.

## Exception

An optional change may become required if validation proves the original fix cannot work safely without it.

When that happens, keep the change as small as possible and explain it.
