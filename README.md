# Plandex (plandex)

Plandex is an open-source, terminal-based AI coding agent designed to take on large, multi-step software development tasks across many files in real-world codebases. Written in Go and released under the MIT license, Plandex builds and executes long-running "plans" — durable, branchable units of work that combine intelligent context management, tree-sitter project maps for 30+ programming languages, an effective 2M-token context window, and a cumulative diff review sandbox that isolates AI edits until a developer explicitly applies them. The tool ships as a CLI with an interactive REPL (fuzzy auto-complete), supports automated debugging of terminal commands and browser applications, integrates with Git for branching and commit-message generation, and is provider-neutral. The Plandex Server exposes a REST management/orchestration API (60+ endpoints) that powers both the CLI/REPL and the hosted Plandex Cloud. Plandex Cloud is winding down as of 2025-10-03; Plandex is now primarily a Docker-based self-hosted / local-mode product.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party
- **License:** MIT
- **Language:** Go
- **Governance:** PlandexAI Inc.

## Tags

 - AI, AI Coding Agent, Developer Tools, Open Source, CLI, Terminal, LLM, Coding Assistant, Agents, Go, Context Management, Plans, Self-Hosted, REST

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-29

## APIs

### Plandex Server API

Management and orchestration REST API exposed by the Plandex server (open-source, Go) used by the Plandex CLI/REPL to drive long-running coding plans across organizations, projects, plans, branches, context, conversation, model packs, and configuration. The same API powered Plandex Cloud (winding down 2025-10-03) and now powers self-hosted / local-mode deployments via Docker. Default local-mode bind is `http://localhost:8099`.

**Human URL:** [https://docs.plandex.ai/development](https://docs.plandex.ai/development)

**Base URL:** http://localhost:8099

#### Tags

 - AI Coding Agent, Plans, REST, Self-Hosted

#### Properties

- [Documentation](https://docs.plandex.ai)
- [SourceCode](https://github.com/plandex-ai/plandex/tree/main/app/server)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/plandex/main/openapi/plandex-server-openapi.yml)
- [JSONSchema — Plan](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-plan-schema.json)
- [JSONSchema — ContextItem](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-context-item-schema.json)
- [JSONSchema — Branch](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-branch-schema.json)
- [JSONSchema — ConvoMessage](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-convo-message-schema.json)
- [JSONSchema — ModelPack](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-model-pack-schema.json)
- [JSONSchema — PlanConfig](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-plan-config-schema.json)
- [JSONStructure — Plan](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-structure/plandex-server-plan-structure.json)
- [JSONStructure — ContextItem](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-structure/plandex-server-context-item-structure.json)
- [JSONStructure — ModelPack](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-structure/plandex-server-model-pack-structure.json)
- [Example — Plan](https://raw.githubusercontent.com/api-evangelist/plandex/main/examples/plandex-server-plan-example.json)
- [Example — ContextItem](https://raw.githubusercontent.com/api-evangelist/plandex/main/examples/plandex-server-context-item-example.json)
- [Example — ConvoMessage](https://raw.githubusercontent.com/api-evangelist/plandex/main/examples/plandex-server-convo-message-example.json)
- [Example — ModelPack](https://raw.githubusercontent.com/api-evangelist/plandex/main/examples/plandex-server-model-pack-example.json)
- [Example — PlanConfig](https://raw.githubusercontent.com/api-evangelist/plandex/main/examples/plandex-server-plan-config-example.json)
- [Authentication](https://docs.plandex.ai/hosting/self-hosting/local-mode-quickstart)

## Common Properties

- [Website](https://plandex.ai)
- [Documentation](https://docs.plandex.ai)
- [GettingStarted](https://docs.plandex.ai/quick-start)
- [Quickstart](https://docs.plandex.ai/hosting/self-hosting/local-mode-quickstart)
- [Install](https://plandex.ai/install.sh)
- [GitHub](https://github.com/plandex-ai/plandex)
- [GitHubOrganization](https://github.com/plandex-ai)
- [GitHubRepository](https://github.com/plandex-ai/plandex)
- [SourceCode](https://github.com/plandex-ai/plandex)
- [License — MIT](https://github.com/plandex-ai/plandex/blob/main/LICENSE)
- [CLI](https://docs.plandex.ai/cli-reference)
- [REPL](https://docs.plandex.ai/repl)
- [Pricing](https://docs.plandex.ai/hosting/cloud)
- [PrivacyPolicy](https://plandex.ai/privacy)
- [TermsOfService](https://plandex.ai/terms)
- [Security](https://docs.plandex.ai/security)
- [Blog](https://plandex.ai/blog)
- [ReleaseNotes](https://github.com/plandex-ai/plandex/releases)
- [Support](https://github.com/plandex-ai/plandex/issues)
- [Discord](https://discord.gg/plandex-ai)
- [Twitter](https://twitter.com/plandex_ai)
- [YouTube](https://www.youtube.com/@plandex-ai)
- [Discussions](https://github.com/plandex-ai/plandex/discussions)
- [Issues](https://github.com/plandex-ai/plandex/issues)
- [Docker Hub](https://hub.docker.com/r/plandexai/plandex-server)
- [docker-compose.yml](https://github.com/plandex-ai/plandex/blob/main/app/docker-compose.yml)

## Artifacts

| Type | File |
|---|---|
| OpenAPI | [openapi/plandex-server-openapi.yml](openapi/plandex-server-openapi.yml) |
| JSON Schema | [json-schema/](json-schema/) — Plan, ContextItem, Branch, ConvoMessage, ModelPack, PlanConfig |
| JSON Structure | [json-structure/](json-structure/) — Plan, ContextItem, ModelPack |
| JSON-LD | [json-ld/plandex-context.jsonld](json-ld/plandex-context.jsonld) |
| Examples | [examples/](examples/) — 5 example payloads |
| Spectral Rules | [rules/plandex-rules.yml](rules/plandex-rules.yml) |
| Vocabulary | [vocabulary/plandex-vocabulary.yml](vocabulary/plandex-vocabulary.yml) |
| Naftiko Capabilities | [capabilities/plandex-plan-management.yaml](capabilities/plandex-plan-management.yaml), [capabilities/plandex-context-and-diffs.yaml](capabilities/plandex-context-and-diffs.yaml) |
| Plans / Pricing | [plans/plandex-plans-pricing.yml](plans/plandex-plans-pricing.yml) |
| Rate Limits | [rate-limits/plandex-rate-limits.yml](rate-limits/plandex-rate-limits.yml) |
| FinOps | [finops/plandex-finops.yml](finops/plandex-finops.yml) |

## Features

- 2M-Token Effective Context Window
- Tree-Sitter Project Maps (30+ Languages)
- Cumulative Diff Sandbox
- Configurable Autonomy (None / Basic / Plus / Semi-Auto / Full-Auto)
- Automated Debugging Of Terminal + Browser Apps
- Model Packs (daily, reasoning, strong, cheap, oss, planner-specialized)
- Multi-Provider Support (Anthropic, OpenAI, Google, OpenRouter, Azure, Bedrock, DeepSeek, Perplexity, Ollama, custom)
- Claude Pro/Max Subscription Support
- Context Caching Across OpenAI, Anthropic, And Google
- Plan Version Control + Branching + Rewind
- Git Integration With Auto-Commit Option
- REPL With Fuzzy Auto-Complete
- One-Line CLI Install
- Background Tasks
- Smart Context + Auto-Load Context
- Streaming Plan Execution With Reconnect

## Solutions

- **Self-Hosted / Local Mode** — MIT-licensed, free, run via Docker with BYO model-provider keys.
- **Plandex Cloud — BYO API Key Mode (Historical)** — $30/month after trial; winding down 2025-10-03.
- **Plandex Cloud — Integrated Models Mode (Historical)** — $45/month + $20/mo of non-expiring credits; winding down 2025-10-03.
