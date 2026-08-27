# Hardware Project Template

Starter template for **UTDesign EPICS hardware teams**. Generate a repo from this
template at the start of the semester, then keep three living documents up to date as
your project evolves:

| Document                             | Path                        | Purpose                                                                                         |
| ------------------------------------ | --------------------------- | ----------------------------------------------------------------------------------------------- |
| **Weekly Progress Report (WPR)**     | `wpr/<semester>/w<n>.md`    | One file per week logging per-member progress, blockers, and project status.                    |
| **Requirements**                     | `requirements.md`           | Single source of truth for what the build must do, tracked in a requirement matrix with status. |
| **Architecture Decision Record (ADR)** | `docs/adr/NNN_<slug>.md`  | One file per significant design decision — the options, the choice made, and the trade-offs.    |

## Getting started

1. Click **Use this template → Create a new repository**, or:
   ```
   gh repo create UTDallasEPICS/<your-team-repo> --template UTDallasEPICS/hardware-template --private
   ```
2. Update `requirements.md` with your project's actual requirements (delete the example rows).
3. Rename the WPR folder to your current semester and start logging weekly.
4. Copy `docs/adr/001_template.md` to a new numbered file whenever you make a real design decision.

## Conventions

### Weekly Progress Reports

- One folder per semester, named `s<n>_<season><yy>` — e.g. `s1_fall26` for the first
  semester of a project starting Fall 2026, `s2_spring27` for its second semester.
- One file per week inside that folder, named `w<n>.md` (`w1.md`, `w2.md`, …).
- Fill out the report before your weekly lab/standup so mentors and partners can follow along.

### Requirements

- Every requirement gets a stable ID (`REQ-F-01`, `REQ-NF-01`, …) that never changes or is reused.
- Update the **Status** column as work progresses; log scope changes in the **Change Log**.
- Map each requirement to the GitHub issue, design doc, drawing, or test that satisfies it.

### Architecture Decision Records

- Number ADRs sequentially: `001`, `002`, … Never renumber or delete an ADR — supersede it instead.
- Write one when a decision is hard to reverse or the reasoning would otherwise be lost
  (component/material selection, mechanism choice, power architecture, safety approach, etc.).
- Keep `001_template.md` as the blank template; copy it to start a new record.
