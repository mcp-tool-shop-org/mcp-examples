---
title: Getting Started
description: Clone the repo and run your first MCP example workspace in under two minutes.
sidebar:
  order: 1
---

Get up and running with mcp-examples in under two minutes.

## Prerequisites

- Python 3.10 or later
- Git

## Clone the repo

```bash
git clone https://github.com/mcp-tool-shop-org/mcp-examples
cd mcp-examples
```

## Run hello-tools

The fastest way to see MCP in action:

```bash
cd hello-tools
python -m tools.echo.main "Hello, MCP!"
```

This runs a minimal echo tool that accepts input and returns it. No network, no writes, no side effects.

## Explore hello-filesystem

Once you are comfortable with hello-tools, move on to the filesystem example:

```bash
cd hello-filesystem
# Read the README first — this example demonstrates
# safe handling of irreversible side effects (file writes)
python -m tools.writer.main
```

hello-filesystem shows how MCP Tool Shop handles tools that perform real writes. Capability is always explicit and opt-in.

## Next steps

- [Examples](/mcp-examples/handbook/examples/) — Detailed walkthrough of each workspace.
- [Principles](/mcp-examples/handbook/principles/) — Why every example is built the way it is.
