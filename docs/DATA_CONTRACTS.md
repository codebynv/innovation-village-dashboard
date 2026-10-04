# Data Contracts

Automation workflows should exchange predictable structured data.

## Contract rules

- Define required fields explicitly.
- Validate data before external writes.
- Keep field names consistent between agents and workflows.
- Handle missing or invalid values explicitly.
- Document changes to important payload structures.

Stable contracts reduce failures when one agent or workflow is changed independently.
