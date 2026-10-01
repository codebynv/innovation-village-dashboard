# Innovation Village Architecture

## System layers

Innovation Village is organized around five logical layers:

    User Interaction
          ↓
    AI Decision Engine
          ↓
    n8n Automation
          ↓
    Operational Data
          ↓
    Dashboard / Insights

### 1. User Interaction

Users provide requests through the conversational interface or dashboard.

### 2. AI Decision Engine

AI agents interpret intent and decide which workflow or specialized agent should handle the request.

### 3. Automation Layer

n8n executes deterministic actions such as:

- reading and updating Google Sheets,
- sending or drafting email,
- triggering image workflows,
- coordinating sub-agents.

### 4. Operational Data

Google Sheets currently acts as the structured data layer. A future PostgreSQL migration can move persistent application data into a dedicated relational database.

### 5. Dashboard and Insights

The dashboard exposes operational state and derived metrics so users can inspect the results of automated workflows.

## Agent boundaries

The orchestrator should delegate domain-specific work rather than directly implementing every operation.

    Main Agent
      /    |         /     |       Stock  Project  Email
 Manager Manager   Agent
                    |
                Image / UGC
                   Agent

Each agent should have a narrow responsibility, explicit inputs, and predictable outputs.

## Reliability principles

- Keep AI interpretation separate from deterministic execution.
- Validate structured data before writing to external systems.
- Keep credentials outside source control.
- Make workflow failures observable.
- Prefer idempotent operations where repeated execution is possible.

## Future evolution

A PostgreSQL data layer, monitoring agent, reporting agent, and analytics agent can be added without changing the overall layered architecture.
