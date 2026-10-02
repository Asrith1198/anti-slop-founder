# Idea Validation

Use this once there's a specific idea (either the user already had one, or it came out of idea-discovery.md's Step 5 one-liner). The job here is to answer one question with evidence, not optimism: **is this a real, sufficiently painful, sufficiently large, sufficiently winnable problem — and does the proposed solution actually beat what's already out there?**

This is a research task — use web_search (and web_fetch on specific promising results) actively and in volume. A validation pass that runs 1-2 searches and declares an idea "validated" hasn't done the job; scale search volume to match the stakes of the decision.

## First: identify the business type — it decides where to look

Don't default to the SaaS/startup playbook (Product Hunt, G2, YC) for everything — that's the single biggest way a validation pass misses the real signal. Match the idea to the closest type below and research accordingly. An idea can span more than one; research both sets of sources when it does.

### Digital Product / SaaS / App
**Where to look:** Product Hunt (launch reception, comment sentiment), G2 / Capterra (mine the 1-2 star reviews of incumbents specifically — that's where unmet needs live), app store reviews for mobile, Y Combinator's current Requests for Startups and company directory (direct/adjacent funded competitors), Reddit/Indie Hackers/Hacker News threads, recent funding news in the category.
**Pain signal:** repeated complaints about a specific missing feature or workflow friction across multiple independent reviewers; people building their own janky workaround (Zapier chains, spreadsheets, scripts).
**Compliance flag:** data privacy obligations if handling personal data (consent, storage, cross-border transfer rules); app store policy compliance; payment-handling rules if processing transactions directly rather than through a PCI-compliant processor.

### Food & Hospitality (physical, local)
**Where to look:** Zomato/Swiggy ratings and review text for comparable local places, Google Maps reviews (read the 2-3 star ones — more diagnostic than 1-star rage or 5-star praise), local competitor density via maps search, Instagram/local food-community engagement on comparable accounts, footfall/rent cost signals for the target area if locatable.
**Pain signal:** recurring complaints about a specific gap (wait time, a missing cuisine/diet option, inconsistent quality, delivery radius) across multiple nearby competitors, not just one bad outlet.
**Compliance flag:** food safety/hygiene licensing (e.g. FSSAI in India), local health department permits, packaging/labeling rules if selling packaged goods — name these explicitly, don't assume they're handled.

### Fashion / D2C Physical Retail (streetwear, apparel, physical goods)
**Where to look:** Instagram/TikTok engagement on comparable small/independent labels (likes, comments, saves as interest proxy), marketplace density and reviews on platforms relevant to the market (Meesho/Myntra/Etsy/Amazon as applicable), small-brand founder threads on Reddit/Indie Hackers about sourcing and margin struggles, direct competitor sell-through signals (sold-out drops, restock announcements).
**Pain signal:** a specific aesthetic/niche with visible engaged demand but thin, low-quality, or absent supply from existing sellers; recurring complaints about fit, material quality, or price in competitor reviews/comments.
**Compliance flag:** textile/labeling regulations, import duties if sourcing internationally, trademark clearance on any graphic/mascot design before production (see naming.md's availability-check step — it applies to visual marks too, not just names).

### Marketplace / Platform (two-sided)
**Where to look:** both sides need separate research — supply-side forums (where potential sellers/providers complain about existing channels) and demand-side forums (where buyers complain about discovery/trust/price). Check existing marketplace players' app store and review-site complaints for the specific friction (trust/fraud, discovery, pricing transparency, fulfillment).
**Pain signal:** a chicken-and-egg gap where one side is underserved by existing platforms specifically (not "marketplaces are hard" in general, but a named, specific failure of the current options).
**Compliance flag:** intermediary/platform liability rules, payment escrow/aggregator licensing if holding funds between parties, data-sharing obligations between the two sides.

### Fintech / Financial Services
**Where to look:** G2/Capterra and app store reviews of incumbents (mine complaints about fees, speed, transparency, support), recent funding news (fintech is capital-intensive and regulation-sensitive, so funded-competitor signal matters more here than most categories), regulator announcements/news for the specific sub-category.
**Pain signal:** complaints about hidden fees, slow settlement, poor support, or a specific underserved segment incumbents don't bother serving well (a common fintech wedge).
**Compliance flag:** the highest-compliance-risk category by default — payment aggregator/PPI licensing, lending licenses, KYC/AML obligations, central-bank-adjacent rules (e.g. RBI guidelines in India). Flag this prominently and explicitly, don't bury it.

### Civic / Community / Hackathon / Non-commercial initiative
**Where to look:** engagement on comparable past initiatives (turnout, repeat participation, social reach), community forum discussion of the specific civic issue, local government/NGO reports on the issue if it's policy-adjacent.
**Pain signal:** this category often isn't "market" validation in the commercial sense — the right question is closer to "does this specific community actually want to mobilize around this," evidenced by prior turnout/engagement on adjacent efforts, not revenue signals.
**Compliance flag:** usually minimal, but check event permit requirements, data-collection rules if gathering participant information, and political-activity restrictions if sponsors/venues are involved.

### Local Services (offline: tutoring, repair, salons, consulting, etc.)
**Where to look:** Google/Justdial-type local-listing reviews of comparable providers, local Facebook/WhatsApp community group discussion, vertical platforms if the category has one (e.g. Practo/UrbanClap-type), direct competitor pricing and booking-friction signals.
**Pain signal:** recurring complaints about availability, pricing opacity, or quality inconsistency across multiple local providers.
**Compliance flag:** professional licensing specific to the service (tutoring generally light; health/beauty/financial-advisory services often licensed), local business registration.

### Content / Creator / Media
**Where to look:** engagement benchmarking on comparable creators/channels in the niche, comment-section complaints on adjacent content about what's missing or done badly, platform algorithm/monetization-policy news for the relevant platform.
**Pain signal:** an underserved angle within a proven-demand niche (the niche clearly has an audience; the specific angle/format/quality bar is the gap).
**Compliance flag:** usually light — note platform monetization-policy risk and copyright/licensing if using others' material.

## Synthesize into a validation brief

Pull the research into these sections, every claim traceable to something actually found (never invented statistics or made-up competitor names — if a number can't be sourced, say it's a rough estimate and flag it as such):

1. **Existing solutions landscape** — a short list of real competitors/alternatives (including "doing it manually" as a valid competitor), one line of positioning each.
2. **What users actually complain about** — the recurring pain points pulled from reviews/forums for the matched business type(s) above, paraphrased in your own words (never reproduce review text verbatim beyond a short attributed phrase — standard copyright/quotation limits apply).
3. **Bottlenecks and missing features/gaps** — the specific openings, as distinct from general complaints ("it's expensive" alone usually isn't actionable; a named missing feature or underserved segment is).
4. **The market-gap thesis** — the specific underserved angle this idea could own, stated as one sharp sentence. This is the sentence `messaging.md` builds the differentiation claim from — make it specific enough to actually ground a "why us," not a generic "there's an opportunity here."
5. **Competitive intensity read** — crowded-and-commoditized, crowded-but-fragmented (room for a focused player), or genuinely open.
6. **Rough market size** — directional, sourced appropriately for the business type (platform user counts / app download estimates for digital; population + local competitor density for physical/local; comparable-niche audience size for content).
7. **Compliance/regulatory check** — name the specific licenses, registrations, or rules that apply per the business-type table above, even if the answer is "minimal" — don't silently skip this section.

## Score it

| Axis | What it measures | Signal to look for |
|---|---|---|
| Severity | How much does this problem actually hurt, versus being a minor annoyance people tolerate? | Do people pay to solve it already, or build workarounds, or just complain and move on? |
| Frequency | How often does the target user hit this problem? | Daily/weekly friction is a stronger foundation than something hit once a year. |
| Market Whitespace | How much of the pain is currently unaddressed by existing options? | Repeated reviews/complaints citing the same gap = whitespace; near-silence on this specific angle = either no pain or it's already well-served. |
| TAM | How many people/businesses plausibly have this problem? | Directional size, sourced per business type as above. |

Give an honest read on each axis (strong / moderate / weak) — the point of this pass is to catch a weak idea before it costs months, not to produce a reassuring report.

## Validation integrity checklist

- **Did I look for disconfirming evidence, not just supporting evidence?** Actively search "why [category] fails" or "[competitor] alternative" threads where people explain why they *didn't* adopt something in this space.
- **Am I treating a handful of posts as proof of a large market?** A real pattern needs multiple independent sources repeating the same complaint.
- **Am I confusing stated preference with revealed preference?** "I'd use that" is weak; "I pay $X/month for a workaround" is strong.
- **Have I actually named the competitors, or hand-waved "no one does this"?** "No one does this" is almost always false and usually means the research wasn't thorough enough.
- **Did I run the compliance check, or skip straight to market signal?** A great market-gap thesis with an unmentioned licensing wall isn't actually validated.

## Verdict

End with a direct call: **proceed**, **proceed with a narrower/adjusted angle** (state the adjustment), or **weak — here's specifically why, and what evidence would change that read**.

**If weak, and this idea came out of idea-discovery.md** — explicitly loop back. Name the other finalist(s) from that phase's Step 5 and offer to run this same validation pass on the next one, rather than ending the conversation at "weak" with nothing to do next.

**If proceed or adjusted** — hand off cleanly: the market-gap thesis feeds `messaging.md`'s differentiation statement, and if Phase 2's brand work was already done provisionally before this validation ran, flag explicitly whether anything about the positioning now needs to change given what the research found.

When the research is thin or genuinely inconclusive either way, say so plainly and point to primary research (survey-design.md) as the next step to close the gap, rather than forcing a confident verdict the secondary research doesn't support.
