# Example: Validation Brief

*Fictional worked example — an invented idea, used to show the output format `idea-validation.md` produces. No real research data.*

**Idea:** "QueueCut" — students at a specific engineering college pre-order canteen food through an app and skip the lunch queue, picking up at a set time.

**Business type:** Hybrid — Local Service (a single campus canteen) + Digital Product (the ordering app). Both source sets apply.

---

## Existing solutions landscape
- **General food-delivery apps** (Swiggy/Zomato-style) — don't serve in-campus canteens; wrong format entirely.
- **WhatsApp/manual pre-ordering** — some canteens informally let regulars message ahead; no system, breaks down past a handful of people.
- **Campus ID/payment apps** — handle fees and attendance, not food ordering.
- **Direct competitor for this specific wedge:** none found.

## What users actually complain about
Recurring themes across campus-forum-style discussion and comparable-college complaints: 15-20 minute queue times during the single shared lunch window; cash-only confusion at peak hours; "holding a spot" for friends causing regular arguments in line; no way to know if a dish has run out before reaching the counter.

## Bottlenecks and gaps
No canteen-scoped ordering tool exists — general delivery apps don't integrate with a single institution's canteen POS, and no competitor is building for the single-campus use case specifically. The gap isn't "food ordering" in general (solved, crowded); it's "skip a physical queue I'm otherwise forced into."

## The market-gap thesis
**Engineering students at single-canteen campuses lose 15-20 minutes of a 45-50 minute lunch break to a queue that a scheduled-pickup app would eliminate — and no existing food app is scoped to solve it at the single-campus level.**

## Competitive intensity
Open. Low competition specifically because the addressable market per campus is small enough that general food-delivery players have no reason to build for it — which is exactly what makes it winnable for a focused, single-campus-first player.

## Rough market size
Directional only: a mid-size engineering college runs ~3,000-6,000 students, a meaningful fraction of whom use the canteen daily. Scoped to one campus this is a small pilot market by design — the real size comes from replicating across multiple colleges in the region once the model is proven, not from one campus alone.

## Compliance/regulatory check
- Food safety licensing (FSSAI-equivalent) sits with the canteen operator, not the app — confirm the canteen already holds it rather than assuming.
- If the app handles payment directly, routing through an existing UPI/payment-gateway provider avoids needing a separate payment-aggregator license; holding funds directly would not.
- Data collected (student IDs, order history) should have a basic, stated privacy policy even at pilot scale.

---

## Score

| Axis | Read | Why |
|---|---|---|
| Severity | Moderate | Annoying, not devastating — but a recurring, universally-felt friction in a fixed time window. |
| Frequency | Strong | Daily, for anyone eating at the canteen. |
| Market Whitespace | Strong | No scoped competitor; the gap is structural (campus-specific), not just underserved. |
| TAM | Weak-to-moderate at single-campus scope | Real size requires multi-campus rollout; stated honestly as a pilot-scale idea, not a large-market one on its own. |

## Validation integrity checklist
- Looked for disconfirming evidence: checked whether canteens might resist a third-party ordering layer (operational friction, staff workflow change) — a real adoption risk, noted rather than ignored.
- Didn't treat a handful of informal complaints as proof of a large market — frequency/severity read as moderate-strong, not inflated to "massive pain."
- Compliance section run in full rather than skipped, despite being a low-regulation category.

## Verdict
**Proceed, with a narrower angle: single-campus pilot first**, not a general multi-campus launch. The whitespace and frequency signals are real; the TAM only becomes interesting after the pilot proves canteen-side adoption is possible — that operational risk (getting a canteen to actually change its workflow) is the real thing to test next, more than demand from the student side.
