# Primary Research: Surveys & Data Analysis

Secondary research (idea-validation.md) tells you what's publicly visible. A survey closes the gap by reaching the user's own target audience directly — and as a side effect, starts building an early audience before launch. Use this when the secondary research is inconclusive, when the user wants to reach their own network/community for a direct read, or whenever they explicitly ask for a survey.

## Designing the survey

**Keep it short.** 5-10 questions max — completion rate falls off fast past that, and a 40% complete 8-question survey beats a 5% complete 20-question one every time.

**Structure, in order:**
1. **Screening question(s)** — confirm the respondent is actually in the target audience (e.g. "Do you currently do/use/deal with [X]?"). If they're not, the rest of their answers are noise — design the flow so off-target respondents can exit early rather than forcing answers from people outside the target group.
2. **Current-behavior questions** — how do they handle this today? What do they use, pay for, or work around with? This is far more reliable than hypothetical questions.
3. **Frequency/severity questions** — how often does this come up, how much does it cost them (time, money, frustration) when it does?
4. **One open-ended question** — "What's the most frustrating part of [X] for you?" or "If you could fix one thing about how you currently handle this, what would it be?" Open text is where the sharpest, most quotable insight usually comes from.
5. **A willingness-to-pay or commitment signal** (if relevant) — not "would you pay for this" (weak, hypothetical, people are polite), but something with actual friction: "would you join a waitlist," "would you give your email for early access," or a real price-anchored question ("would $X/month be reasonable, too high, or too low for solving this").
6. **Optional contact opt-in** — "Open to a quick 15-min chat about this? Leave your email/handle." This is the single highest-value question in the whole survey — it's what turns the survey from a one-way data pull into a pipeline of real interview candidates.

**Avoid:**
- Leading or loaded phrasing ("Don't you think X is frustrating?") — ask neutrally and let the answer tell you, don't plant the answer in the question.
- Double-barreled questions (two things being asked at once — split them).
- Pure hypotheticals ("Would you use an app that...") as the main evidence — they're useful color, not proof.

## Building and distributing it

Two paths — ask which fits, or default based on what the user seems to want:

**A. A shareable page Claude builds and publishes directly.** Build it as a clean HTML form (follow this environment's artifact-publishing rules) and use the shared persistent-storage capability so every respondent's submission accumulates in one place, keyed by a response ID. Include a lightweight results view on the same page (e.g. behind a simple "view results" toggle or a separate state) that lets the page owner see the aggregated/raw responses — they can then copy that out and paste it back into the conversation for analysis. This keeps the whole loop (build → distribute → collect → analyze) inside tools already available, with no third-party account needed.

**B. Questions formatted for an existing tool (Google Forms, Typeform, etc.)** — when the user already has a preferred survey tool, or wants built-in analytics/export the user's own tool provides. In this case just hand over the finished question set, cleanly formatted and ready to paste in, rather than building a page.

Either way: once it's live, the user distributes the link themselves (their network, relevant communities, social) — Claude doesn't have a way to push distribution on its own.

## When the data comes back

The user will paste or drop the collected responses back into the conversation. Analyze it as real primary data, not a formality:

1. **Segment** — group responses by whatever natural clusters appear (e.g. by how they currently solve the problem, by severity level, by any demographic/role field collected).
2. **Surface the sharpest verbatim quotes** — since this is the user's own collected data (not third-party published content), quoting respondents directly is fine and often the most persuasive part of the output; pull the 3-5 quotes that best capture the real pain in the respondents' own words.
3. **Recompute the validation score** from idea-validation.md's four-axis frame (Severity / Frequency / Market Whitespace / TAM) using the real data instead of inferred-from-reviews data — note explicitly where the survey confirmed, contradicted, or added nuance to the earlier secondary-research read.
4. **Flag follow-up interview candidates** — respondents who opted into the contact question, especially ones with high-severity/high-specificity answers. List them by response label (e.g. "Respondent 7 — left contact info, described a daily workaround costing ~2 hrs/week") rather than inventing or assuming any identity beyond what they actually provided.
5. **Point to where to find more candidates beyond the survey**, if more depth is needed — real public venues where this exact audience is known to gather (a specific relevant subreddit, an Indie Hackers/niche Discord community, a LinkedIn/X search query targeting the role or interest) based on where the secondary research in idea-validation.md already found them talking. Never fabricate or guess at specific named private individuals to "contact" — only point to public communities/search strategies, or the respondents who themselves opted in.
6. **Give the same direct verdict idea-validation.md calls for** — proceed, adjust, or weak — updated for what the primary data actually showed, including if it overturned the secondary-research read entirely (that's a legitimate and valuable outcome, not a failure of the process).

## Caveats to flag honestly in the analysis

- **Sample size and self-selection** — a survey shared mostly within the founder's own network skews toward people predisposed to be supportive; say so rather than presenting 20 friendly responses as proven market demand.
- **Small samples don't support precise percentages** — "6 of 8 respondents mentioned X" is honest; "75% of users face this problem" overstates what 8 responses can support.
