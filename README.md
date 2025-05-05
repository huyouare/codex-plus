# codex-plus 🧦

## Features to Implement

### Core Features

- [ ] 1. MCP Support
  - See https://github.com/openai/codex/pull/270 and https://docs.anthropic.com/en/docs/agents-and-tools/claude-code/tutorials#set-up-model-context-protocol-mcp
  - This may take care of items 4 5, and 8.
- [ ] 2. Local Model Support
  - See https://github.com/openai/codex/issues/26
- [ ] 3. Cost Management
  - Cost tracking in progress: https://github.com/openai/codex/issues/117
  - See discussion on rate limit: https://github.com/openai/codex/discussions/328
- [ ] 4. Web Search Integration
  - See https://github.com/openai/codex/issues/259
- [ ] 5. Browser/Desktop Agent
- [ ] 6. Voice Input
  - See https://github.com/openai/codex/issues/418
- [ ] 7. Bash History Integration
  - See https://github.com/openai/codex/discussions/350 (kinda)
- [ ] 8. Memory
  - See https://github.com/openai/codex/discussions/323 and https://github.com/openai/codex/discussions/587 and https://github.com/openai/codex/discussions/341

## Installation

<details open>
<summary><strong>From npm (Recommended)</strong></summary>

```
TODO
```

</details>

<details>
<summary><strong>Build from source</strong></summary>

```bash
# Clone the repository
git clone https://github.com/huyouare/codex.git
cd codex

# Enable corepack
corepack enable

# Install dependencies and build
pnpm install
pnpm build

# Run the locally‑built CLI directly
node ./dist/cli.js

# Or link the command globally
pnpm link
```

</details>

## Contributing

We welcome contributions! Here's how to get started:

### Development Setup

1. Fork and clone the repository
2. Install dependencies: `pnpm install`
3. Enable Git hooks: `pnpm prepare`

### Development Workflow

```bash
# Watch mode (tests rerun on change)
pnpm test:watch

# Type‑check without emitting files
pnpm typecheck

# Automatically fix lint + prettier issues
pnpm lint:fix
pnpm format:fix
```

### Git Hooks

We use Husky to enforce code quality:

- **Pre-commit**: Runs lint-staged to format and lint files
- **Pre-push**: Runs tests and type checking

### Pull Request Process

1. Create a topic branch from `main` (e.g., `feat/web-search`)
2. Make your changes and add tests
3. Run all checks locally: `pnpm test && pnpm lint && pnpm typecheck`
4. Push and open a PR
5. Fill in the PR template explaining What/Why/How
6. Ensure all checks pass

## System Requirements

- Node.js 22 or newer (LTS recommended)
- macOS 12+, Ubuntu 20.04+/Debian 10+, or Windows 11 via WSL2
- Git (recommended)
- 4GB RAM minimum (8GB recommended)

## License

Apache-2.0 License
