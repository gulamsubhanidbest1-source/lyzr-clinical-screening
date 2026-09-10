# frontend

Coordinator UI and client applications. Suggested layout:

- frontend/app/          - React/Next.js or CRA app for coordinators
- frontend/components/   - reusable UI components (EvidenceHighlight, AuditTimeline, PatientList)
- frontend/api/          - API client wrappers for backend endpoints (screening, audit, HITL)

UX guidance

- Show per-criterion evidence with linked source excerpts
- Provide HITL actions: Accept, Reject, Flag for follow-up, plus an electronic signature flow
- Filter by confidence, protocol, and date; surface AIMS events for audit
