# SEID 2364 Template Redesign Task Tracker

Date: 2026-06-28
Branch: template-redesign-2026

## Purpose

This file tracks the concrete work needed to finish the template redesign. It should stay actionable and easy to update as tasks are completed.

## Priority Order

### 1. Remove course-instance specificity from top-level docs

- [ ] Replace Spring 2026 wording in the main README with template-neutral language.
- [ ] Remove or relocate live Moodle and instructor-specific details from the README.
- [ ] Sanitize the syllabus file so it can serve as a reusable template reference instead of a semester snapshot.
- [ ] Decide whether placeholder tokens should stay as literal `{{...}}` markers or be replaced through a generation workflow.
- [ ] If replacement is required, define the template/cloning process that fills in semester-specific values.

### 2. Separate template guidance from semester workflow

- [ ] Move submission-path instructions out of the template README if they are only relevant to a live class run.
- [ ] Add a short instructor quick-start for adopting the template next semester.
- [ ] Add a migration note that explains where legacy AI-Curriculum planning materials now live.

### 3. Finish wiki governance and cleanup

- [ ] Create a curated wiki index that lists only active wiki pages.
- [ ] Mark experimental or superseded wiki pages with an archived status.
- [ ] Verify that all assignment and resource links resolve to the template wiki targets.
- [ ] Add lecture-note slide decks and supporting outlines to the evidence map for all weeks.
- [ ] Track the lecture-note PDFs as part of the documented delivery record rather than leaving them implicit.

### 4. Build the Spring 2026 coverage evidence base

- [ ] Treat the lecture-note PDFs in `resources/lecture notes/` as the primary record of what was actually delivered.
- [ ] Treat the assignment files in `assignments/` as the primary record of what students were actually asked to do.
- [ ] Include any newly copied lecture-note PDFs as tracked source evidence.
- [ ] Build a week-by-week coverage matrix that compares the syllabus, lecture PDFs, assignments, and resources.
- [ ] Treat the current weekly resource folders as provisional; do not reorganize them until the revised syllabus is finalized.
- [ ] After the revised syllabus is finalized, build or normalize one resource bundle per week as needed.

### 5. Package the template for reuse

- [ ] Add a changelog entry documenting the redesign decisions.
- [ ] Add a short evidence note for OAA innovation reporting.
- [ ] Create or tag a template release version.

## Suggested Status Labels

- `not started`
- `in progress`
- `blocked`
- `done`

## Notes

- Keep this file focused on implementation tasks rather than design principles.
- When a task is complete, record the relevant file or commit in a short note under the finished item if needed.