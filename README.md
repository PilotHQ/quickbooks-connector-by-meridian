# QuickBooks Connector by Meridian for Gemini CLI

Connect Gemini CLI to QuickBooks Online through the free, hosted
[QuickBooks Connector by Meridian](https://qbo-connector.meridian.pilot.com/).

The connector can work with multiple QuickBooks companies and supports both
read-only and read-and-write access. You choose the access level for each
company in Meridian.

## Install

```sh
gemini extensions install https://github.com/PilotHQ/quickbooks-connector-by-meridian
```

Restart Gemini CLI, then authorize the connector:

```text
/mcp auth quickbooks-connector-by-meridian
```

The browser flow lets you sign in to Meridian, connect QuickBooks companies,
and approve Gemini CLI's access. OAuth tokens are managed by Gemini CLI; this
repository contains no credentials or connector implementation code.

## Useful requests

- List the QuickBooks companies I have connected.
- Show this month's profit and loss statement.
- Find overdue invoices for this company.
- Create a draft invoice after showing me exactly what will be created.

## Security and support

- MCP endpoint: `https://qbo-connector.meridian.pilot.com/mcp`
- [Privacy policy](https://qbo-connector.meridian.pilot.com/privacy)
- [Terms of service](https://qbo-connector.meridian.pilot.com/terms)
- Support: `qbo-mcp@pilot.com`

The connector is operated by [Pilot](https://pilot.com/).
