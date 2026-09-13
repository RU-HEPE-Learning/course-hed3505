# RU-HEPE-CLASSROOM-03B.2R — Roster-Deferred Pilot Identity Model

Status: **APPROVED OPERATING MODEL**

Institutional context: Ramkhamhaeng University teaching operations do not provide the official student roster to the instructor until the final-examination period. Therefore, early official-roster availability is not a prerequisite for a controlled learning pilot.

## Operating sequence

Student participation claim → instructor confirms actual HED3505 learning participation → GitHub identity verified → private pilot access may be prepared → learning evidence generated → official roster becomes available later → deferred roster reconciliation → official enrollment status confirmed or handled as an exception.

## Status separation

Each pilot participant must keep three separate states:

- Participation Status
- GitHub Identity Status
- Official Enrollment Status

Official enrollment must remain `DEFERRED_ROSTER_VERIFICATION` until authoritative end-of-term roster evidence is available.

## Pilot eligibility

A participant may proceed toward pilot access when:

1. They actually participate in HED3505 learning activities.
2. Participation in the pilot is voluntary.
3. The instructor confirms participation.
4. The GitHub username is verified directly.
5. The participant acknowledges the privacy and AI-use rules.

## Privacy boundary

Real names, student IDs, personal contact details, health data, grades, and private identity mappings must not be committed to this public repository. Public-safe records may use only anonymous internal pilot IDs and non-identifying workflow states.

## Grading safeguard

GitHub remains outside the official final-grade system during this pilot. Official grading and final enrollment reconciliation remain human-authority functions.

## Deferred reconciliation

When the official examination roster becomes available, run a controlled reconciliation for each pilot identity with outcomes such as `MATCH_CONFIRMED`, `NOT_FOUND`, `AMBIGUOUS`, or `WITHDRAWN_NOT_ELIGIBLE`. Learning evidence must not be retroactively destroyed solely because official enrollment was not confirmed.

## Release rule

The absence of an early official roster is **not a blocker**. Provisioning remains blocked only until instructor-confirmed participation, verified GitHub identity, and privacy acknowledgement are available.
