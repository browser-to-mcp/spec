# Browser Workflow Tools for MCP

[Proposal](https://browser-to-mcp.github.io/spec/) |
[Source](index.bs) |
[Issues](https://github.com/browser-to-mcp/spec/issues)

---

This repository contains a draft contract and execution model for turning a
reviewed browser workflow into a narrow, typed MCP tool.

```text
workflow contract -> validation -> policy check -> replay -> typed result
```

The proposal covers workflow schemas, deterministic replay, MCP mapping,
permissions, assertions, redacted traces, provenance, and evaluation. It is an
early community proposal, not an official W3C or MCP standard.

### Repository contents

- [`index.bs`](index.bs) is the detailed standards-style source.
- [`index.html`](index.html) is the dependency-free publication served by
  GitHub Pages.
- [The issue tracker](https://github.com/browser-to-mcp/spec/issues) is the
  public place for design feedback and implementation evidence.

### Current scope

A reference implementation supports local, read-only workflow validation and
replay, generated MCP tools over STDIO, structured results, policy enforcement,
redacted traces, and read-only discovery of native WebMCP metadata. Native
WebMCP execution, authenticated workflows, writes, hosted browsers, and remote
transport remain outside the implemented scope.

The current execution-parity benchmark verifies internal runtime paths that all
share Playwright. It is not evidence that the project outperforms Playwright or
Playwright MCP. Product claims require a separate same-model comparison between
generic browser tools and generated workflow tools, together with safety and
resilience evaluation.

### Local preview

Open `index.html` directly, or serve this repository with any static file
server.

To validate the standards-style source when Bikeshed is available:

```bash
uvx bikeshed spec index.bs /tmp/browser-workflow-tools.html
```

### License

Apache-2.0.
