# Example: Survey + Analysis

*Fictional worked example, continuing the QueueCut idea from `example-validation.md`. The responses below are invented to illustrate what an analysis looks like — not real data from real people.*

## The survey (per `survey-design.md`)

1. **Screening:** Do you eat at the [campus] canteen during the lunch break? *(Yes / No — No exits the survey)*
2. **Current behavior:** How do you usually get your food? *(Queue normally / Have a friend hold a spot / Skip lunch some days / Other)*
3. **Frequency/severity:** On a typical day, about how many minutes do you spend waiting in the canteen line?
4. **Open-ended:** What's the most frustrating part of the canteen experience for you?
5. **Commitment signal:** Would you pre-pay a small convenience fee (e.g. ₹5-10) to skip the line and have your order ready at a set pickup time? *(Yes, definitely / Maybe, depends on the fee / No)*
6. **Contact opt-in:** Want early access when this launches? Leave your email or phone *(optional)*.

9 questions would be excessive for this ask — kept to 6, screening included.

## Fictional responses (illustrative sample, n=11)

| # | Wait time | Frustration (open-ended) | Would pay? | Opted in? |
|---|---|---|---|---|
| 1 | 20 min | "Friends holding 4 spots at once, it's chaos" | Yes, definitely | Yes |
| 2 | 15 min | "Never know if the good dish ran out till I reach" | Maybe | No |
| 3 | 10 min | "It's fine honestly" | No | No |
| 4 | 25 min | "I just skip lunch some days, not worth it" | Yes, definitely | Yes |
| 5 | 18 min | "Cash confusion, no one has change" | Maybe | No |
| 6 | 20 min | "Queue holding for friends" | Yes, definitely | No |
| 7 | 12 min | "Not that bad for me" | No | No |
| 8 | 22 min | "Lose half my break just standing there" | Yes, definitely | Yes |
| 9 | 15 min | "Fine most days, bad on non-veg days" | Maybe | No |
| 10 | 19 min | "Spot-holding arguments happen weekly" | Yes, definitely | Yes |
| 11 | 8 min | "No real complaints" | No | No |

## Analysis (per `survey-design.md`'s framework)

**Segments:** a clear split — roughly 55% (6/11) report 18+ minute waits and strong willingness to pay; the remaining 45% have shorter waits (8-15 min) and are lukewarm-to-no on paying. Wait time, not general sentiment, is the real segmenting variable.

**Sharpest quotes:** *"Friends holding 4 spots at once, it's chaos"* and *"Spot-holding arguments happen weekly"* — two independent respondents naming the same specific friction (queue-holding disputes), stronger signal than either alone. *"I just skip lunch some days, not worth it"* is the most severe data point in the set — that's a respondent opting out of eating rather than tolerating the queue.

**Rescored against `example-validation.md`:** Severity moves from "moderate" to **moderate-strong** — the skipped-meals data point is a more severe signal than the secondary research alone surfaced. Frequency and whitespace reads hold. TAM is unchanged (survey can't speak to multi-campus size).

**Follow-up interview candidates:** Respondents 1, 4, 8, and 10 opted in and gave the highest-severity answers — worth a 15-minute call with these four specifically before building anything, rather than a broader sample.

**Caveats:** n=11 is a small, self-selected sample (likely shared first in the respondent's own friend group) — directionally useful, not statistically representative. Treat "55% would pay" as "about half, in this small sample," not a precise market percentage.

**Updated verdict:** Consistent with `example-validation.md` — proceed with the single-campus pilot, with the four opted-in high-severity respondents as the first interviews before writing any code.
