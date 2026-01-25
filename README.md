# MCP Examples

Example workspaces for [MCP Tool Shop](https://github.com/mcp-tool-shop).

## How MCP Tool Shop Fits Together

- **Registry** ([mcp-tool-registry](https://github.com/mcp-tool-shop/mcp-tool-registry)) → what tools exist
- **CLI** ([mcpt](https://github.com/mcp-tool-shop/mcpt)) → how you consume them
- **Examples** → how you learn the model (this repo)
- **Tags** (v0.1.0, v0.2.0) → stability, reproducibility
- **main** → development only, not for production
- **Tools default to least privilege** → no network, no writes, no side effects
- **Capability is always explicit and opt-in** → you decide when to enable

## Examples

| Example | Description |
|---------|-------------|
| [hello-tools](./hello-tools/) | Your first MCP workspace in 2 minutes |
| [hello-filesystem](./hello-filesystem/) | Irreversible side effects handled safely |

## Quick Start

```bash
cd hello-tools
python -m tools.echo.main "Hello, MCP!"
```

## Related

- [mcpt](https://github.com/mcp-tool-shop/mcpt) - CLI for discovering and running tools
- [mcp-tool-registry](https://github.com/mcp-tool-shop/mcp-tool-registry) - Tool metadata registry
