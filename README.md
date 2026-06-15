# Plandex (plandex)

Plandex is an open-source, terminal-based AI coding agent designed to take on large, multi-step software development tasks across many files in real world codebases. Written in Go and released under the MIT license, Plandex builds and executes long-running "plans" — durable, branchable units of work that combine intelligent context management, project maps generated with tree-sitter for 30+ programming languages, an effective 2M-token context window, and a cumulative diff review sandbox that isolates AI edits until a developer explicitly applies them. The tool ships as a CLI with an interactive REPL (fuzzy auto-complete), supports automated debugging of terminal commands and browser applications, integrates with Git for branching and commit-message generation, and is provider-neutral — working with Anthropic Claude, OpenAI, Google Gemini, OpenRouter.ai, Azure OpenAI, AWS Bedrock, DeepSeek, Perplexity, Ollama, and any OpenAI-compatible custom provider. The Plandex Server exposes a REST management/orchestration API (over 60 endpoints across accounts, orgs, projects, plans, branches, context, conversation, diffs, settings, model packs, and streaming execution) that powers both the CLI/REPL and the hosted Plandex Cloud. Plandex Cloud is winding down as of 2025-10-03; Plandex is now distributed primarily as a Docker-based self-hosted / local-mode product that users run with their own model-provider API keys.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- AI
- AI Coding Agent
- Developer Tools
- Open Source
- CLI
- Terminal
- LLM
- Coding Assistant
- Agents
- Go
- Context Management
- Plans
- Self-Hosted
- REST

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-29

## APIs

### Plandex Server API

Management and orchestration REST API exposed by the Plandex server (open-source, Go) used by the Plandex CLI/REPL to drive long-running coding plans across organizations, projects, plans, branches, context, conversation, model packs, and configuration. The same API powered Plandex Cloud (winding down 2025-10-03) and now powers self-hosted / local-mode deployments via Docker. Default local-mode bind is http://localhost:8099.

- **Human URL:** [https://docs.plandex.ai/development](https://docs.plandex.ai/development)
- **Base URL:** `http://localhost:8099`

#### Tags

- AI Coding Agent
- Plans
- REST
- Self-Hosted

#### Properties

- [Documentation](https://docs.plandex.ai)
- [Source Code](https://github.com/plandex-ai/plandex/tree/main/app/server)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/plandex/main/openapi/plandex-server-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-plan-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-context-item-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-branch-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-convo-message-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-model-pack-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-schema/plandex-server-plan-config-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-structure/plandex-server-plan-structure.json)
- [JSON Structure](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-structure/plandex-server-context-item-structure.json)
- [JSON Structure](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-structure/plandex-server-model-pack-structure.json)
- [Example](https://raw.githubusercontent.com/api-evangelist/plandex/main/examples/plandex-server-plan-example.json)
- [Example](https://raw.githubusercontent.com/api-evangelist/plandex/main/examples/plandex-server-context-item-example.json)
- [Example](https://raw.githubusercontent.com/api-evangelist/plandex/main/examples/plandex-server-convo-message-example.json)
- [Example](https://raw.githubusercontent.com/api-evangelist/plandex/main/examples/plandex-server-model-pack-example.json)
- [Example](https://raw.githubusercontent.com/api-evangelist/plandex/main/examples/plandex-server-plan-config-example.json)
- [Authentication](https://docs.plandex.ai/hosting/self-hosting/local-mode-quickstart)
- [Postman Collection](collections/plandex-server.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/plandex-server.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://plandex.ai)
- [Documentation](https://docs.plandex.ai)
- [Getting Started](https://docs.plandex.ai/quick-start)
- [Quickstart](https://docs.plandex.ai/hosting/self-hosting/local-mode-quickstart)
- [Install](https://plandex.ai/install.sh)
- [Git Hub](https://github.com/plandex-ai/plandex)
- [GitHub Organization](https://github.com/plandex-ai)
- [GitHub Repository](https://github.com/plandex-ai/plandex)
- [Source Code](https://github.com/plandex-ai/plandex)
- [License](https://github.com/plandex-ai/plandex/blob/main/LICENSE)
- [C L I](https://docs.plandex.ai/cli-reference)
- [R E P L](https://docs.plandex.ai/repl)
- [Pricing](https://docs.plandex.ai/hosting/cloud)
- [Privacy Policy](https://plandex.ai/privacy)
- [Terms of Service](https://plandex.ai/terms)
- [Security](https://docs.plandex.ai/security)
- [Blog](https://plandex.ai/blog)
- [Release Notes](https://github.com/plandex-ai/plandex/releases)
- [Changelog](https://github.com/plandex-ai/plandex/releases)
- [Support](https://github.com/plandex-ai/plandex/issues)
- [Discord](https://discord.gg/plandex-ai)
- [Twitter](https://twitter.com/plandex_ai)
- [YouTube](https://www.youtube.com/@plandex-ai)
- [Discussions](https://github.com/plandex-ai/plandex/discussions)
- [Issues](https://github.com/plandex-ai/plandex/issues)
- [Docker](https://hub.docker.com/r/plandexai/plandex-server)
- [Docker Compose](https://github.com/plandex-ai/plandex/blob/main/app/docker-compose.yml)
- [Spectral Rules](https://raw.githubusercontent.com/api-evangelist/plandex/main/rules/plandex-rules.yml)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/plandex/main/vocabulary/plandex-vocabulary.yml)
- [J S O N- L D](https://raw.githubusercontent.com/api-evangelist/plandex/main/json-ld/plandex-context.jsonld)
- [Plans](https://raw.githubusercontent.com/api-evangelist/plandex/main/plans/plandex-plans-pricing.yml)
- [Rate Limits](https://raw.githubusercontent.com/api-evangelist/plandex/main/rate-limits/plandex-rate-limits.yml)
- [Fin Ops](https://raw.githubusercontent.com/api-evangelist/plandex/main/finops/plandex-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
