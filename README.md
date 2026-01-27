# OpenCode Workspace Config

This repository contains a minimal OpenCode configuration and related agent notes.

## What’s here

-   `opencode.json`: OpenCode config, including MCP server definitions.
-   `agent/`: Agent guidance and prompts.
-   `package.json`: Node dependency for OpenCode plugins.

## AI Coding Skills

AI coding skills that enhance developer productivity. See [awesome-solana-ai](https://github.com/solana-foundation/awesome-solana-ai) for more resources.

### Solana Development

-   [solana-dev-skill](skills/solana-dev-skill/) - End-to-end Solana development skill. Covers wallet connections (wallet-standard-first), Anchor/Pinocchio programs, Codama-based client generation, testing with LiteSVM/Mollusk/Surfpool, and security best practices. Prefers `@solana/kit` for new client code.
-   [solana-anchor-claude-skill](skills/solana-anchor-claude-skill/) - End-to-end Solana development for Anchor and Solana Kit, focusing on modern, minimal, readable code. Testing with native JS test runners or LiteSVM.

### Debugging & Development

-   [be-debug-skill](skills/be-debug-skill/) - Backend debugging skill for systematic issue diagnosis and resolution.
-   [fe-skill](skills/fe-skill/) - Frontend development skill for UI implementation.
-   [web3-debug-skill](skills/web3-debug-skill/) - Web3-specific debugging for blockchain and smart contract issues.

## Agents

### Development Agents

-   `ag_typescript.md`: TypeScript/JavaScript (NestJS, Next.js 16.1+, React 19+)
-   `ag_go.md`: Golang development
-   `ag_rust.md`: Rust development
-   `ag_anchor_sol.md`: Solana Anchor development
-   `ag_solidity.md`: Solidity development (Foundry prioritized)

### Sub-agents

-   `sag_analysis.md`: Requirements analysis and planning
-   `sag_frontend-design.md`: Frontend UI/UX implementation
-   `sag_review.md`: Code review and optimization
-   `sag_write_testcase.md`: Test generation and validation
-   `sag_audit.md`: Code quality and security audit
-   `sag_force.md`: Autonomous task execution agent

## Requirements

-   Node.js (required for local MCP servers that run via `npx`)
-   Python + `uv` (required for the local MCP server that runs via `uvx`)

## Install

### 1. Clone Repository

Clone this repository to your local configuration directory (`~/.config/opencode`):

```bash
git clone https://github.com/lugondev/opencode-config.git ~/.config/opencode
```

### 2. Install Dependencies

Navigate to the directory and install dependencies:

```bash
cd ~/.config/opencode
bun install
# or
npm install
# or
pnpm install
```

## MCP servers

The `opencode.json` file defines several MCP servers:

-   `context7` (remote)
-   `fetch` (local via `uvx mcp-server-fetch`)
-   `docs-rs` (local via `npx @nuskey8/docs-rs-mcp@latest -y`)
-   `memory` (local via `npx @modelcontextprotocol/server-memory`)
-   `sequential-thinking` (local via `npx @modelcontextprotocol/server-sequential-thinking`)

If a local server fails to start, verify your Node/Python tooling is installed and available in your PATH.
