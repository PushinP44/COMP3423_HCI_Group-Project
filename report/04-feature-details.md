# 4. Feature Details (4–6 pages)

*Owner: shared, one feature per person is a natural split (5 features, 5 people). Rubric: 20% total — all 5 features prototyped & clickable (4), annotated real-app problem evidence (4), named HCI principles (3), before/after captures (4), prototype quality: nav/states/edge cases (5).*

Budget ~1 page per feature after captures — write concisely. (b) and (d) below are draft design rationale from the plan's initial hypothesis — refine once the real heuristic evaluation is done. (a) and (c) need the real app's screenshots and your actual Figma frames once you've built them.

---

## 4.1 Feature: Home Dashboard & Quick Actions *(owner: Member X)*

**(a) Existing problem — annotated evidence**
[FILL IN — annotated screenshot from `assets/screenshots/existing-app/` showing frequent actions (transfer, pay bills) buried under menus rather than surfaced on the home screen.]

**(b) HCI principle(s) violated**
Draft: Nielsen's *Recognition Rather Than Recall* — users must remember where a frequent action lives rather than seeing it presented directly; and *Efficiency of Use* — frequent tasks require more navigation steps than their frequency justifies. Cite the real source once added to `report/references.md`.

**(c) Redesign — before/after**
[FILL IN — Figma frame link + before/after captures once designed.]

**(d) Design rationale**
Surface the most frequent actions as a single-tap quick-actions row directly on the home screen, reducing the frequent-task path from menu-navigation to one tap. Tradeoff to weigh: a fully customizable quick-actions row (user-chosen) adds settings-UI complexity without directly addressing the identified problem — probably not worth it for this scope.

---

## 4.2 Feature: Simplified Transfer Flow *(owner: Member X)*

**(a) Existing problem — annotated evidence**
[FILL IN — annotated screenshot(s) of the real app's transfer flow showing excess confirmation steps and/or unclear post-submit feedback.]

**(b) HCI principle(s) violated**
Draft: Nielsen's *Visibility of System Status* — if the existing flow gives no clear feedback during/after submission, and *Error Prevention* / *Help Users Recognize, Diagnose, and Recover from Errors* — if a failed transfer doesn't clearly state whether funds moved.

**(c) Redesign — before/after**
[FILL IN — Figma frames + before/after captures once designed.]

**(d) Design rationale**
Collapse to a short flow (details → review & confirm) with one explicit confirmation screen, plus a dedicated success state and an edge-case failure state that explicitly states whether funds were deducted — directly addressing system-status visibility and error recovery. Tradeoff to weigh: a single-step "instant send" (no review screen) removes the one confirmation point needed to catch entry mistakes before an irreversible transfer — probably keep the review step.

---

## 4.3 Feature: Bill Pay Findability *(owner: Member X)*

**(a) Existing problem — annotated evidence**
[FILL IN — annotated screenshot showing bill pay buried in navigation or hard to locate in the real app.]

**(b) HCI principle(s) violated**
Draft: Nielsen's *Recognition Rather Than Recall* (same underlying issue as 4.1, applied specifically to bill pay) and *Match Between System and the Real World* — if biller names/search don't match how users actually think of their bills.

**(c) Redesign — before/after**
[FILL IN — Figma frames + before/after captures once designed.]

**(d) Design rationale**
Surface saved billers immediately with due dates and typical amounts pre-filled, cutting the pay-a-bill path to as few taps as possible for a recurring biller. Tradeoff to weigh: auto-pay/scheduling adds a recurring-payments data model beyond a 5-feature, 8-week redesign — probably out of scope, but worth naming explicitly in the report's scope paragraph if considered and cut.

---

## 4.4 Feature: Transaction Status Visibility *(owner: Member X)*

**(a) Existing problem — annotated evidence**
[FILL IN — annotated screenshot of the real app's transaction list/history showing unclear or missing status indication.]

**(b) HCI principle(s) violated**
Draft: Nielsen's *Visibility of System Status* — the core principle this feature addresses directly; a transaction with no clear status leaves users unsure whether money actually moved.

**(c) Redesign — before/after**
[FILL IN — Figma frames + before/after captures once designed.]

**(d) Design rationale**
Give every transaction an explicit status (completed/processing/failed) that pairs color with text — not color alone, which also matters for Feature 5's accessibility angle — and make a failed transaction's detail view explicitly state whether funds moved, with a direct retry action. Tradeoff to weigh: real-time push notifications for status changes require backend/notification infrastructure outside this project's scope — worth naming as a Future Work candidate (`report/06-conclusion.md`) rather than attempting it.

---

## 4.5 Feature: Accessible Account Overview *(owner: Member X)*

**(a) Existing problem — annotated evidence**
[FILL IN — this one should be backed directly by `research/accessibility-audit.md` findings: contrast, touch target size, text scaling, screen-reader labeling issues in the real app.]

**(b) HCI principle(s) violated**
Draft: WCAG 2.x basics (contrast minimum 4.5:1, target size ≥44×44pt) framed through Nielsen's *Accessibility/Flexibility* lens — cite the real WCAG source and any accessibility-specific HCI literature from `report/02-related-work.md` once added.

**(c) Redesign — before/after**
[FILL IN — Figma frame + before/after captures once designed.]

**(d) Design rationale**
Meet a 44×44pt minimum touch target on all interactive elements, keep focus states visibly distinct (not just default browser outline), and make sure status/labels pair text with color rather than color alone. Document the accommodation decisions directly next to the accessibility settings in the design (not just in the report) so the connection between audit finding and redesign choice is easy for markers to trace, per the rubric's "accessibility accommodations shown and explained" bonus item.

---

## Prototype quality checklist (verify before submission, per feature)

- [ ] Feature 1 (Home) — quick actions + activity list all wired up and clickable.
- [ ] Feature 2 (Transfer) — details → confirm → success **and** error state designed and linked; error state doesn't just dead-end.
- [ ] Feature 3 (Bill Pay) — list → confirm → success designed and linked.
- [ ] Feature 4 (Transaction Status) — list → detail designed; all relevant status states (completed/processing/failed) represented as distinct, linked frames.
- [ ] Feature 5 (Account) — accessibility accommodations visible and explained in the design itself, not just described in the report.
- [ ] All 5 reachable from a shared, consistent navigation pattern, not isolated/orphaned frames.
- [ ] Figma link tested in an incognito window (view/comment access confirmed).
