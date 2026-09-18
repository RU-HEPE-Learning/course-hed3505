# Course Status

Status: **PILOT**

Phase: **HED3505-GITHUB-LEARNING-HUB-05 — INTEGRATION QA & PILOT READINESS GATE**

Gate result: **PASS WITH CONDITIONS**

## Canonical operating model

**Teaching → Student Activity → Evidence Capture → Feedback → Portfolio**

GitHub Classroom is not a dependency of the approved architecture.

## Integration status

- Course Hub navigation: READY / CI confirmation pending
- HED3505 course workspace: PASS
- Assignment template: READY / revised CI confirmation pending
- Student portfolio template: READY / first portfolio CI confirmation pending
- Interactive lab: contextual / optional integration only
- `kasemch.github.io`: NO CHANGE

## Pilot boundary

- student work is private by default;
- official scores and grades remain outside GitHub unless later explicitly authorized;
- CLO/PLO mappings, deadlines, assessment weights and outcomes require authoritative evidence;
- public repositories must not contain sensitive student, health, identity, grade or confidential school data;
- automated validation is structural only;
- final academic judgment remains human/instructor authority.

## Current conditions before baseline merge

1. Confirm successful revised CI for `assignment-template`.
2. Confirm successful revised CI for `course-hub`.
3. Confirm successful first CI for `student-portfolio-template`.
4. Preserve all PRs as draft until CI closure.
5. Merge in controlled dependency order only after the above conditions pass.

## Recommended merge order

1. assignment-template
2. student-portfolio-template
3. course-hed3505
4. course-hub

## QA Record

See `INTEGRATION-QA-05.md`.

## Next transition

**HED3505-GITHUB-LEARNING-HUB-06 — CI Closure, Merge Readiness Confirmation & Controlled Baseline Promotion**
