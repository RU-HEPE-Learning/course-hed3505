# HED3505 GitHub Learning Hub — Migration Map 01

## Purpose

This document records the first migration mapping from the former GitHub Classroom-oriented operating model to the approved HED3505 GitHub Learning Hub architecture.

## Canonical workflow

**Teaching → Student Activity → Evidence Capture → Feedback → Portfolio**

## Component mapping

| Component | Current decision | Target role |
|---|---|---|
| `course-hed3505` | KEEP + ADAPT | Canonical course workspace |
| `assignment-template` | KEEP + ADAPT | Reusable activity/submission template |
| `student-portfolio-template` | KEEP + ADAPT | Student evidence/reflection portfolio |
| `course-hub` | KEEP + ADAPT | Organization learning entry point |
| `kasemch/hed3505-interactive-lab` | KEEP / REVIEW | Static interactive activity prototype |
| GitHub Classroom-specific phases | RETIRE | No longer part of active architecture |
| Classroom roster/provisioning dependency | RETIRE | Replace with controlled repository access |
| Learning Hub navigation | CREATE | Student-facing course journey |
| Evidence/progress index | CREATE | Lightweight learning evidence tracking |
| Teacher review flow | CREATE / ADAPT | Feedback and quality review, separate from official grades |

## Non-interference rule

This migration does **not** modify `kasemch/kasemch.github.io`.

The public academic website remains an independent system and is not the implementation target of this migration.

## Governance

- Evidence-First / No Fabrication
- Static-first where possible
- No mandatory backend
- Mobile-friendly
- Minimum student friction
- Sensitive data excluded from public repositories
- Human authority retained for grading, curriculum mapping, schedules, and roster decisions

## Gate for Phase 02

Phase 02 may proceed when:
- legacy Classroom language is removed from active course instructions;
- the student journey can be expressed without Classroom;
- assignment and portfolio templates can support private-repository use;
- navigation can be implemented without changing the public academic website.
