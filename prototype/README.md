# HTML/CSS Redesign Prototype — "Nova Bank" (placeholder brand)

Real, working HTML/CSS screens for the 5 features, built as a starting draft from the plan's initial pain-point hypotheses (`../2026-09-16-comp3423-project-plan.md`, Part 2). **This is a first-pass design draft, not final** — the team should revise it once the real app's actual usability problems are confirmed (`../research/heuristic-evaluation.md`, `../research/candidate-usability-problems.md`), and re-brand away from "Nova Bank" once you've picked/confirmed the specific real app being redesigned.

## Why HTML/CSS instead of building directly in Figma

Figma's canvas can only be edited inside the real Figma app (no API/automation path for creating design content). Writing real HTML/CSS here means: (a) it's genuinely reusable if the team wants a coded prototype at all, and (b) it imports cleanly into Figma as editable layers via the `html.to.design` plugin — much faster than manually redrawing 14 screens from scratch.

## Screens (14 files, 5 features)

| Feature | Files |
|---|---|
| 1. Home Dashboard & Quick Actions | `home.html` |
| 2. Simplified Transfer Flow | `transfer-details.html` → `transfer-confirm.html` → `transfer-success.html` / `transfer-error.html` (edge case) |
| 3. Bill Pay Findability | `billpay.html` → `billpay-confirm.html` → `billpay-success.html` |
| 4. Transaction Status Visibility | `transactions.html` → `transaction-detail.html?state=success\|pending\|failed\|success2` |
| 5. Accessible Account Overview | `account.html` |

Open `index.html` to preview all 14 screens at once (this file is a picker only, not part of the app itself).

## How to import into Figma via html.to.design

1. **Serve the folder locally** so the plugin can fetch real URLs (it can't read `file://` paths reliably):
   ```bash
   cd prototype
   npx serve .
   # or: python3 -m http.server 8080
   ```
2. In the Figma desktop or web app, open your project file, then **Plugins → html.to.design**.
3. Use **"Import from URL"**, pointing at each screen's local URL one at a time (e.g. `http://localhost:3000/home.html`) — import all 14 for full coverage, or start with the 5 primary screens (`home.html`, `transfer-confirm.html`, `billpay.html`, `transactions.html`, `account.html`) if you want to hand-build the secondary states directly in Figma instead.
4. The plugin drops each import as a new frame — rename frames to match the feature naming in `../report/04-feature-details.md`, then wire up prototype links (Figma's own click-through connections) between frames to match the navigation these HTML files already demonstrate.
5. Once imported, this becomes a normal Figma file — restyle, adjust, and iterate there. Treat the HTML as the starting draft, not a locked spec.

## What still needs the real team/app

- Swap "Nova Bank" branding for your actual chosen app (or keep a rebrand if the team prefers presenting the redesign under a new name — check this is fine with the rubric's "coherent and consistent" requirement either way).
- Replace the 5 draft features here if the real heuristic evaluation turns up different/better-evidenced problems.
- Every "before" screenshot in the report must still come from the real existing app — these HTML screens are the "after" only.
