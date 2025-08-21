# Decision Log – One-Line Append Format

Target file (append-only): `inputs/decision-log.md`

## Rules
- Always append; never rewrite or delete.
- One decision per line.
- Business-level outcome only; no technical details.

## Exact line format
```
// Decision – YYYY-MM-DD HH:MM – <Short Title> : <Very short description>
```

## Examples
```
// Decision – 2025-08-20 14:32 – Update Frequency : Status must refresh every 60 minutes
// Decision – 2025-08-21 09:10 – Access : Only customers can view status, not partners
// Decision – 2025-08-22 11:05 – Notifications : SMS updates are explicitly excluded
```
