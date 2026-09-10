# backend

APIs, services, and deterministic logic. Suggested layout:

- backend/services/      - deterministic matcher, unit converters, ontology mappers
- backend/integrations/  - clients for Lyzr Safe AI, Lyzr Agent API, AIMS event streamer
- backend/api/           - FastAPI/Flask endpoints for screening, audit, and HITL webhooks
- backend/tests/         - pytest unit and integration tests, synthetic EHR dataset

Core responsibilities

- Enforce deterministic comparisons for numeric thresholds and time windows
- Never log raw PHI — call Lyzr Safe AI to redact and store redaction maps in a secure vault
- Emit signed, append-only audit events to AIMS for every decision and human override
