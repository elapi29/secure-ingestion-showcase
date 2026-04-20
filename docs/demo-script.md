# Demo Script

## Goal

Communicate a validated secure-ingestion baseline before downstream AI, analytics, or clinical workflow use.

## Open with

“This showcase demonstrates a secure ingress layer for sensitive clinical metadata. The goal is to verify, validate, record, and control release before downstream AI or analytics systems receive anything.”

## Step 1 — Open the README hero

Show the README opening section.

Talk track:

- this is a public showcase, not the private managed platform
- the claim is a validated secure-ingestion baseline
- the problem is controlled handoff before downstream AI or analytics use

## Step 2 — Bronze and audit model

Show:

- `docs/bronze-flow.png`

Talk track:

- accepted metadata becomes a Bronze record
- evidence and release trace are persisted separately in Audit
- this creates a cleaner boundary between operational ingest and downstream usage evidence
- tenant-aware policy can decide whether release is allowed before downstream use

## Step 3 — Accepted response

Show:

- `docs/screenshots/accepted-response.png`

Talk track:

- the accepted response demonstrates signature validity, schema validity, policy allow decision, and generated Bronze / Audit paths
- this is validated demo output, not a placeholder mock
- the platform evaluates before release, not after the fact

## Step 4 — Bronze evidence

Show:

- `docs/screenshots/bronze-output.png`

Talk track:

- Bronze stores the accepted normalized metadata record
- this is the controlled data handoff artifact
- the point is not just acceptance, but structured accepted release

## Step 5 — Audit evidence

Show:

- `docs/screenshots/audit-output.png`

Talk track:

- Audit stores traceable evidence of what happened and why
- this matters when downstream AI or analytics use must be explainable
- Bronze and Audit are intentionally separated

## Step 6 — Managed platform direction

Show:

- `docs/ui-secure-ingestion.png`

Talk track:

- the control-plane layer is being developed privately
- this image shows the intended direction for tenant operations, usage visibility, policy management, and invoice preview
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

