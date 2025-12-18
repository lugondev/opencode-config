# OpenCode Workspace Config

This repository contains a minimal OpenCode configuration and related agent notes.

## What’s here

- `opencode.json`: OpenCode config, including MCP server definitions.
- `agent/`: Agent guidance and prompts.
- `package.json`: Node dependency for OpenCode plugins.

## Agents

### Development Agents
- `ag_typescript.md`: TypeScript/JavaScript (NestJS, Next.js 16+, React 19+)
- `ag_go.md`: Golang development
- `ag_rust.md`: Rust development
- `ag_anchor_sol.md`: Solana Anchor development
- `ag_solidity.md`: Solidity development (Foundry prioritized)

### Sub-agents
- `sag_analysis.md`: Requirements analysis and planning
- `sag_frontend-design.md`: Frontend UI/UX implementation
- `sag_review.md`: Code review and optimization
- `sag_write_testcase.md`: Test generation and validation

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
