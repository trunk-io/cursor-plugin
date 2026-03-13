# Trunk Flaky Tests — Cursor Plugin

Flaky test detection, root cause analysis, and fix suggestions for development teams.

## What it does

This plugin connects Cursor to the [Trunk Flaky Tests](https://trunk.io) MCP server, giving you AI-powered tools, commands, and built-in knowledge for debugging and fixing flaky tests.

### MCP Tools

| Tool                  | Description                                                      |
| --------------------- | ---------------------------------------------------------------- |
| `fix-flaky-test`      | Retrieve root cause analysis and fix suggestions for flaky tests |
| `setup-trunk-uploads` | Generate a setup plan to upload test results to Trunk            |

### Commands

| Command          | Description                                                  |
| ---------------- | ------------------------------------------------------------ |
| `fix-flaky`      | Get root cause analysis and apply a fix for a flaky test     |
| `why-flaky`      | Explain why a test is flaky without making changes           |
| `setup-uploads`  | Set up test result uploads to Trunk for your repository      |

### Skills

| Skill                  | Description                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------ |
| `flaky-test-patterns`  | Common flaky test patterns and fixes — activates when debugging or writing tests     |
| `trunk-ci-setup`       | CI pipeline best practices for test uploads — activates when editing CI config files |

### Rules

| Rule                     | Description                                                                  |
| ------------------------ | ---------------------------------------------------------------------------- |
| `flaky-test-awareness`   | Contextual awareness when editing test files — suggests Trunk tools when relevant |

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

## Also Available For

- [Claude Code](https://github.com/trunk-io/claude-code-plugin)
- [Any MCP client](https://github.com/trunk-io/mcp-server) (GitHub Copilot, Gemini CLI, and more)

## License

MIT
