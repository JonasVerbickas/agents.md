# Agents Blueprint Repository

This repository holds “blueprint” instruction files for different project types. Each blueprint contains setup, testing, formatting, and linting guidelines so that various AI agents (e.g., OpenAI Codex, Anthropic Claude) can consume them correctly.

## Agent Compatibility

Different AI agents expect different filenames when loading instructions:

- **OpenAI Codex** expects a file named `AGENTS.md`.
- **Anthropic Claude** expects a file named `claude.md`.

To support both agents, you can duplicate or symlink your blueprint:

```bash
# for Node+TypeScript example
cp projectTypes/nodeWithTypescript.md projectTypes/AGENTS.md
cp projectTypes/nodeWithTypescript.md projectTypes/claude.md
```
