---
title: Examples
description: Detailed walkthrough of every example workspace in mcp-examples.
sidebar:
  order: 2
---

Each example workspace teaches one concept. Start with hello-tools and work your way up.

## hello-tools

**Your first MCP workspace in 2 minutes.**

hello-tools is the simplest possible MCP workspace. It contains a small set of tools (echo, add, list) that run locally with zero side effects. Nothing touches the network. Nothing writes to disk.

What you learn:

- How an MCP workspace is structured (directory layout, tool modules, entry points).
- How to invoke a tool from the command line.
- That tools default to least privilege — no network, no writes, no side effects.

### Run it

```bash
cd hello-tools
python -m tools.echo.main "Hello, MCP!"
```

## hello-filesystem

**Irreversible side effects, handled safely.**

hello-filesystem introduces a tool that writes to the filesystem. This is the first example where something real happens — files get created. The workspace demonstrates how MCP Tool Shop handles irreversible actions through explicit capability grants.

What you learn:

- How side effects are declared and scoped.
- That capability is always opt-in — the tool cannot write unless you allow it.
- How to read a tool's capability requirements before running it.
- A pattern for handling irreversible actions safely in your own tools.

### Run it

```bash
cd hello-filesystem
# Read the README first to understand the capability model
python -m tools.writer.main
```

## Adding your own examples

Each example is a self-contained directory with its own README and tool modules. To add a new example, create a directory at the repo root with a clear name, a README explaining what it teaches, and one or more tool modules under a `tools/` subdirectory.
