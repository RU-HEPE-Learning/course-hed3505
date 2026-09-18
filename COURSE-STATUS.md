# Course Status

Status: **PILOT**

Phase: **HED3505-GITHUB-LEARNING-HUB-01 — CURRENT REPOSITORY RECONSTRUCTION & MIGRATION MAPPING**

Migration decision: **APPROVED**

## Operating model

GitHub Classroom is no longer a dependency of this course architecture.

The approved course workflow is:

**Teaching → Student Activity → Evidence Capture → Feedback → Portfolio**

Primary components:
- `RU-HEPE-Learning/course-hed3505` — canonical controlled course workspace
- `RU-HEPE-Learning/assignment-template` — reusable assignment structure
- `RU-HEPE-Learning/student-portfolio-template` — student evidence and reflection structure
- `RU-HEPE-Learning/course-hub` — organization-level learning entry point
- `kasemch/hed3505-interactive-lab` — interactive/static learning activity prototype where useful

## Locked design principles
- Static-first
- Mobile-friendly
- Low-cost
- Maintainable
- No mandatory backend
- Evidence-First / No Fabrication
- Human academic judgment remains authoritative
- No sensitive student, health, grade, or identity data in public repositories

## Repository reconstruction decision

### KEEP
- course materials, weekly packages, assignments, evidence, rubrics, portfolio guidance
- privacy and governance controls
- reusable assignment and portfolio templates
- structural validation through GitHub Actions where useful

### ADAPT
- any workflow, status label, documentation, or onboarding instruction that assumes GitHub Classroom
- submission instructions so they work through repository / pull-request / portfolio workflows
- pilot provisioning language so it is tool-independent

### RETIRE
- GitHub Classroom-specific phase names
- Classroom roster/provisioning dependency
- Classroom-specific activation gates

### CREATE
- Learning Hub navigation and student-facing start page
- migration-safe assignment launch instructions
- lightweight progress/evidence index
- teacher review workflow that remains separate from official grading records

## Current pilot boundary
- Student work: private by default
- Official grades: outside GitHub unless explicitly authorized later
- CLO/PLO mappings: publish only from authoritative curriculum evidence
- Deadlines: publish only from verified teaching schedule
- Real student identities: never stored in public control records

## Next transition
**HED3505-GITHUB-LEARNING-HUB-02 — Student Journey, Navigation & Submission Workflow Refactor**
