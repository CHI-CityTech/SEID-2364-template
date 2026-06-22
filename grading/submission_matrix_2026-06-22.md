# SEID-2364 Submission Matrix (Branch-Based)

Date: 2026-06-22
Branch: grading-private-2026-06-22 (local only, not pushed)

Scope:
- Presence/absence of assignment artifacts by student branch.
- Detection by assignment number in filenames across two common locations:
  - assignments/
  - students/*/assignments/
- Completeness pass only (not quality scoring).
- Assignments may have been optional/over-assigned; treat missing items as informational until policy is finalized.

Legend: X = assignment-number match found, . = no match found

| Student Branch | A01 | A02 | A03 | A04 | A05 | A06 | A07 | A08 | A09 | A10 | A11 | A12 | A13 | A14 | Total |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Atien-Ferra | X | X | X | X | X | X | X | X | X | X | X | X | X | X | 14 |
| Aydogdyyev-Azim | X | X | X | . | . | . | . | . | . | . | . | . | . | . | 3 |
| Mizetskyi/Pavlo | X | X | X | X | X | X | . | . | . | . | . | . | . | . | 6 |
| davidstudent | X | X | X | . | . | . | . | . | . | . | . | . | . | . | 3 |
| marin | X | X | X | X | X | X | X | X | X | X | . | . | X | . | 11 |
| samuel | X | X | X | X | X | X | X | X | X | X | X | X | . | . | 12 |

## Important Validation Notes
- Samuel has submissions on both origin/main (students/) and origin/samuel (assignments/).
- Marin submissions were not on origin/main; they are present on origin/marin under students/marin/assignments/.
- Filename normalization varies; matching is number-based to tolerate naming differences.

## Privacy Recommendation
- Safe now: keep grading artifacts on local branch grading-private-2026-06-22 and do not push.
- If cloud backup is needed, push to a private repo/fork not accessible to students.
