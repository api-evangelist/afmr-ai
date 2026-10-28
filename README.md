# Agent Failure Mode Registry

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

The Agent Failure Mode Registry (AFMR) is a reputation-integrity standard for agentic commerce. AFMR 1.0 is a published, citable vocabulary of 32 permanent failure-mode families in eight classes describing how autonomous agent systems fail as designed mechanisms; afmr.ai is the independent public front door and machine-discovery router for it. The site publishes a read-only Discovery API described by an OpenAPI 3.1 document (CC BY 4.0), a public read-only MCP server (Streamable HTTP at /api/rpc, listed in the official MCP Registry as ai.afmr/discovery), an A2A 1.0 agent card and JSON-RPC endpoint, llms.txt / llms-full.txt, a Reputation Attestation Working Draft 0.1 (human spec, JSON Schema 2020-12, verifier requirements), a pinned governance-and-voting binding, an intentionally empty endpoint-conformance registry and a configuration-only Lift Evidence index. The AFMR 1.0 vocabulary itself is governed from the editor's GitHub machine index and is not mirrored on afmr.ai.

**Areas:** Company · AI Agents · Agent Governance · Standards · Reputation · Failure Modes · Discovery · MCP · A2A · Machine-Readable Standards

## Agent Failure Mode Registry on APIs.io

Everything profiled for Agent Failure Mode Registry is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/afmr-ai/](https://apis.io/providers/afmr-ai/)** — or go straight to one of the APIs or properties below.

### APIs (17)

- [AFMR Discovery MCP Server](https://apis.io/apis/afmr-ai/afmr-discovery-mcp-server/) — Public read-only Model Context Protocol server (ai.afmr/discovery, MCP 2025-11-25, Streamable HTTP, stateless, no SSE listening stream) exposing four tools…
- [Agent Failure Mode Registry A2a API](https://apis.io/apis/afmr-ai/afmr-ai-a2a-api/) — The A2a API from Agent Failure Mode Registry — 1 operation(s) for a2a.
- [Agent Failure Mode Registry Agents.json API](https://apis.io/apis/afmr-ai/afmr-ai-agents-json-api/) — The Agents.json API from Agent Failure Mode Registry — 1 operation(s) for agents.json.
- [Agent Failure Mode Registry Changelog.json API](https://apis.io/apis/afmr-ai/afmr-ai-changelog-json-api/) — The Changelog.json API from Agent Failure Mode Registry — 1 operation(s) for changelog.json.
- [Agent Failure Mode Registry Evidence API](https://apis.io/apis/afmr-ai/afmr-ai-evidence-api/) — The Evidence API from Agent Failure Mode Registry — 1 operation(s) for evidence.
- [Agent Failure Mode Registry Feed.xml API](https://apis.io/apis/afmr-ai/afmr-ai-feed-xml-api/) — The Feed.xml API from Agent Failure Mode Registry — 1 operation(s) for feed.xml.
- [Agent Failure Mode Registry Lift Evidence API](https://apis.io/apis/afmr-ai/afmr-ai-lift-evidence-api/) — The Lift Evidence API from Agent Failure Mode Registry — 1 operation(s) for lift evidence.
- [Agent Failure Mode Registry Llms Full.txt API](https://apis.io/apis/afmr-ai/afmr-ai-llms-full-txt-api/) — The Llms Full.txt API from Agent Failure Mode Registry — 1 operation(s) for llms full.txt.
- [Agent Failure Mode Registry Llms.txt API](https://apis.io/apis/afmr-ai/afmr-ai-llms-txt-api/) — The Llms.txt API from Agent Failure Mode Registry — 1 operation(s) for llms.txt.
- [Agent Failure Mode Registry Registries API](https://apis.io/apis/afmr-ai/afmr-ai-registries-api/) — The Registries API from Agent Failure Mode Registry — 1 operation(s) for registries.
- [Agent Failure Mode Registry Resources.json API](https://apis.io/apis/afmr-ai/afmr-ai-resources-json-api/) — The Resources.json API from Agent Failure Mode Registry — 1 operation(s) for resources.json.
- [Agent Failure Mode Registry Rpc API](https://apis.io/apis/afmr-ai/afmr-ai-rpc-api/) — The Rpc API from Agent Failure Mode Registry — 1 operation(s) for rpc.
- [Agent Failure Mode Registry Server.json API](https://apis.io/apis/afmr-ai/afmr-ai-server-json-api/) — The Server.json API from Agent Failure Mode Registry — 1 operation(s) for server.json.
- [Agent Failure Mode Registry Sitemap.xml API](https://apis.io/apis/afmr-ai/afmr-ai-sitemap-xml-api/) — The Sitemap.xml API from Agent Failure Mode Registry — 1 operation(s) for sitemap.xml.
- [Agent Failure Mode Registry Standards API](https://apis.io/apis/afmr-ai/afmr-ai-standards-api/) — The Standards API from Agent Failure Mode Registry — 4 operation(s) for standards.
- [Agent Failure Mode Registry Status.json API](https://apis.io/apis/afmr-ai/afmr-ai-status-json-api/) — The Status.json API from Agent Failure Mode Registry — 1 operation(s) for status.json.
- [Agent Failure Mode Registry .well Known API](https://apis.io/apis/afmr-ai/afmr-ai-well-known-api/) — The .well Known API from Agent Failure Mode Registry — 3 operation(s) for .well known.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [AFMR Discovery](https://apis.io/servers/afmr-ai/ai-afmr-discovery/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Afmr Ai Agentic Access](https://apis.io/agentic-access/afmr-ai/afmr-ai-agentic-access/)

#### JSON Schema (1)

The data models the API reads and writes.

- [AFMR Reputation Attestation](https://apis.io/schemas/afmr-ai/afmr-ai-reputation-attestation-0.1/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Afmr Ai Discovery Api Overlay](https://apis.io/overlays/afmr-ai/afmr-ai-discovery-api-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Afmr Ai Authentication](https://apis.io/security/afmr-ai/afmr-ai-authentication/)
- [Afmr Ai Domain Security](https://apis.io/security/afmr-ai/afmr-ai-domain-security/)
- [Afmr Ai Vulnerability Disclosure](https://apis.io/security/afmr-ai/afmr-ai-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Afmr Ai Plans Pricing](https://apis.io/plans/afmr-ai/afmr-ai-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Afmr Ai Rate Limits](https://apis.io/rate-limits/afmr-ai/afmr-ai-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://afmr.ai/)
- [Documentation](https://afmr.ai/llms-full.txt)
- [Getting started](https://afmr.ai/llms.txt)
- [API reference](https://afmr.ai/openapi.json)
- [Changelog](https://afmr.ai/changelog.json)

## API Evangelist rating

**Kin Score 35.3** — thin · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 47.7 |
| Contract governance | 18.2 |
| Operational transparency | 36.8 |
| Developer ergonomics | 42.3 |
| Access clarity | 0.0 |

**Agent readiness 32.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | conformant |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 22.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/afmr-ai/](https://apis.io/providers/afmr-ai/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Agent Failure Mode Registry: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/afmr-ai/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
