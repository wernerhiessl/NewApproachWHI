# Workflow – Core Index (Always Loaded)

This repository uses a two‑mode workflow with minimal files:
- Scoping (user‑led capture)
- Review (non‑technical requirements check)

Active folders:
- `Workflow/` – this index, per‑mode guides, and lightweight templates
- `inputs/` – timestamped scope notes and `decision-log.md`

## Startup and switching
- If no mode is specified at start, default to Review Mode without asking.
- Switch by user message: "Scoper" or "Reviewer". On switch, quickly catch up from `inputs/` and continue without re‑asking.

## File I/O and determinism
- Persisted outputs are in English.
- Do not modify existing inputs unless appending decisions.
- Follow repository file‑operations policy (no shell I/O).
- Be deterministic: concise phrasing, stable headings, fixed behaviors.

## Loading policy (keep prompt small)
- Always load: `Workflow/index.md` (this file)
- Load exactly one mode:
  - Scoping: `Workflow/modes/scoping.md`
  - Review: `Workflow/modes/review.md`
- Templates loaded on demand (identical approach for both logs):
  - Decision log format: `Workflow/templates/decision-log.md`
  - Scope log format: `Workflow/templates/scope-log.md`

## Structure summary
- `Workflow/modes/scoping.md` – Scoping behavior
- `Workflow/modes/review.md` – Review behavior
- `Workflow/templates/` – minimal, task‑specific snippets
