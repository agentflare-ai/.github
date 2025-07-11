# Contributing to AgentFlare

Thank you for your interest in contributing to AgentFlare! We're building the infrastructure for AI agents, and your help—whether through code, docs, or feedback—makes us better. This guide explains how to get involved.

## 📜 Code of Conduct

We follow the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct.html). By participating, you agree to uphold it. Report issues to [hello@agentflare.ai](mailto:hello@agentflare.ai).

## 🤔 How Can I Contribute?

### Reporting Bugs

- Use the [issue tracker](https://github.com/agentflare-ai/monorepo/issues) to report bugs.
- Check for duplicates first.
- Include: Description, steps to reproduce, expected vs. actual behavior, screenshots (if UI-related), and environment details (e.g., Node version, OS).

### Suggesting Features

- Open an issue with "[Feature Request]" in the title.
- Explain the problem it solves, proposed solution, and any alternatives considered.
- For AI-specific features (e.g., new observability metrics), include use cases like agent decision tracing.

### Submitting Pull Requests

1. **Fork the Repo**: Fork https://github.com/agentflare-ai/monorepo and clone your fork.
2. **Set Up Development**:
   - Install dependencies: `npm install` (or yarn/pnpm if using).
   - Use monorepo tools: If Nx/Turbo is set up, run `nx build` or `turbo run build`.
   - For AI testing: Set up env vars for models (e.g., API keys for OpenAI/Anthropic).
   - Run tests: `npm test`.
3. **Make Changes**:
   - Branch from `main`: `git checkout -b feature/your-feature`.
   - Follow code style: Use ESLint/Prettier (run `npm run lint`).
   - For SDKs: Ensure compatibility with TypeScript, Python, etc.
   - Add tests: Cover new features with unit/integration tests (e.g., Jest for JS, pytest for Python).
   - Update docs: Modify READMEs or https://docs.agentflare.ai as needed.
4. **Commit and Push**:
   - Use clear commit messages: e.g., "feat: add cost attribution to Telepathy".
   - Push to your fork.
5. **Open a PR**:
   - Target the `main` branch.
   - Reference related issues: e.g., "Closes #123".
   - Describe changes, why they're needed, and any risks (e.g., breaking changes in observability API).
   - We'll review and merge if it aligns!

### First-Time Contributors

Look for issues labeled "good first issue" or "help wanted". Start small, like fixing typos or adding examples to /examples.

## 🛠️ Development Setup

- **Requirements**: Node.js >=18, Python >=3.10, Git.
- **Monorepo Tips**: All projects are in one repo—use workspace commands for efficiency.
- **Testing AI Features**: Mock agents with sample data; avoid real API calls in CI.
- **Building**: Run `npm run build` for SDKs.
- **Debugging**: Use Telepathy's own tools for tracing during dev!

## 🎉 Acknowledgments

Shoutout to all contributors! Your work is credited in release notes.

Questions? Join our [Discord](https://discord.gg/agentflare) or email [hello@agentflare.ai](mailto:hello@agentflare.ai).

Let's build the future of AI agents together! 🚀
