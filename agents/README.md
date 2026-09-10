# agents

This directory holds Lyzr Agent API artifacts and orchestration configs. Put agent definitions, prompt templates, and orchestration workflows here. Example contents:

- agents/protocol-extractor/  - extract inclusion/exclusion criteria from protocol PDFs into structured JSON
- agents/phi-scrubber/       - wrappers that call Lyzr Safe AI for PHI redaction and tokenization
- agents/screening-orchestrator/ - workflows that coordinate extraction, scrubbing, deterministic matcher, and audit logging
- agents/README.md           - this file

Agent config tips

- Keep prompts limited to extraction/normalization; do not use LLMs for final eligibility decisions.
- Record agent versions and image SHAs in AIMS events for reproducibility.
