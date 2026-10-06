# Retry Policy

Retries should be used for failures that are likely to be temporary.

## Retry candidates

- Temporary network failures
- Rate-limit responses
- Short-lived provider outages

## Do not blindly retry

- Invalid input
- Authentication failures
- Permission failures
- Deterministic validation errors

Where an action can be repeated, design it to be idempotent or check the previous execution before retrying.
