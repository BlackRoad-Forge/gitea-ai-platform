<!-- BlackRoad SEO Enhanced -->

# gitea ai platform

> Part of **[BlackRoad OS](https://blackroad.io)** — Sovereign Computing for Everyone

[![BlackRoad OS](https://img.shields.io/badge/BlackRoad-OS-ff1d6c?style=for-the-badge)](https://blackroad.io)
[![BlackRoad Forge](https://img.shields.io/badge/Org-BlackRoad-Forge-2979ff?style=for-the-badge)](https://github.com/BlackRoad-Forge)
[![License](https://img.shields.io/badge/License-Proprietary-f5a623?style=for-the-badge)](LICENSE)

**gitea ai platform** is part of the **BlackRoad OS** ecosystem — a sovereign, distributed operating system built on edge computing, local AI, and mesh networking by **BlackRoad OS, Inc.**

## About BlackRoad OS

BlackRoad OS is a sovereign computing platform that runs AI locally on your own hardware. No cloud dependencies. No API keys. No surveillance. Built by [BlackRoad OS, Inc.](https://github.com/BlackRoad-OS-Inc), a Delaware C-Corp founded in 2025.

### Key Features
- **Local AI** — Run LLMs on Raspberry Pi, Hailo-8, and commodity hardware
- **Mesh Networking** — WireGuard VPN, NATS pub/sub, peer-to-peer communication
- **Edge Computing** — 52 TOPS of AI acceleration across a Pi fleet
- **Self-Hosted Everything** — Git, DNS, storage, CI/CD, chat — all sovereign
- **Zero Cloud Dependencies** — Your data stays on your hardware

### The BlackRoad Ecosystem
| Organization | Focus |
|---|---|
| [BlackRoad OS](https://github.com/BlackRoad-OS) | Core platform and applications |
| [BlackRoad OS, Inc.](https://github.com/BlackRoad-OS-Inc) | Corporate and enterprise |
| [BlackRoad AI](https://github.com/BlackRoad-AI) | Artificial intelligence and ML |
| [BlackRoad Hardware](https://github.com/BlackRoad-Hardware) | Edge hardware and IoT |
| [BlackRoad Security](https://github.com/BlackRoad-Security) | Cybersecurity and auditing |
| [BlackRoad Quantum](https://github.com/BlackRoad-Quantum) | Quantum computing research |
| [BlackRoad Agents](https://github.com/BlackRoad-Agents) | Autonomous AI agents |
| [BlackRoad Network](https://github.com/BlackRoad-Network) | Mesh and distributed networking |
| [BlackRoad Education](https://github.com/BlackRoad-Education) | Learning and tutoring platforms |
| [BlackRoad Labs](https://github.com/BlackRoad-Labs) | Research and experiments |
| [BlackRoad Cloud](https://github.com/BlackRoad-Cloud) | Self-hosted cloud infrastructure |
| [BlackRoad Forge](https://github.com/BlackRoad-Forge) | Developer tools and utilities |

### Links
- **Website**: [blackroad.io](https://blackroad.io)
- **Documentation**: [docs.blackroad.io](https://docs.blackroad.io)
- **Chat**: [chat.blackroad.io](https://chat.blackroad.io)
- **Search**: [search.blackroad.io](https://search.blackroad.io)

---


[![CI](https://github.com/blackboxprogramming/gitea-ai-platform/actions/workflows/ci.yml/badge.svg)](https://github.com/blackboxprogramming/gitea-ai-platform/actions/workflows/ci.yml)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6.svg)](https://typescriptlang.org)
[![Cloudflare Workers](https://img.shields.io/badge/Cloudflare-Workers-F38020.svg)](https://workers.cloudflare.com)
[![Claude AI](https://img.shields.io/badge/Claude-code_review-CC785C.svg)](https://anthropic.com)
[![Gitea](https://img.shields.io/badge/Gitea-self--hosted-609926.svg)](https://gitea.io)

> **AI-powered Gitea automation on Cloudflare Workers** — Claude-powered PR code review, AI issue triage, auto-deploy webhooks, GitHub↔Gitea mirroring, and real-time dashboard.

## Features

- **AI Code Review** — Claude analyzes PRs for bugs, security issues, and style violations
- **Issue Triage** — Automatic priority and label assignment using AI classification
- **Auto Deploy** — Webhook-triggered deployments to Cloudflare Pages on push
- **GitHub Mirror** — Bi-directional sync between Gitea and GitHub repositories
- **Dashboard API** — Real-time deployment logs, repo stats, and activity feed

## Architecture

```
Gitea → Webhook → Cloudflare Worker → Claude API → PR Comment
                                     → Cloudflare Pages Deploy
                                     → GitHub Mirror Sync
```

## Endpoints

| Route | Method | Description |
|-------|--------|-------------|
| `/webhook/push` | POST | Handle push events, trigger deploys |
| `/webhook/pr` | POST | AI code review on pull requests |
| `/webhook/issue` | POST | AI issue triage and labeling |
| `/api/chat` | POST | Chat with AI about your codebase |
| `/api/mirror` | POST | Sync repo to GitHub |
| `/api/repos` | GET | List all repositories |
| `/api/deploys` | GET | Recent deployment logs |
| `/dashboard` | GET | Real-time dashboard UI |

## Deploy

```bash
cd worker
npm install
npx wrangler deploy
```

## Tech Stack

- **Runtime**: Cloudflare Workers (edge, globally distributed)
- **Language**: TypeScript
- **AI**: Anthropic Claude API with Workers AI fallback
- **Storage**: Cloudflare KV for deploy logs
- **Git**: Gitea API + GitHub API

## License

Proprietary — BlackRoad OS, Inc.
