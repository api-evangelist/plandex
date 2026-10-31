# Plandex

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

**Areas:** Artificial Intelligence · AI Coding Agents · Developer Tools · Open Source · CLI · Terminal · LLM · Coding Assistant · Agents · Go · Context Management · Plans

## Plandex on APIs.io

Everything profiled for Plandex is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/plandex/](https://apis.io/providers/plandex/)** — or go straight to one of the APIs or properties below.

### APIs (15)

- [Plandex Accounts API](https://apis.io/apis/plandex/plandex-accounts-api/) — User account, email verification, and authentication operations.
- [Plandex Branches API](https://apis.io/apis/plandex/plandex-branches-api/) — Per-plan branches for parallel exploration and diffing.
- [Plandex Context API](https://apis.io/apis/plandex/plandex-context-api/) — Files, directory trees, URLs, notes, and images loaded into a plan.
- [Plandex Conversation API](https://apis.io/apis/plandex/plandex-conversation-api/) — Prompts, responses, and rewind history within a plan branch.
- [Plandex Diffs API](https://apis.io/apis/plandex/plandex-diffs-api/) — Per-file pending changes, apply, and reject operations.
- [Plandex Execution API](https://apis.io/apis/plandex/plandex-execution-api/) — Streaming connect, build, tell, and stop endpoints for plan execution.
- [Plandex FileMap API](https://apis.io/apis/plandex/plandex-filemap-api/) — Tree-sitter project map generation and cached map loading.
- [Plandex Health API](https://apis.io/apis/plandex/plandex-health-api/) — Operational health and version endpoints.
- [Plandex Invites API](https://apis.io/apis/plandex/plandex-invites-api/) — Invite users into an org and manage pending invites.
- [Plandex Models API](https://apis.io/apis/plandex/plandex-models-api/) — Model packs, custom models, custom providers, default settings.
- [Plandex Orgs API](https://apis.io/apis/plandex/plandex-orgs-api/) — Organization and role membership management.
- [Plandex Plans API](https://apis.io/apis/plandex/plandex-plans-api/) — Long-running, branchable units of AI coding work over loaded context.
- [Plandex Projects API](https://apis.io/apis/plandex/plandex-projects-api/) — Project containers that group plans, mapped to a working directory.
- [Plandex Settings API](https://apis.io/apis/plandex/plandex-settings-api/) — Per-plan model settings, default settings, and org/user config.
- [Plandex Users API](https://apis.io/apis/plandex/plandex-users-api/) — User listing and removal within an org.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Plandex Agentic Access](https://apis.io/agentic-access/plandex/plandex-agentic-access/)

#### JSON Schema (6)

The data models the API reads and writes.

- [Branch](https://apis.io/schemas/plandex/plandex-server-branch/)
- [ContextItem](https://apis.io/schemas/plandex/plandex-server-context-item/)
- [ConvoMessage](https://apis.io/schemas/plandex/plandex-server-convo-message/)
- [ModelPack](https://apis.io/schemas/plandex/plandex-server-model-pack/)
- [Plan](https://apis.io/schemas/plandex/plandex-server-plan/)
- [PlanConfig](https://apis.io/schemas/plandex/plandex-server-plan-config/)

#### JSON Structure (3)

Data models expressed in JSON Structure.

- [Plandex Server Context Item Structure](https://apis.io/json-structure/plandex/plandex-server-context-item-structure/)
- [Plandex Server Model Pack Structure](https://apis.io/json-structure/plandex/plandex-server-model-pack-structure/)
- [Plandex Server Plan Structure](https://apis.io/json-structure/plandex/plandex-server-plan-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Plandex Context](https://apis.io/jsonld/plandex/plandex-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Plandex Vocabulary](https://apis.io/vocabularies/plandex/plandex-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Plandex Server Context Item Example](https://apis.io/examples/plandex/plandex-server-context-item-example/)
- [Plandex Server Convo Message Example](https://apis.io/examples/plandex/plandex-server-convo-message-example/)
- [Plandex Server Model Pack Example](https://apis.io/examples/plandex/plandex-server-model-pack-example/)
- [Plandex Server Plan Config Example](https://apis.io/examples/plandex/plandex-server-plan-config-example/)
- [Plandex Server Plan Example](https://apis.io/examples/plandex/plandex-server-plan-example/)

#### Collections (31)

Postman and Open Collection request collections.

- [Plandex Server Accounts API](https://apis.io/collections/plandex/open-plandex-accounts-api/)
- [Plandex Server Accounts Branches API](https://apis.io/collections/plandex/open-plandex-branches-api/)
- [Plandex Server Accounts Context API](https://apis.io/collections/plandex/open-plandex-context-api/)
- [Plandex Server Accounts Conversation API](https://apis.io/collections/plandex/open-plandex-conversation-api/)
- [Plandex Server Accounts Diffs API](https://apis.io/collections/plandex/open-plandex-diffs-api/)
- [Plandex Server Accounts Execution API](https://apis.io/collections/plandex/open-plandex-execution-api/)
- [Plandex Server Accounts FileMap API](https://apis.io/collections/plandex/open-plandex-filemap-api/)
- [Plandex Server Accounts Health API](https://apis.io/collections/plandex/open-plandex-health-api/)
- [Plandex Server Accounts Invites API](https://apis.io/collections/plandex/open-plandex-invites-api/)
- [Plandex Server Accounts Models API](https://apis.io/collections/plandex/open-plandex-models-api/)
- [Plandex Server Accounts Orgs API](https://apis.io/collections/plandex/open-plandex-orgs-api/)
- [Plandex Server Accounts Plans API](https://apis.io/collections/plandex/open-plandex-plans-api/)
- [Plandex Server Accounts Projects API](https://apis.io/collections/plandex/open-plandex-projects-api/)
- [Plandex Server API](https://apis.io/collections/plandex/open-plandex-server/)
- [Plandex Server Accounts Settings API](https://apis.io/collections/plandex/open-plandex-settings-api/)
- [Plandex Server Accounts Users API](https://apis.io/collections/plandex/open-plandex-users-api/)
- [Plandex Server Accounts API](https://apis.io/collections/plandex/postman-plandex-accounts-api/)
- [Plandex Server Accounts Branches API](https://apis.io/collections/plandex/postman-plandex-branches-api/)
- [Plandex Server Accounts Context API](https://apis.io/collections/plandex/postman-plandex-context-api/)
- [Plandex Server Accounts Conversation API](https://apis.io/collections/plandex/postman-plandex-conversation-api/)
- [Plandex Server Accounts Diffs API](https://apis.io/collections/plandex/postman-plandex-diffs-api/)
- [Plandex Server Accounts Execution API](https://apis.io/collections/plandex/postman-plandex-execution-api/)
- [Plandex Server Accounts FileMap API](https://apis.io/collections/plandex/postman-plandex-filemap-api/)
- [Plandex Server Accounts Health API](https://apis.io/collections/plandex/postman-plandex-health-api/)
- [Plandex Server Accounts Invites API](https://apis.io/collections/plandex/postman-plandex-invites-api/)
- …and 6 more published on APIs.io

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Plandex — jsonschema rules](https://apis.io/rules/plandex/plandex-jsonschema-spectral-rules/)
- [Plandex API Rules](https://apis.io/rules/plandex/plandex-rules/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Plandex Authentication](https://apis.io/security/plandex/plandex-authentication/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Plandex Plans Pricing](https://apis.io/plans/plandex/plandex-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Plandex Rate Limits](https://apis.io/rate-limits/plandex/plandex-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Plandex Finops](https://apis.io/finops/plandex/plandex-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://plandex.ai)
- [Documentation](https://docs.plandex.ai)
- [Getting started](https://docs.plandex.ai/quick-start)
- [Pricing](https://docs.plandex.ai/hosting/cloud)
- [Support](https://github.com/plandex-ai/plandex/issues)
- [Changelog](https://github.com/plandex-ai/plandex/releases)
- [Blog](https://plandex.ai/blog)
- [Security](https://docs.plandex.ai/security)
- [Terms of service](https://plandex.ai/terms)
- [Privacy policy](https://plandex.ai/privacy)
- [GitHub](https://github.com/plandex-ai)

## API Evangelist rating

**Kin Score 38.9** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 59.0 |
| Contract governance | 27.3 |
| Operational transparency | 31.6 |
| Developer ergonomics | 27.4 |
| Access clarity | 23.7 |

**Agent readiness 22.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 19.1** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/plandex/](https://apis.io/providers/plandex/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Plandex: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/plandex/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
