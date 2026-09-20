---
name: Look up an AFMR failure mode via MCP
description: Use the public read-only MCP server at /api/rpc to resolve a permanent AFMR-F### identifier or a bounded text query to its canonical AFMR 1.0 record.
api: openapi/afmr-ai-discovery-api-openapi.yml
operations: [mcpJsonRpc]
mcp_tools: [lookup_failure_mode, discover_afmr]
generated: '2026-09-19'
method: generated
---

# Look up an AFMR failure mode via MCP

The REST surface does not serve failure-mode records (they live in the governed index on
wulfkaal.github.io); the MCP tool `lookup_failure_mode` does. Everything below is one operation,
`mcpJsonRpc` (`POST /api/rpc`, JSON-RPC 2.0, MCP 2025-11-25, Streamable HTTP, no auth).

1. `initialize` with `protocolVersion: "2025-11-25"`; the server answers with `tools` + `resources`
   capabilities and its `instructions`.
2. `tools/list` — four tools, all `readOnlyHint: true`, `idempotentHint: true`.
3. `tools/call` `lookup_failure_mode` with **either** `{"id": "AFMR-F010"}` (pattern
   `^AFMR-F[0-9]{3}$`) **or** `{"query": "<2-100 chars>", "limit": 1-10}`. The result's
   `structuredContent.matches[]` carries `id`, `class`, `name`, `definition`, `status`,
   `trigger_conditions[]`, `grounding_claims[]` and `institutional_antecedent`.
4. Do **not** open `GET /api/rpc` expecting SSE — it returns 405 `application/problem+json` with
   `Allow: POST, OPTIONS`; the server is stateless.

Cite `canonical_registry` from the response, not afmr.ai, as the authority for the record.
