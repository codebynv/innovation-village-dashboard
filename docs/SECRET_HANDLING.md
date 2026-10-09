# Secret Handling

- Store API keys and tokens in approved secret configuration.
- Never place secrets in source files or workflow payloads visible to users.
- Avoid logging authorization headers or credentials.
- Rotate credentials if they are accidentally exposed.
- Use the least privilege available for each integration.

An environment variable is a configuration mechanism, not a substitute for access control over deployment settings.
