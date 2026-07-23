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

## What it covers

- Human-reviewable workflow contracts.
- Typed MCP inputs and structured outputs.
- Deterministic browser replay.
- Domain and side-effect policies.
- Assertions, redacted traces, and provenance.

The first implementation target is local, read-only workflows.

## What it is not

This is not another generic browser-control server. Projects such as
Playwright MCP expose low-level browser actions for an agent. This proposal
defines the layer above that: a reviewed workflow becomes one reusable tool.

It also does not replace a website's API or WebMCP support. A runtime should
prefer those first and use browser replay when they are unavailable.

## Local preview

Open `index.html` directly or serve this repository with a static file server.

## Bikeshed source

When Bikeshed is available:

```bash
uvx bikeshed spec index.bs index.html
```

## License

Apache-2.0.
