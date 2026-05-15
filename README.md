# Shelby Toolkit

> Community-built tools for [Shelby Protocol](https://shelby.xyz) — decentralized hot storage on Aptos.

## What's inside

### 1. Storage Dashboard (`/dashboard`)

A web-based explorer for any Shelby Protocol storage account. Paste an address, see all blobs — sizes, expirations, file types, transaction links. All data sourced directly from on-chain APIs.

**[Live Demo →](https://jasekeee.github.io/shelby-toolkit/dashboard/)**

Features:
- Explore any account on shelbynet or testnet
- Visual expiration timeline — see which blobs expire soon
- Storage breakdown by file type (docs, data, media, code, binaries)
- Direct links to Aptos Explorer for every transaction
- Dark theme, responsive, zero dependencies
- No backend — reads directly from Shelby's Aptos API

### 2. Agent Skill (`/skill`)

A [SKILL.md](https://github.com/agentskills) for AI coding agents (Claude Code, Codex, Cursor, Gemini CLI, etc.) that teaches them to interact with Shelby Protocol.

Install in Claude Code:
```bash
/skill add https://github.com/Jasekeee/shelby-toolkit skill/SKILL.md
```

Or copy `skill/SKILL.md` to your `.claude/skills/`, `.cursor/rules/`, or equivalent directory.

Covers: upload, download, delete, account management, benchmarking, SDK usage, troubleshooting, networks, and configuration.

## Quick start

### Use the Dashboard
Just open `dashboard/index.html` in your browser, or visit the live demo link above.

### Use the Agent Skill
Copy `skill/SKILL.md` into your AI agent's skills directory and start asking it to interact with Shelby.

## Environment

- Tested on Apple M4 Pro, macOS
- Shelby CLI v0.0.29
- Networks: shelbynet, testnet (Early Access)

## Performance benchmarks

Real-world measurements from Almaty, Kazakhstan on Apple M4 Pro:

| File size | Upload time | Network |
|-----------|------------|---------|
| 0.3 KB    | 5.97s      | shelbynet |
| 10 KB     | 8.14s      | shelbynet |
| 100 KB    | 10.88s     | shelbynet |
| 1 MB      | 8.24s      | shelbynet |
| Download (3 files) | 1.2s | shelbynet |

Upload latency is relatively flat across small files, suggesting a fixed per-transaction overhead of ~6–8s. Download is significantly faster.

## Contributing

Issues and PRs welcome. If you find bugs in the dashboard or want to add commands to the skill, please open a PR.

## Links

- [Shelby Protocol](https://shelby.xyz)
- [Shelby Docs](https://docs.shelby.xyz)
- [Shelby Explorer](https://explorer.shelby.xyz)
- [Shelby GitHub](https://github.com/shelby)
- [Shelby Discord](https://discord.gg/GEDwKxKKdP)
- [Shelby Feedback](https://github.com/shelby/feedback)

## Author

**[Jasekeee](https://github.com/Jasekeee)** — Early Access participant since May 2026.

## License

MIT
