# Workflow Test Plan

Test each automation with:

- valid input,
- missing required fields,
- malformed payloads,
- temporary provider failure,
- repeated delivery,
- partial completion,
- retry and recovery.

Verify the final data state, not just whether the workflow reports success. Ensure repeated runs do not create duplicate records or notifications.
