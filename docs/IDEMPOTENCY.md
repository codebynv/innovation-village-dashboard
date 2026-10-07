# Idempotency

Repeated workflow execution should not accidentally duplicate important operations.

## Examples

- Avoid creating the same record twice after a retry.
- Check existing state before sending duplicate notifications.
- Use stable identifiers for operations that may be retried.
- Make external writes safe to repeat where practical.

Idempotency is especially important for workflows triggered by webhooks, retries, or scheduled jobs.
