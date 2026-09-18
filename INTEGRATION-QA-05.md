# HED3505 GitHub Learning Hub — Integration QA & Pilot Readiness Gate

Date: 18 September 2026

## Gate Result

**PASS WITH CONDITIONS**

The Learning Hub architecture is coherent across the four active repositories and is ready for controlled merge preparation. Final baseline merge should wait until the remaining CI confirmations complete.

## Scope

Repositories reviewed:
- `RU-HEPE-Learning/course-hub`
- `RU-HEPE-Learning/course-hed3505`
- `RU-HEPE-Learning/assignment-template`
- `RU-HEPE-Learning/student-portfolio-template`

Read-only contextual review:
- `kasemch/hed3505-interactive-lab`

Protected / not modified:
- `kasemch/kasemch.github.io`

## QA Results

| QA Area | Result | Notes |
|---|---|---|
| Cross-repository architecture | PASS | Hub → Course → Assignment / Portfolio roles are coherent |
| Naming consistency | PASS | HED3505 naming and five-week labels aligned in active migration branches |
| Five-week course alignment | PASS | Week 01–05 map consistently to Assignment 01–05 |
| Assignment-template compatibility | PASS | Workflow states, evidence, reflection and feedback templates added |
| Portfolio traceability | PASS | Task → Evidence → Reflection → Feedback → Final Artifact chain defined |
| Privacy boundary | PASS | Private-by-default and no public sensitive/grade records consistently stated |
| Mobile usability baseline | PASS | GitHub web workflow defined without command line requirement |
| GitHub Classroom dependency removal | PASS | No active dependency found in reviewed target branch materials |
| GitHub Actions compatibility | PASS WITH CONDITION | Course workflows passed; assignment/hub CI rerun pending; portfolio workflow newly added |
| Public/private separation | PASS | Public course material separated from private student work |
| Student submission workflow | PASS | Tool-independent submission lifecycle defined |
| Instructor feedback workflow | PASS | Human academic authority preserved |
| Evidence traceability | PASS | Required relationship defined across template and portfolio |
| Draft PR consistency | PASS | All four migration PRs remain draft and mergeable at last check |
| Merge readiness | PASS WITH CONDITION | Complete CI confirmation required before merge |

## Defect Register

### D-01 — Assignment CI did not validate newly added Learning Hub files
Status: **REMEDIATED**

Remediation:
- updated assignment workflow to validate:
  - `STATUS.md`
  - `EVIDENCE-REQUIREMENTS.md`
  - `REFLECTION.md`
  - `FEEDBACK.md`

### D-02 — Portfolio template had no Learning Hub structure CI
Status: **REMEDIATED / CI CONFIRMATION PENDING**

Remediation:
- added `.github/workflows/validate-portfolio.yml`

### D-03 — Course Hub CI did not validate the new HED3505 mobile navigation artifact
Status: **REMEDIATED**

Remediation:
- updated hub structure workflow to require:
  - `docs/student-workflow.md`
  - `docs/hed3505-mobile-navigation.md`

### D-04 — Legacy architecture document names include “classroom”
Status: **NON-BLOCKING / DOCUMENTATION DEBT**

Rationale:
- filename alone does not create a runtime dependency;
- active student/instructor workflows no longer require GitHub Classroom;
- may be renamed in a later documentation-cleanup phase to reduce conceptual ambiguity.

## CI Evidence

Confirmed:
- `course-hed3505` — Validate HED3505 Structure: **SUCCESS**
- `course-hed3505` — Validate learning structure: **SUCCESS**

Pending at this gate:
- `assignment-template` updated workflow run
- `course-hub` updated workflow run
- `student-portfolio-template` first run of newly added portfolio validation workflow

## Merge Sequence

Recommended order after CI is green:

1. `assignment-template` PR #1
2. `student-portfolio-template` PR #1
3. `course-hed3505` PR #2
4. `course-hub` PR #2

Rationale:
templates first → course implementation second → navigation layer last.

## Rollback Plan

If a merged repository causes an issue:
1. identify the merge commit;
2. revert only that repository's merge commit;
3. retain the other repositories if unaffected;
4. reopen remediation on a new branch;
5. do not modify `kasemch.github.io`.

## Pilot Readiness Checklist

- [x] Five-week course path verified
- [x] Five assignments present
- [x] Evidence requirements present
- [x] Reflection workflow present
- [x] Feedback workflow present
- [x] Portfolio traceability defined
- [x] Private-by-default rule defined
- [x] Official grades separated from GitHub
- [x] Mobile/browser-only baseline documented
- [x] No command line required
- [x] No GitHub Classroom dependency required
- [x] Human academic authority retained
- [x] Course structural CI passed
- [ ] Assignment revised CI completed successfully
- [ ] Hub revised CI completed successfully
- [ ] Portfolio validation CI completed successfully
- [ ] Draft PRs converted to final merge-ready state
- [ ] Merge sequence executed

## Next Gate

**HED3505-GITHUB-LEARNING-HUB-06 — CI Closure, Merge Readiness Confirmation & Controlled Baseline Promotion**
