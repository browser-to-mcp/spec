# Browser Workflow Tools for MCP

Websites are full of useful actions that still have no API. This project
explores a practical way to turn a reviewed browser workflow into a typed,
traceable MCP tool.

In simple terms:

```text
reviewed workflow -> validation -> browser replay -> MCP tool
```

For example, a developer could expose `download_latest_invoice(customer_id)`
instead of asking an agent to rediscover the same clicks every time.

This repository contains the proposal for that idea. It is written to be
clear enough to implement, test, and challenge.

- [Read the live proposal](https://browser-to-mcp.github.io/spec/)

This is an early community proposal, not an official W3C or MCP standard.

## Local preview

Open `index.html` directly or serve this repository with a static file server.

## Bikeshed source

When Bikeshed is available:

```bash
uvx bikeshed spec index.bs index.html
```

## License

Apache-2.0.
