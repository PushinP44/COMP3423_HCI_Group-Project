# 4. Feature Details (4–6 pages)

*Owner: shared, one feature per person is a natural split (5 features, 5 people). Rubric: 20% total — all 5 features prototyped & clickable (4), annotated real-app problem evidence (4), named HCI principles (3), before/after captures (4), prototype quality: nav/states/edge cases (5).*

Budget ~1 page per feature after captures — write concisely. (b) and (d) below are drafted from the plan's hypothesis and the `prototype/` HTML build; (a) and (c) still need the real app's screenshots and the actual Figma frames once imported — see `prototype/README.md`.

---

## 4.1 Feature: Home Dashboard & Quick Actions *(owner: Member X)*

**(a) Existing problem — annotated evidence**
[FILL IN — annotated screenshot from `assets/screenshots/existing-app/` showing frequent actions (transfer, pay bills) buried under menus rather than surfaced on the home screen.]

**(b) HCI principle(s) violated**
Draft: Nielsen's *Recognition Rather Than Recall* — users must remember where a frequent action lives rather than seeing it presented directly; and *Efficiency of Use* — frequent tasks require more navigation steps than their frequency justifies. Cite the real source once added to `report/references.md`.

**(c) Redesign — before/after**
[FILL IN — Figma frame link, once `prototype/home.html` is imported. Draft after-state: `prototype/home.html`.]

**(d) Design rationale**
The redesign surfaces the 4 most frequent actions as a single-tap quick-actions row directly below the balance card, reducing the frequent-task path from menu-navigation to one tap. Tradeoff considered: a fully customizable quick-actions row (user-chosen) was rejected for this scope — adds settings-UI complexity without directly addressing the identified problem.

---

## 4.2 Feature: Simplified Transfer Flow *(owner: Member X)*

**(a) Existing problem — annotated evidence**
[FILL IN — annotated screenshot(s) of the real app's transfer flow showing excess confirmation steps and/or unclear post-submit feedback.]

**(b) HCI principle(s) violated**
Draft: Nielsen's *Visibility of System Status* — if the existing flow gives no clear feedback during/after submission, and *Error Prevention* / *Help Users Recognize, Diagnose, and Recover from Errors* — if a failed transfer doesn't clearly state whether funds moved.

**(c) Redesign — before/after**
[FILL IN — Figma frames, once `prototype/transfer-details.html`, `transfer-confirm.html`, `transfer-success.html`, `transfer-error.html` are imported.]

**(d) Design rationale**
Collapsed to a 2-step flow (details → review & confirm) with one explicit confirmation screen, plus a dedicated success state and an edge-case failure state that explicitly states no funds were deducted (`transfer-error.html`) — directly addressing system-status visibility and error recovery. Tradeoff: a single-step "instant send" (no review screen) was rejected — removes the one confirmation step needed to catch entry mistakes before an irreversible transfer.

---

## 4.3 Feature: Bill Pay Findability *(owner: Member X)*

**(a) Existing problem — annotated evidence**
[FILL IN — annotated screenshot showing bill pay buried in navigation or hard to locate in the real app.]

**(b) HCI principle(s) violated**
Draft: Nielsen's *Recognition Rather Than Recall* (same underlying issue as 4.1, applied specifically to bill pay) and *Match Between System and the Real World* — if biller names/search don't match how users actually think of their bills.

**(c) Redesign — before/after**
[FILL IN — Figma frames, once `prototype/billpay.html`, `billpay-confirm.html`, `billpay-success.html` are imported.]

**(d) Design rationale**
Saved billers are surfaced immediately with due dates and typical amounts pre-filled, cutting the pay-a-bill path to 2 taps for a recurring biller. Tradeoff: auto-pay/scheduling was considered but out of scope — adds a recurring-payments data model beyond a 5-feature, 8-week redesign.

---

## 4.4 Feature: Transaction Status Visibility *(owner: Member X)*

**(a) Existing problem — annotated evidence**
[FILL IN — annotated screenshot of the real app's transaction list/history showing unclear or missing status indication.]

**(b) HCI principle(s) violated**
Draft: Nielsen's *Visibility of System Status* — the core principle this feature addresses directly; a transaction with no clear status leaves users unsure whether money actually moved.

**(c) Redesign — before/after**
[FILL IN — Figma frames, once `prototype/transactions.html` and `transaction-detail.html` (all 3 states) are imported.]

**(d) Design rationale**
Every transaction carries an explicit status badge (completed/processing/failed) that pairs color with text (not color alone — also an accessibility consideration, ties to Feature 5), and a failed transaction's detail screen explicitly states funds were not moved plus offers a direct retry action. Tradeoff: real-time push notifications for status changes were considered but require backend/notification infrastructure outside a static-prototype scope — noted as a Future Work candidate (`report/06-conclusion.md`).

---

## 4.5 Feature: Accessible Account Overview *(owner: Member X)*

**(a) Existing problem — annotated evidence**
[FILL IN — this one should be backed directly by `research/accessibility-audit.md` findings: contrast, touch target size, text scaling, screen-reader labeling issues in the real app.]

**(b) HCI principle(s) violated**
Draft: WCAG 2.x basics (contrast minimum 4.5:1, target size ≥44×44pt) framed through Nielsen's *Accessibility/Flexibility* lens — cite the real WCAG source and any accessibility-specific HCI literature from `report/02-related-work.md` once added.

**(c) Redesign — before/after**
[FILL IN — Figma frame, once `prototype/account.html` is imported.]

**(d) Design rationale**
All interactive elements meet a 44×44pt minimum touch target, focus states are visible (not just default browser outline), and status/labels pair text with color rather than color alone. The screen also documents the accommodation decisions directly (accessibility toggles + rationale note) so the connection between audit finding and redesign choice is traceable, per the rubric's "accessibility accommodations shown and explained" bonus item.

---

## Prototype quality checklist (verify before submission, per feature)

- [ ] Feature 1 (Home) — `prototype/home.html` imported and wired to all 4 quick actions + activity list.
- [ ] Feature 2 (Transfer) — details → confirm → success **and** error state imported and linked; error state doesn't just dead-end.
- [ ] Feature 3 (Bill Pay) — list → confirm → success imported and linked.
- [ ] Feature 4 (Transaction Status) — list → detail imported; all 3 status states (completed/processing/failed) represented as distinct, linked frames in Figma (the HTML uses one templated file with a query param — Figma needs 3 separate frames/variants).
- [ ] Feature 5 (Account) — `prototype/account.html` imported, accessibility toggles/notes visible.
- [ ] All 5 reachable from a shared bottom-nav pattern in Figma (matches `prototype/styles.css` `.bottom-nav`), not isolated/orphaned frames.
- [ ] Figma link tested in an incognito window (view/comment access confirmed).
- [ ] "Nova Bank" placeholder branding replaced with the real chosen app's identity (or an intentional rebrand, noted as such in the report).
