# Agentic Pipeline – Two Modes (Modular)

This repo uses a minimal, modular structure optimized for LLM performance:

- Scoping (user‑led capture)
- Review (non‑technical requirements check)

Start here: `Workflow/index.md` (core, always‑loaded rules). Load exactly one mode file and only the needed template at runtime:
- Modes: `Workflow/modes/scoping.md`, `Workflow/modes/review.md`
- Templates: `Workflow/templates/decision-log.md` (append-only one-line decisions), `Workflow/templates/scope-log.md` (append-only one-line scope)

Persisted artifacts live under `inputs/`:
- `inputs/scope-log.md` (append-only one-line scope facts)
- `inputs/decision-log.md` (append-only one-line decisions)
