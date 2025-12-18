# OpenCode Workspace Config

This repository contains a minimal OpenCode configuration and related agent notes.

## What’s here

- `opencode.json`: OpenCode config, including MCP server definitions.
- `agent/`: Agent guidance and prompts.
- `package.json`: Node dependency for OpenCode plugins.

## Requirements

- Node.js (required for local MCP servers that run via `npx`)
- Python + `uv` (required for the local MCP server that runs via `uvx`)

## Install

Install Node dependencies using one of the following:

- `bun install` (recommended if you use Bun; `bun.lock` is present)
- `npm install`
- `pnpm install`

## MCP servers

The `opencode.json` file defines several MCP servers:

- `context7` (remote)
- `fetch` (local via `uvx mcp-server-fetch`)
- `docs-rs` (local via `npx @nuskey8/docs-rs-mcp@latest -y`)
- `memory` (local via `npx @modelcontextprotocol/server-memory`)
- `sequential-thinking` (local via `npx @modelcontextprotocol/server-sequential-thinking`)

If a local server fails to start, verify your Node/Python tooling is installed and available in your PATH.
