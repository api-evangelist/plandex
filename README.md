# Plandex (plandex)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
