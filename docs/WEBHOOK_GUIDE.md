# Webhook Guide

Webhook-driven workflows should assume requests can arrive more than once.

- Validate the incoming payload.
- Verify authentication or signature where supported.
- Use an idempotency strategy.
- Handle duplicate deliveries safely.
- Record execution status.
- Keep provider-specific assumptions isolated.

Never trust a webhook payload simply because it arrived at an expected endpoint.
