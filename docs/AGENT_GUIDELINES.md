# Agent Guidelines

## Agent responsibilities

Each agent should have one clear operational responsibility.

### Main Agent

- Interpret user intent.
- Select the appropriate specialist.
- Coordinate the workflow.
- Return a concise result.

### Stock Manager

- Read and update inventory data.
- Detect low-stock conditions.
- Validate structured fields before writes.

### Project Manager

- Handle project and client updates.
- Track status and revenue information.
- Trigger approved notifications.

### Email Agent

- Classify incoming messages.
- Draft structured responses.
- Keep sending actions behind explicit workflow controls.

### UGC Image Agent

- Analyze image requirements.
- Build generation prompts.
- Trigger the approved image workflow.

## Reliability

AI should decide or classify where useful, while deterministic workflow nodes perform validated external actions.
