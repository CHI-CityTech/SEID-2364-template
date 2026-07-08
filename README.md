# SEID 2364 Template Repository

<img src="./resources/images/SEID2364%20logo%20ChatGPT.png" alt="SEID 2364 logo" width="160">

Work in progress: this repository is currently being revised into a more complete v2 version of the SEID 2364 course template.

This repository is the reusable template baseline for SEID 2364 (Societal and Ethical Impacts of Data Science).

SEID 2364 is an applied ethics course in data science that examines how responsibility, judgment, power, mediation, and harm emerge across human, institutional, and computational systems. Grounded in the Balanced Blended Space (BBS) framework, the course treats ethical reasoning as a practical activity within complex socio-technical environments rather than as abstract rule application alone. It increasingly incorporates EDOCA, SRDMPA, case-based reasoning, and future-capability analysis to help students evaluate data-driven systems under conditions of ambiguity, complexity, and change.

The course is intentionally multimodal. Students work across discussion, case analysis, writing, mapping, game and simulation structures, AI-mediated interaction, synchronous and asynchronous exchange, and repository-based documentation. These modalities are not only delivery mechanisms; they can themselves become objects of ethical analysis. Across the semester, the course is designed to help students develop both a thoughtful personal ethical framework and a professional ethical framework for responsible practice in data science and hybrid human-machine environments.

This repository captures a maintainable course structure derived from the Spring 2026 delivery and supports future semester adaptation without preserving live-semester operational noise in the root.

## Repository Goal

Use this repository to:

1. Run future offerings of SEID 2364.
2. Preserve stable course architecture (syllabus, assignments, resources, case studies).
3. Maintain a clear separation between reusable template assets and historical assessment artifacts.

## What Is Canonical

1. `SYLLABUS.md` at repository root is the active maintained syllabus for the template.
2. `assignments/`, `case-studies/`, and `resources/` provide the reusable instructional materials.
3. `assessment/` contains redesign analysis and planning artifacts from the first iteration and later redesign passes.

## Historical Source Artifacts

Historical syllabus source files are stored in:

1. `docs/syllabus-sources/`

These are preserved for reconstruction and comparison, not as the primary syllabus to edit.

## Repository Organization

1. `SYLLABUS.md`
2. `README.md`
3. `assignments/`
4. `assignments/archive/`
5. `assignments/upcoming/`
6. `case-studies/`
7. `resources/`
8. `resources/week-03/` through `resources/week-06/`
9. `resources/week-08/` through `resources/week-12/`
10. `resources/lecture notes/`
11. `resources/glossaries/`
12. `assessment/`
13. `docs/syllabus-sources/`
14. `students/`

## Assessment and Redesign Workspace

The redesign workspace is intentionally located in:

1. `assessment/`

Start here:

1. `assessment/README.md`
2. `assessment/COURSE_REDESIGN_FINDINGS.md`
3. `assessment/TEMPLATE_REDESIGN_TASKS.md`

These files track findings, priorities, and redesign execution steps, including syllabus and sequence updates.

## Adoption Workflow for a New Semester

1. Copy or branch from this template baseline.
2. Update `SYLLABUS.md` for the upcoming offering.
3. Select active assignments in `assignments/` and adjust schedule references.
4. Confirm weekly resource bundles in `resources/week-*`.
5. Keep redesign/planning notes in `assessment/` rather than root.
6. Archive superseded materials in `assignments/archive/` or `resources/archive/`.

Weekly resource normalization is still in progress. At present, week folders exist for weeks 03-06 and 08-12; additional consolidation can continue as the lecture/resource cleanup proceeds.

## Notes on AI and Evidence

1. AI collaboration is expected to be transparent and attributable in course artifacts.
2. Evidence-first workflow remains important: readings, source traceability, and reproducible assignment references should be preserved.
3. Methods and terminology from the redesign analysis (including SRDMPA and EDOCA framing) should be integrated through syllabus and assignment revisions, not only in assessment notes.

## Related Repositories

1. AI-Curriculum planning repository:
   https://github.com/CHI-CityTech/AI-Curriculum

## Maintenance Principle

Keep root files minimal and stable.

Put operational analysis, redesign notes, and historical interpretation in `assessment/` and `docs/`, while maintaining template-facing teaching assets in `SYLLABUS.md`, `assignments/`, `case-studies/`, and `resources/`.
