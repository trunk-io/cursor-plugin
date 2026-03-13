# Trunk Flaky Tests — Cursor Plugin

Flaky test detection, root cause analysis, and fix suggestions for development teams.

## What it does

This plugin connects Cursor to the [Trunk Flaky Tests](https://trunk.io) MCP server, giving you access to:

| Tool                  | Description                                                      |
| --------------------- | ---------------------------------------------------------------- |
| `fix-flaky-test`      | Retrieve root cause analysis and fix suggestions for flaky tests |
| `setup-trunk-uploads` | Generate a setup plan to upload test results to Trunk            |

## Install

Install from the [Cursor Marketplace](https://cursor.com/marketplace), or add manually to `.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "trunk": {
      "url": "https://mcp.trunk.io/mcp"
    }
  }
}
```

## Authorization

The Trunk MCP server uses **OAuth 2.0 + OpenID Connect**. When you first connect, you'll be prompted to authenticate via your Trunk account.

## Documentation

- [Trunk Flaky Tests docs](https://docs.trunk.io/flaky-tests)
- [MCP server docs](https://docs.trunk.io/flaky-tests/use-mcp-server)
- [Cursor setup guide](https://docs.trunk.io/flaky-tests/use-mcp-server/configuration/cursor-ide)

## License

MIT
