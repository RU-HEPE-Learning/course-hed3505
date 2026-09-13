# Deferred Roster Reconciliation Procedure

Use this procedure when the official end-of-term examination/course roster becomes available.

## Inputs

- Controlled private pilot identity mapping
- Official roster evidence
- Current anonymous pilot state

## Reconciliation outcomes

- `MATCH_CONFIRMED`
- `NOT_FOUND`
- `AMBIGUOUS`
- `WITHDRAWN_NOT_ELIGIBLE`

## Rules

1. Reconcile in a controlled/private context.
2. Do not publish names or student IDs to public repositories.
3. Change official enrollment state to `VERIFIED` only when authoritative evidence supports the match.
4. If `NOT_FOUND` or `AMBIGUOUS`, preserve learning evidence but keep it separate from official grading decisions.
5. All exceptions remain subject to instructor/course authority review.

## Evidence preservation

Pilot learning evidence is instructional evidence. It must not be silently rewritten or deleted solely to make later roster reconciliation appear cleaner.
