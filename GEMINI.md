# QBO Connector by Meridian

Use the `quickbooks-connector-by-meridian` MCP server whenever the user asks to
inspect, explain, report on, create, or update information in a connected
QuickBooks Online company.

## Authentication

If the connector is not yet authorized, ask the user to run:

```text
/mcp auth quickbooks-connector-by-meridian
```

Gemini CLI will open the Meridian authorization flow in the user's browser.

## Safe use

- Respect the access mode reported for each company. Do not attempt mutations
  on a read-only connection.
- When more than one company is connected, list the available companies first
  and use the opaque company identifier returned by this connector.
- Never guess a company identifier or reuse one obtained from another tool.
- Follow the connector's confirmation and idempotency requirements for writes.
- Use pagination when the user asks for all matching records.
