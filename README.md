# COMP3423 Group Project — Mobile Banking App Redesign

Group project for COMP3423 Human Computer Interaction (HKPolyU, Sem 1, due 2026-11-15). Team of 5 redesigning a mobile banking app based on HCI principles: usability analysis → redesign → Figma prototype (5 features) → Maze user testing → report + video.

**Start here:** [`2026-09-16-comp3423-project-plan.md`](2026-09-16-comp3423-project-plan.md) — full 8-week plan, Gantt chart, role assignments, and a submission QA checklist mapped to the grading rubric. The spec itself is [`COMP3423-Group-Project-Description-2026S1.pdf`](COMP3423-Group-Project-Description-2026S1.pdf).

## Repo layout

```
report/                  Report sections as separate files (merge into one Word/PDF doc before submission)
  00-cover-page.md          Workload declaration table (Appendix I format)
  01-introduction.md        ~1 page
  02-related-work.md        2-4 pages, 10-20 refs
  03-overall-design.md      3-5 pages
  04-feature-details.md     4-6 pages, one subsection per feature (x5)
  05-testing-results.md     3-5 pages
  06-conclusion.md          ~1 page
  references.md             Master reference list (keep in sync with in-text citations)

research/                 Analysis-stage working documents (Accessibility & Evaluation Lead owns most of this)
  heuristic-evaluation.md    Nielsen's 10 heuristics applied to the real app
  accessibility-audit.md     WCAG-basics checklist (contrast, touch targets, text scaling, screen reader)
  candidate-usability-problems.md   Working list of 8-10 problems, narrowed to 5 features in Week 3

testing/                  Testing-stage working documents (User Researcher owns most of this)
  maze-test-plan.md          Tasks, metrics, procedure
  recruitment-script.md      Outreach message + screening criteria
  results-log.md             Where raw Maze results get summarized (raw export goes in report appendix)

prototype/                Real, working HTML/CSS draft of the redesign (14 screens, 5 features)
  index.html                 Screen picker/preview
  README.md                  How to import into Figma via the html.to.design plugin
  (see report/01-introduction.md §1.4 for what each feature is and why)

assets/                   Evidence
  screenshots/existing-app/  Real screenshots of the current app ONLY — see README inside
  screenshots/redesign/      Before/after captures for the report
  figma/                     Figma project link + notes

project-management/       Process evidence (protects the workload declaration)
  task-log.csv               Who did what, when, link to the deliverable
  meeting-notes/              One file per sync

presentation/
  ppt-outline.md             Slide-by-slide outline, screenshot-driven
  video-script.md            Timed script matching the spec's suggested structure
```

## Ground rules (from the spec's marker notes — read before contributing)

- **Screenshots of the existing app must be real**, not AI-generated mockups — markers check this explicitly.
- **Maze data must be real** — a generic or implausible-looking results table gets queried.
- **Every declared role needs a visible, traceable contribution** — log your work in `project-management/task-log.csv` as you go, not retroactively.
- **Every design decision needs a named HCI principle** and, where relevant, a cited source in `report/references.md`.
- Keep the Figma project set to public **view/comment** access at all times — verify in an incognito window before submitting.
