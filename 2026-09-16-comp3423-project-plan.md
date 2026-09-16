# COMP3423 Group Project Plan — Redesigning an Everyday Application

> **Spec:** `COMP3423-Group-Project-Description-2026S1.pdf` (this directory)
> **Goal:** Deliver a report (≤20 pages) + Figma prototype (5 clickable features) + Maze study (≥5 real participants) + ≤10-min video, maximizing the checkable-evidence rubric (100% + 5% accessibility bonus).
> **Due:** 2026-11-15 (Sun) 23:59. **Today:** 2026-09-16. Week 1 (kick-off) starts 2026-09-22 — you have ~1 week of pre-work runway before the official clock starts.

## Global Constraints (verbatim from spec — every week's tasks inherit these)

- Group of 5, each member **exactly one primary role** (Project Lead & UX Strategist / User Researcher / Interaction Designer / Visual & UI Designer / Accessibility & Evaluation Lead). Supporting other roles is allowed but the *primary* role and its report ownership is fixed.
- 5 major features prototyped in Figma (N = team size = 5), clickable, with navigation, states, and edge cases.
- ≥5 real participants tested via Maze; raw export + dashboard screenshot required in appendix.
- Report: **≤20 pages** excluding references/appendices. References: **10–20**, all cited in body.
- Video: **≤10 min**, must show the Figma prototype live on screen.
- Figma link must be **publicly accessible (view/comment)** — marks deducted if markers can't open it.
- "Before" screenshots must be from the **real existing app** — AI-generated mockups are explicitly disallowed and checked by markers.
- Iteration evidence required: the prototype must **visibly change** after Maze testing (dated v1 vs v2, Figma version history acceptable).
- One zip (report + PPT) submitted **once** to Canvas by the group leader; video uploaded **separately**, not in the zip.
- Mid-project checkpoint (Week 4, 13–19 Oct) is **mandatory but ungraded** — a gate, not a rubric item, but missing it is a process failure.

---

## Part 1 — Pre-Week-1 Setup (do this before 22 Sep)

- [ ] **Form the group of 5** and confirm everyone is committed to the semester-long workload.
- [ ] **Set up shared infrastructure** (do this once, first, so no week is lost to tooling):
  - Shared Figma team project (Team plan or Education plan — confirm seat access for all 5 before Week 1; Figma education verification can take days).
  - Maze account (confirm free-tier participant/test limits are sufficient for ≥5 participants × 5 tasks; check before committing to it in Week 5).
  - Shared cloud doc (Google Docs) for collaborative report drafting → exported to Word/PDF at the end. Decide this now — mixing local Word copies late causes merge conflicts.
  - A shared reference tracker (Zotero/Mendeley or a shared spreadsheet) so citations accumulate from Week 1, not Week 7.
  - A lightweight task log (spreadsheet: date, name, task, deliverable link) — this becomes your evidence for the workload declaration table and protects against a "no traceable contribution" flag (see Appendix II marker notes).
- [ ] **Decide the accessibility bonus up front** (recommend: yes). It's worth +5% (capped at 100%) for work that's cheap if planned from Week 1 (fold into the Week 2 heuristic audit, Week 3 design, Week 6 test tasks) but expensive if retrofitted in Week 7. This is a one-time decision that changes scope for 3 different roles — don't leave it implicit.

---

## Part 2 — App Selection (finish by end of Week 1)

The rubric explicitly grades **"scope realistic for 5 students in 8 weeks" (2 marks)** — the biggest risk here is picking something too ambitious (non-screen modality, deep backend complexity, or a domain no one can recruit real test users for).

**Recommendation: pick a mobile-app or desktop-GUI redesign (screen-based) unless a team member already has strong voice/AR/gesture design experience.** Non-screen modalities add a translation-layer requirement (spec: *"the report must explicitly explain how the physical/gestural/voice layer maps onto the prototype"*) — extra writing and design work for no extra rubric weight.

Shortlist (ranked by 8-week feasibility + ease of recruiting 5 real test participants who already use the app):

| Candidate | Why it's a good fit | Feasibility risk |
|---|---|---|
| **Food delivery app** (e.g., a real app your team already uses) | Rich, well-documented HCI pain points (cart/checkout flow, address management, order tracking, promo/coupon UX); every teammate is a plausible test participant + can recruit peers easily | Low — very familiar domain |
| **Mobile banking app** | Strong HCI + trust/security literature to cite for Related Work; accessibility angle is natural (forms, contrast, error recovery) | Medium — sensitive domain, be careful with real screenshots (redact account numbers) |
| **Public transit app** | Wayfinding/real-time info is a classic HCI case study with abundant literature; strong accessibility story (visually impaired wayfinding) | Medium — good if your city's app has a large, well-known local app to critique |

Whichever is chosen: confirm **(a)** the app has enough recognizable usability problems to fill 5 distinct features, **(b)** at least the Accessibility & Evaluation Lead can install/screenshot it now, and **(c)** the team can realistically recruit ≥5 real people who'd use it (not just classmates pretending).

- [ ] Pick the app + write a 3–4 sentence justification (feeds directly into Introduction, 2 rubric marks: "Justification of app choice and why the existing interface fails").
- [ ] Define the target user group (feeds User Researcher's persona/journey work).
- [ ] Draft a candidate list of 8–10 usability problems (over-scope slightly; you'll cut to 5 features in Week 3).

---

## Part 3 — Role Assignments & Report Ownership

Each role owns one report section outright but every design decision anywhere in the report must be tied to a **named HCI principle** (rubric requirement, not optional prose) — this is a cross-cutting QA responsibility for the Project Lead, not just a Feature Details requirement.

| Role | Owns (report) | Core deliverables |
|---|---|---|
| **Project Lead & UX Strategist** | Introduction, Conclusion | Timeline/coordination; enforces HCI-principle citations throughout; final QA pass; owns the workload declaration table |
| **User Researcher** | Testing Method, Results & Discussion | Target user group, personas, user journey; Maze test design (tasks, metrics, recruitment plan); recruitment execution |
| **Interaction Designer** | Application walkthrough (part of Overall Design) | Information architecture, wireframes, Figma prototype structure (navigation, states) |
| **Visual & UI Designer** | — (contributes across Overall Design + Feature Details) | Visual language/style guide, high-fidelity screens, owns the PPT |
| **Accessibility & Evaluation Lead** | Accessibility considerations (Overall Design) + Accessibility Bonus items | Heuristic evaluation of existing app, accessibility audit, accessibility accommodations in redesign, accessibility-aware Maze task/participant |

- [ ] Assign names to roles; fill the Appendix I cover-page table format now (Name, SID, Role, Key tasks) even in draft form — it's the artifact markers use to check "each declared role should have a visible, distinct contribution."

---

## Part 4 — Week-by-Week Plan

Each week lists concrete, checkable tasks per role. Deviations from the spec's suggested timeline are called out with **why**.

### Week 1 (22–28 Sep) — Kick-off
- [ ] All: finalize app choice, roles, target user group (Part 2 above, if not already done pre-Week-1).
- [ ] Accessibility Lead: install/access the real app now; start a running screenshot log (dated filenames) — this is your evidence trail against the "before screenshots must be real, not AI-generated" check.
- [ ] Project Lead: set up the task log and a shared timeline doc; schedule weekly 20-min sync.
- [ ] User Researcher: start drafting recruitment criteria (who counts as a "real participant" for this app).
- [ ] **All: start logging Related Work references as you read them** (deviation from suggested timeline, which puts Related Work reading in Week 2 — starting a week early avoids the Week 7 crunch where report writing, iteration, and PPT drafting collide).

### Week 2 (29 Sep–5 Oct) — Usability Analysis
- [ ] Accessibility Lead: complete heuristic evaluation of existing app (Nielsen's heuristics or equivalent) + accessibility audit (contrast, touch target size, text scaling, screen-reader compatibility) — write findings directly against annotated screenshots, not just a list.
- [ ] All: from the 8–10 candidate problems, each teammate drafts a one-paragraph "why this is poorly designed" note citing a specific HCI principle — this is the raw material for Feature Details later, don't lose it.
- [ ] Continue Related Work reading (target: 5–8 refs logged by end of week).

### Week 3 (6–12 Oct) — Journey, IA, Wireframes, Feature Selection
- [ ] User Researcher: build the illustrated user journey (stages, touchpoints, pain points) + 1–2 personas.
- [ ] Interaction Designer: information architecture + low-fidelity wireframes.
- [ ] **All: finalize the exact list of 5 features** — pick the ones with (a) clearest existing-app evidence, (b) clean mapping to a named HCI principle, (c) testable as a discrete Maze task. Write one sentence per feature stating the HCI principle now — this becomes the Feature Details section skeleton.
- [ ] Project Lead: draft the Introduction section (problem statement, target user group, scope) — it only depends on Weeks 1–3 output, no reason to wait.

### Week 4 (13–19 Oct) — Mandatory Checkpoint + Hi-Fi Start
- [ ] **Submit the 1–2 page progress snapshot** (app choice, roles, user journey draft, wireframes, feature list) — ungraded gate but treat the deadline as hard.
- [ ] Visual & UI Designer: finalize style guide (colors, type, components) before hi-fi work starts, so all 5 features stay visually consistent (rubric: "interface coherent and consistent as a whole").
- [ ] Interaction Designer + Visual Designer: **start hi-fi Figma on all 5 features in parallel** (not just features 1–3 as the spec's suggested timeline implies) — splitting 5 features across 2 people from Week 4 is what makes Week 5's "complete all 5" achievable without a crunch.
- [ ] User Researcher: draft the full Maze test plan (tasks, success metrics, recruitment script) so recruitment can start the moment the prototype is testable.

### Week 5 (20–26 Oct) — Complete Prototype + Start Recruitment
- [ ] Complete Figma prototype: all 5 features clickable, navigation + states + edge cases handled (empty states, error states — these are explicitly graded: "prototype quality: navigation, states, edge cases handled," 5 marks).
- [ ] **User Researcher: start participant recruitment now**, not Week 6 as the spec's suggested timeline implies — recruiting 5 real people who fit your target user profile, scheduling them, and getting the Maze test link ready is a multi-day process with real risk of slippage; starting a week early buffers that.
- [ ] Finalize Maze test tasks against the actual finished prototype (not the wireframe version).

### Week 6 (27 Oct–2 Nov) — Run the Test
- [ ] Run Maze with ≥5 real participants; collect raw data (Maze dashboard export + per-participant, per-task metrics).
- [ ] **Include at least one accessibility-relevant task or a participant with an accessibility need** if pursuing the bonus (1 mark, cheap to add here if planned, awkward to retrofit).
- [ ] Capture verbatim quotes during/after sessions — the rubric explicitly wants quotes, not paraphrases.
- [ ] Duplicate the current Figma file/pages before making any post-test changes (Figma version history is your "iteration evidence" — don't edit in place and lose the before-state).

### Week 7 (3–9 Nov) — Analyze, Iterate, Write
- [ ] Analyze Maze results; identify what to change.
- [ ] Iterate the prototype (v2), keeping v1 visible via Figma history/duplicated pages.
- [ ] Write Overall Design, Feature Details, Testing Method/Results/Discussion sections — these depend on real data so they genuinely can't start earlier, but Introduction, Related Work, and much of the walkthrough should already be drafted from Weeks 1–3, so this week is "finish," not "start from zero."
- [ ] Visual & UI Designer: start the PPT draft in parallel with report writing (screenshot-driven, not text-heavy — pull directly from the Figma before/after captures already in the report).

### Week 8 (10–15 Nov) — Finalize & Submit
- [ ] Project Lead: full QA pass — page count (≤20 excl. refs/appendices), every design decision traceable to a named HCI principle, every reference cited in body, workload table filled and matches the task log.
- [ ] Verify the Figma link is public (view/comment) — **test it in an incognito/private browser window**, not just "it worked for me."
- [ ] Record the ≤10 min video (structure: problem & users 1.5 min → user journey 1 min → design & 5 features live Figma walkthrough 4 min → Maze testing & results 2.5 min → conclusion & future direction 1 min). **Do a timed dry run at least once before the final recording** — 10 minutes disappears fast when demoing a live prototype.
- [ ] Package: one zip (report + PPT) submitted once by the group leader to Canvas; video uploaded separately to the video link (not in the zip).
- [ ] Confirm late-penalty policy timing with enough margin (submit same day, not at 23:58).

---

## Part 5 — Risks Identified in the Spec's Suggested Timeline (and how this plan fixes them)

1. **Week 7 overload.** The spec's suggested timeline puts "analyse results, iterate, write the report, draft PPT" all in one week. Fix: Related Work and Introduction start in Week 1–3; hi-fi work on all 5 features starts Week 4 (not just features 1–3) so Week 5 isn't a bottleneck.
2. **Recruitment risk.** Spec implies recruiting happens in Week 6 alongside running the test. Real recruitment (finding, screening, scheduling ≥5 people who match the target user group) takes longer than a same-week turnaround allows. Fix: recruitment plan is ready by Week 4, outreach starts Week 5.
3. **Losing "before" state during iteration.** The rubric explicitly wants dated v1 vs v2 comparisons. Editing the same Figma file in place risks losing the evidence. Fix: explicit "duplicate before you touch it" step before Week 7 iteration.
4. **Accessibility bonus as an afterthought.** Bolting on an accessibility audit in Week 7 produces a shallow, disconnected 2%. Fix: decision made Week 1 (pre-work), audit done Week 2 alongside the main heuristic evaluation, accommodations designed alongside the main redesign (not after), one Maze task/participant chosen with accessibility in mind from the Week 4 test plan.
5. **Workload declaration risk.** Markers explicitly flag members with no traceable contribution. Fix: shared task log from Week 1 (date, name, task, link to deliverable) doubles as the evidence base for the final declaration table.
6. **Non-screen modality scope creep.** Choosing voice/AR/robot adds a translation-layer writing requirement with no extra rubric credit. Fix: default recommendation is a screen-based app unless the team has specific relevant experience.
7. **Access failure at grading time.** "Marks deducted if markers can't access the Figma link" is an explicit, avoidable point loss. Fix: incognito-window test as an explicit Week 8 checklist item, not an assumption.
8. **Report page budget is tight.** Feature Details alone (4–6 pages for 5 features) leaves ~1 page/feature after subtracting captures. Fix: draft each feature write-up concisely from Week 3's one-sentence HCI-principle notes rather than writing loosely and cutting later.

---

## Part 6 — Final Submission QA Checklist (run this in Week 8, tied directly to Appendix II)

- [ ] Cover page: title, all names + SIDs, workload table (Name/SID/Role/Key tasks), leader marked with `*`.
- [ ] Intro: problem statement, target user group, app-choice justification, scope names the 5 features, scope is realistic for 5 people/8 weeks.
- [ ] Related Work: 10–20 refs, **all** cited in body, balanced across HCI theory / domain / modality, critical synthesis (not a summary list), each design decision traceable to a cited source.
- [ ] Overall Design: app overview, illustrated user journey with pain points, walkthrough with screen captures, rationale tied to **named** HCI principles, coherent/consistent across the whole interface.
- [ ] Feature Details (×5): annotated real-app evidence, named HCI principle(s), before/after captures, navigation/states/edge cases demonstrated, all clickable via the public link.
- [ ] Testing: method (recruitment, tasks, metrics, procedure) fully described, results with tables/figures + verbatim quotes, discussion linked back to design decisions, visible iteration evidence.
- [ ] Conclusion: summary matches the evidence actually presented, one concrete justified future direction, honest limitations.
- [ ] References list: 10–20, consistent citation style.
- [ ] Appendices: raw Maze export/dashboard screenshot, task script, Figma URL, extra captures.
- [ ] Figma link: public (view/comment), verified in an incognito window.
- [ ] Page count ≤20 (excl. references/appendices).
- [ ] PPT: screenshot-driven, no walls of text.
- [ ] Video: ≤10 min, live Figma walkthrough included, timed dry run done.
- [ ] Submission: one zip (report + PPT) via Canvas by the leader only; video uploaded separately.
