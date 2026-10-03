# Workflow Failure Handling

Automation should fail visibly and predictably.

## Recommended pattern

    Trigger
      ↓
    Validate input
      ↓
    Execute action
      ↓
    Check result
      ↓
    Record outcome
      ↓
    Notify when intervention is required

## Failure rules

- Validate required fields before external writes.
- Avoid silently swallowing workflow errors.
- Keep enough execution context to diagnose failures.
- Make retries safe where possible.
- Separate temporary provider failures from permanent validation failures.

A workflow that completes successfully should leave the data layer and dashboard in a consistent state.
