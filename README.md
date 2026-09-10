# lyzr-clinical-screening

Governed Clinical Trial Patient Screening & Regulatory Audit Agent — MVP scaffold integrating Lyzr Agent API, Lyzr Safe AI, and AIMS-style audit logging.

This repository contains a modular scaffold for the MVP: ingestion, protocol criteria extraction, PHI redaction, deterministic screening, and audit dossier generation, plus a coordinator UI.

Repository structure

- agents/ — Lyzr agent configs, orchestration, and agent code
- frontend/ — Coordinator UI and client apps that call agents
- backend/ — APIs, deterministic services, and integrations (Safe AI, AIMS)
- Dockerfile (optional) — container build for backend service
- docker-compose.yml (optional) — local multi-service run
- .env.example — environment variables template (no secrets)
- README.md — this file

Next steps

1. Implement deterministic matcher and unit tests in backend/
2. Add agent definitions and Lyzr orchestration configs in agents/
3. Build a simple React UI in frontend/ and wire to backend APIs
4. Add CI, secrets (KMS/HSM), and branch protection before production

See project board and issues for detailed milestones (coming next).
