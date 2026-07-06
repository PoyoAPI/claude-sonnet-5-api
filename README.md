# Claude Sonnet 5 API Examples for PoYo

[![Model page](https://img.shields.io/badge/Model%20page-claude-sonnet-5-84cc16)](https://poyo.ai/models/claude-sonnet-5)
[![API docs](https://img.shields.io/badge/API%20docs-docs.poyo.ai-22d3ee)](https://docs.poyo.ai/api-manual/chat-series/claude-messages)
[![License: MIT](https://img.shields.io/badge/License-MIT-111827)](LICENSE)
[![Main examples](https://img.shields.io/badge/Main%20examples-PoyoAPI%2Fpoyo--examples-0f172a?logo=github)](https://github.com/PoyoAPI/poyo-examples)

Focused server-side examples for building with `claude-sonnet-5` on PoYo.

Claude Sonnet 5 is useful for agentic coding, planning, browser or computer-use orchestration, long-context analysis, and production assistant workflows.

[Try on PoYo](https://poyo.ai/models/claude-sonnet-5) | [Get API Key](https://poyo.ai/dashboard/api-key) | [Docs](https://docs.poyo.ai/api-manual/chat-series/claude-messages) | [Pricing](https://poyo.ai/pricing) | [Main Examples](https://github.com/PoyoAPI/poyo-examples)

## What This Repo Covers

- Chat completions with `claude-sonnet-5`
- OpenAI-style `/v1/chat/completions` requests
- Node.js backend example
- Prompt examples and production integration notes

## Quick Start

```bash
cp .env.example .env
export POYO_API_KEY="your-api-key"
```

Run the Node.js example:

```bash
cd node
npm start
```

Keep `POYO_API_KEY` on the server. Do not expose it in browser code, mobile apps, screenshots, or public logs.

## Examples

| Path | What it covers |
| --- | --- |
| [`curl/generate.md`](curl/generate.md) | Copy-paste API request. |
| [`node/`](node/) | Native Node.js backend example. |
| [`docs/prompt-examples.md`](docs/prompt-examples.md) | Practical prompts for product workflows and creative tests. |
| [`docs/production-notes.md`](docs/production-notes.md) | Security and reliability notes before launch. |

## Run Checks

```bash
make check
```

On Windows:

```powershell
./scripts/check.ps1
```

## License

MIT
