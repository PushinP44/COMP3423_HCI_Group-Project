# Accessibility Audit — [App Name]

*Owner: Member 5 (Accessibility & Evaluation Lead), Week 2. Feeds the +5% accessibility bonus (2% for this audit being documented). WCAG-basics checklist — not a full WCAG conformance audit, just the items the spec calls out explicitly.*

## Contrast

- [ ] Check text/background contrast ratio on key screens (balance display, transfer confirmation, error messages) — WCAG AA minimum is 4.5:1 for normal text, 3:1 for large text. Use a contrast checker tool on real screenshots.
- Findings: [FILL IN]

## Touch target size

- [ ] Check tap target size on key interactive elements (numeric keypad, buttons, list items) — WCAG/mobile guidance recommends ≥44x44pt (iOS) / ≥48x48dp (Android).
- Findings: [FILL IN]

## Text scaling

- [ ] Test the app with the OS system font size increased (iOS: Settings > Accessibility > Display & Text Size; Android: Settings > Accessibility > Font size) — does layout break, does text get cut off?
- Findings: [FILL IN]

## Screen-reader compatibility

- [ ] Test key flows with a screen reader on (iOS VoiceOver / Android TalkBack) — are interactive elements labeled meaningfully, or does the reader just say "button, button, button"?
- Findings: [FILL IN]

## Summary for report

[FILL IN once the above is done — 2-3 sentences summarizing the overall accessibility posture of the existing app, to go in `report/03-overall-design.md` §3.5.]

## Accommodations planned for the redesign

[FILL IN in Week 3-4, alongside the main redesign, not after — list per-feature accommodations here, then reference them in `report/04-feature-details.md`.]
