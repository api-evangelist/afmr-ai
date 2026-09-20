---
name: Discover AFMR resources
description: Resolve the AFMR authority map, machine resource index, agent/tool index and publication status before relying on any AFMR document — the provider's own "machine action path".
api: openapi/afmr-ai-discovery-api-openapi.yml
operations: [getAfmrDiscovery, getMachineResourceIndex, getAgentAndToolIndex, getPublicationStatus]
generated: '2026-09-19'
method: generated
---

# Discover AFMR resources

No authentication is needed for any step. Every response is `application/json`, CORS-open, cached
`max-age=3600, must-revalidate`; a wrong path returns RFC 9457 `application/problem+json`.

1. **Resolve authority** — `getAfmrDiscovery` (`GET /.well-known/afmr.json`). Read
   `vocabulary.authority` (the governed AFMR 1.0 index on wulfkaal.github.io — afmr.ai does NOT
   mirror it), `protocols.mcp.endpoint` and `protocols.a2a.endpoint`.
2. **Enumerate what exists** — `getMachineResourceIndex` (`GET /resources.json`). Only URLs listed in
   `read_resources[]` / `protocol_endpoints[]` are published; do not guess paths.
3. **Find the agent surfaces** — `getAgentAndToolIndex` (`GET /agents.json`) for the A2A card + MCP
   manifest pair.
4. **Check lifecycle before citing** — `getPublicationStatus` (`GET /status.json`). Each component
   carries `status` (published / working-draft / pre-publication / operational / available). Treat a
   working-draft profile as a draft, and note `entries: 0` / `cards: 0` registries are empty by design.

Rules: read-only surface (no idempotency key needed); respect the provider's stated claim boundary —
discovery is not admission, admission is not trust, trust is not transaction authority.
