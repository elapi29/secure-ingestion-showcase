# Demo Script

## Goal

Communicate a validated secure-ingestion baseline before downstream AI / analytics / clinical workflow use.

## Open with

“This showcase demonstrates a secure ingress layer for sensitive clinical metadata. The goal is to verify, validate, record, and control release before downstream AI or analytics systems receive anything.”

## Step 1 — Architecture overview

Show:

- `docs/architecture-overview.png`
- optionally `docs/architecture-overview-v2.jpeg`

Talk track:

- metadata is protected before handoff
- secure backend ingest verifies and validates before release
- downstream use is controlled, not implicit
- the platform is about trusted ingress, not just transport

## Step 2 — Bronze and audit model

Show:

- `docs/bronze-flow.png`

Talk track:

- accepted metadata becomes a Bronze record
- evidence and release trace are persisted separately in Audit
- this creates a cleaner boundary between operational ingest and downstream usage evidence
- tenant-aware policy can decide whether release is allowed

## Step 3 — Validated response

Show:

- `docs/screenshots/accepted-response.png`

Talk track:

- accepted response demonstrates signature validity, schema validity, policy allow decision, and generated Bronze / Audit paths
- this is not a placeholder mock; it reflects validated demo output
- the platform is evaluating before release, not after the fact

## Step 4 — Evidence outputs

Show:

- `docs/screenshots/bronze-output.png`
- `docs/screenshots/audit-output.png`

Talk track:

- Bronze stores the accepted normalized metadata record
- Audit stores evidence of what happened and why
- this separation matters when downstream AI or analytics use must be explainable

## Step 5 — Managed platform direction

Show:

- `docs/ui-secure-ingestion.png`

Talk track:

- the control-plane layer is being developed privately
- this is the direction for tenant operations, usage visibility, policy management, and invoice preview
- the public repository demonstrates architecture and validated baseline behavior
- the operational platform layer is where commercial managed value grows

## Exact validated claims

Use these exact claims:

- signed gateway authentication
- replay protection
- PQC transport hardening track
- mTLS-secured ingress path
- schema and policy validation before downstream release
- Bronze / Audit write separation
- integrated ingest pipeline behavior
- live metering into a private platform layer

## Close with

“This is a validated and pilot-ready secure-ingestion baseline. The public showcase demonstrates the architecture and the validated flow. The managed platform layer — including tenant administration, billing, usage visibility, lifecycle tooling, and enterprise operations — continues privately.”

