# Workflow Timeouts

Every external request should have a timeout appropriate to the operation.

- Avoid indefinite waits.
- Distinguish timeout from a valid empty response.
- Retry only when safe.
- Record the workflow execution identifier.
- Keep partial completion visible.
- Avoid duplicate writes when a timed-out request may have succeeded remotely.

Timeout handling should leave the workflow in a diagnosable state.
