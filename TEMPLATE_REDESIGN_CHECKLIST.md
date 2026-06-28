# SEID 2364 Template Redesign Checklist

## Purpose
This repository is a clone of the frozen SEID-2364 main baseline for conversion into a reusable template.

## Freeze Provenance
- Source repository: CHI-CityTech/SEID-2364
- Freeze tag (local in source repo): freeze-2026-06-28-main-573b8be
- Source baseline commit on main: 573b8be

## Template Conversion Steps
1. Remove or sanitize any semester-specific dates.
2. Replace course-instance identifiers with placeholders.
3. Ensure grading operations and private evaluation logic are excluded.
4. Keep assignment and case-study scaffolding reusable.
5. Add an instructor quick-start for next-semester adoption.
6. Add a changelog entry documenting redesign decisions.

## Suggested Placeholder Conventions
- {{TERM}}
- {{INSTRUCTOR_NAME}}
- {{SECTION}}
- {{OFFICE_HOURS}}
- {{DELIVERY_MODE}}

## Recommended Deliverables
1. A clean README for template users.
2. A template release tag (for example, v1.0.0-template).
3. A migration note pointing to legacy AI-Curriculum location.
4. A short evidence note to support OAA innovation reporting.
