## Create Output – Phase 1 (Minimal)

Sources: `inputs/input.md` (baseline), `inputs/scope-log.md`, `inputs/decision-log.md`, `inputs/notes.md`
Output: `concepts/<YYYYMMDD-HHMMSS>-Phase1.md`

Sections (exactly, in order; no others). If multiple Parts are detected (see "Parts"), these sections repeat per Part.

## 🎯 **Goal** – What should be achieved?
- One concise sentence. Prefer a decision titled "Goal"/"Objective"; otherwise synthesize from the most central decision(s); if unclear, write "TBD".

## 📌 **Requirements** – Which decisions or must-have criteria are set?
- Include all decisions except those classified as Non-Goals.
- Single-line bullets; deduplicate; order by importance and narrative coherence.
- Include quoted facts that define exact wording (e.g., UI text); preserve wording.
 - Default destination for decisions: include all entries from `inputs/decision-log.md` unless a Non-Goals or Goal rule applies.

## 🚫 **Non-Goals** – What should explicitly not be included?
- Decisions that clearly exclude scope (e.g., contain "not ", "no ", "exclude", "excluded", "out of scope", "won’t", "without").
- When ambiguous, keep in Requirements (do not move to Non-Goals).
- Single-line bullets; deduplicate; order by importance and narrative coherence.

## 📌 **Additions** – What important decisions or items don't fit the other three categories?
- Only items not classifiable as Goal, Requirements, or Non-Goals; use sparingly.
- Single-line bullets; deduplicate; order by importance and narrative coherence.

Source precedence and conflicts:
- Treat `inputs/input.md` as timestamp 0 (earliest facts).
- Later facts in `inputs/scope-log.md` override conflicting facts from `inputs/input.md`.
- Decisions in `inputs/decision-log.md` override both logs; if a fact conflicts with a decision, align with the decision or omit the fact.

Notes inclusion:
- Include a note only if referenced by a log line via [ref:KEY].
- Use the note’s first paragraph verbatim (quoted).
- Classify based on the referencing line; notes never override decisions.

Classification (apply in order):
- Non-Goals: contains any of ["not ", "no ", "exclude", "excluded", "out of scope", "won’t", "without"].
- Goal: title/line includes ["goal", "objective", "aim", "purpose"] or phrasing like “should achieve/enable”.
- Decisions default to Requirements unless Non-Goals or Goal matches.
- Requirements: obligation cues ["must", "shall", "will", "must not", "need to", "required", "require"] or acceptance-like statements.
- Else: Additions.
 - When uncertain, prefer Requirements over Additions.

 

Rules:
- Plain English. No links, file paths, timestamps, or metadata.
- Do not include the Overview or the Review List in this file.
 - Ordering: importance and narrative coherence; tie-break by source precedence (decisions > scope-log > input.md) and recency within source.

Parts (optional):
- Split into multiple Parts only if distinct themes are clearly separable from the inputs.
- Title each Part with a concise 2–4 word theme derived from recurring Topics/titles (no links/paths).
- Render the four sections (Goal, Requirements, Non-Goals, Additions) within each Part.
- Items not clearly attributable to a specific theme remain in a single “General” Part (rendered first).
- Notes are included only when referenced by a log line within the same Part; do not carry notes across Parts.
- Apply existing classification, precedence, and ordering rules within each Part.

