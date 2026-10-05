# Observability Notes

Automation becomes easier to operate when workflow outcomes are visible.

## Track

- workflow start and completion,
- validation failures,
- external API failures,
- retries,
- final action status.

## Principle

Logs should provide enough context to diagnose a failed workflow without storing sensitive payloads unnecessarily.

Where possible, give each workflow execution a traceable identifier.
