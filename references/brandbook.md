# Compiling the Brand Book

Everything else in this skill produces pieces — a name, a palette, a font pairing, a logo direction, a tagline. This file is where those pieces become one handoff-able thing, instead of staying scattered across chat messages.

## When to compile one

**Do compile a brand book:**
- Explicit ask — "put this all together," "make this a document," "give me the brand book," "compile everything," "I need something I can show someone."
- The end of a **full identity pass** (Phase 2 run end-to-end: name + archetype + palette + fonts + logo) — that was the implied deliverable of asking for "the whole thing," even if the user didn't say the word "document."
- The end of a **full three-phase run** (idea → brand → validate) — the natural closing artifact for the whole pipeline.

**Don't compile one for a single piecemeal ask** ("just give me colors," "one logo idea") — that stays in the chat reply per the usual file-creation judgment call. Offer it at the end instead: one line, "want this compiled into a brand doc once the rest is locked in?"

## What goes in it

A one-page brand book, in this order:

1. **Cover** — name, tagline, archetype (e.g. "Streetwear / Mascot Rebel").
2. **The one-liner** — the value proposition from `messaging.md`.
3. **Elevator pitch** — 3-4 sentences.
4. **Who it's for** — the target audience, stated specifically.
5. **Visual identity** — color palette as actual rendered swatches with hex codes and role labels, the font pairing named (heading/body), the logo direction described (and rendered if an SVG/image was produced).
6. **Voice** — 2-3 lines capturing the tone-of-voice row from `messaging.md`, plus the messaging pillars.
7. **Validation snapshot** (only if Phase 3 ran) — the verdict, the market-gap thesis in one line, and the headline score read (severity/frequency/whitespace/TAM at a glance). Skip this section entirely if validation hasn't run yet — don't fabricate a placeholder verdict.
8. **Status note** — if the brand was built before validation ran, say so plainly on the page itself ("provisional — pending validation"), so the document doesn't overstate certainty it doesn't have.

Keep it to one page's worth of content. This is a reference artifact, not an essay — density and scanability over exhaustive explanation.

## Choosing the output format

Check what's actually available in the current environment before picking:

- **If Claude Docs tools are available** → build it as a Doc. It's the right default for something the user will keep, edit, or send on.
- **If artifact publishing is available and no specific file format was requested** → build a single self-contained HTML page styled *using the brand's own chosen colors and fonts* — the brand book should look like the brand, not like a generic template. Publish it so it's a shareable link.
- **If the user explicitly names a format** (Word, PDF, PowerPoint) → honor that directly: the `docx`, `pdf`, or `pptx` skill respectively (read the matching SKILL.md before building, per this environment's standard skill-use rules). A one-page brand book maps naturally to a single-slide or few-slide deck if PowerPoint is requested.
- **If no file/artifact tooling is available at all** (plain text context) → lay the same content out cleanly in the chat reply itself, in the order above, clearly formatted — the structure matters more than the medium.

When in doubt and nothing above resolves it, ask once rather than guessing between formats that would take meaningfully different effort to produce.

## Keep it current

If the user comes back after validation changes the thesis, or after a name gets swapped, or after they pick a different archetype — recompile rather than leaving a stale brand book as the last word. Treat an existing brand book as a living document for this venture, not a one-time artifact.
