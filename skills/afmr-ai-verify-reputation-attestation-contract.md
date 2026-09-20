---
name: Fetch the Reputation Attestation contract
description: Pull the Working Draft 0.1 specification, JSON Schema and verifier requirements, plus the (empty) endpoint-conformance registry, so an attestation can be validated fail-closed.
api: openapi/afmr-ai-discovery-api-openapi.yml
operations: [getReputationAttestationSpecification, getReputationAttestationSchema, getVerifierRequirements, getEndpointConformanceRegistry, getGovernanceVotingContract]
generated: '2026-09-19'
method: generated
---

# Fetch the Reputation Attestation contract

1. `getReputationAttestationSchema` (`GET /standards/reputation-attestation/0.1/schema.json`,
   `application/schema+json`, JSON Schema 2020-12). Validate the whole candidate attestation against
   it first (verifier requirement V-02). The root requires `type` const `AFMRReputationAttestation`
   and `profile` const `https://afmr.ai/standards/reputation-attestation/0.1`.
2. `getVerifierRequirements` (`GET /standards/reputation-attestation/0.1/verifier.json`). Apply
   V-01…V-nn in order; outcomes are exactly `valid`, `invalid` or `indeterminate` — missing
   authoritative material is `indeterminate`, never `valid`.
3. `getEndpointConformanceRegistry` (`GET /registries/endpoints/v0.1/index.json`). As of
   2026-09-19 `entries` is `[]` and status is `pre-publication`: no endpoint is represented as
   conforming, so any candidate that cites one must resolve `indeterminate`.
4. `getGovernanceVotingContract` (`GET /standards/governance-voting/1.0/contract.json`) for the pinned
   definitions of governance / vote / standing referenced by an attestation's `governance` object.
5. `getReputationAttestationSpecification` (`text/html`) is the human-readable normative text.

Errors: unknown paths return 404 `application/problem+json`; there are no auth or rate-limit
signals. Fail closed on any conflict between these documents and the candidate.
