# Venture Builder

A Claude skill for turning an early product idea into a structured, research-backed venture direction — idea, validated, named, and branded, with a document to show for it.

## What it does

```
Idea
 ↓
Research
 ↓
Validation
 ↓
Survey
 ↓
Analysis
 ↓
Brand
 ↓
Messaging
 ↓
Brand Book
```

Instead of asking Claude disconnected questions like "give me startup ideas" or "name my startup," Venture Builder uses a structured workflow and a set of specialized reference files so the output is evidence-driven and consistent, not a one-off brainstorm that doesn't hold together.

`SKILL.md` is the orchestrator — it decides which phase a request needs and which reference file to pull. The `references/` files are the specialists: one for finding an idea, one for market/competitor/compliance research branched by business type, one for primary surveys, and five for the actual brand system (naming, visual style, color, type, logo, voice).

## The three phases

**1. Idea** — if there isn't one yet: founder-edge mapping, market-signal reading, problem-mining, scoring, convergence to a testable thesis.

**2. Brand** — name, visual style archetype, colors, fonts, logo direction, voice/messaging — picked as one coherent system, not four separate brainstorms.

**3. Validate** — real competitor/market research branched by business type (a SaaS idea and a cloud-kitchen idea get different research playbooks), a compliance check, a four-axis score, and a primary-research path (survey design → distribution → response analysis) when secondary research isn't enough.

Each phase works standalone too — ask for just a logo, or just a validation pass, and that's what you get.

## Install

**Claude.ai / Claude apps:** download the `.skill` file from [Releases](../../releases) and use the in-app "Add skill" / "Save skill" flow.

**Claude Code:**
```bash
git clone https://github.com/<your-username>/venture-builder.git
cp -r venture-builder ~/.claude/skills/venture-builder
```

## Use it

Just talk to it naturally — no special syntax:
- *"I don't have an idea yet, help me find one"*
- *"Is this idea any good — [describe it]"*
- *"Name a [X] brand for [audience]"*
- *"Build me a survey to validate this"*
- *"Put this all together into a brand book"*

See `examples/` for sample output on a worked (fictional) idea, start to finish.

## Structure

```
venture-builder/
├── SKILL.md                    orchestrator
├── references/
│   ├── idea-discovery.md
│   ├── idea-validation.md
│   ├── survey-design.md
│   ├── naming.md
│   ├── style-archetypes.md
│   ├── color-palettes.md
│   ├── typography.md
│   ├── logo-concepts.md
│   ├── messaging.md
│   ├── brandbook.md
│   └── anti-ai-slop.md
├── examples/
│   ├── example-validation.md
│   ├── example-survey.md
│   └── example-brandbook.md
├── CHANGELOG.md
└── LICENSE
```

## Why reference files, not one giant prompt

A single SKILL.md with everything inlined either stays shallow or blows past what's useful to load on every request. Splitting by phase means Claude reads only what a given request actually needs — a "give me a palette" ask loads one file, not eleven — and each file can go deep on its own domain without bloating the others.

## Contributing

Found a cliché `anti-ai-slop.md` missed, a research source that should be in `idea-validation.md`, or a style archetype worth adding? Open a PR or an issue.

## License

MIT — see [LICENSE](./LICENSE).

---

If this saved you a few days of disconnected ChatGPT tabs, a star helps other people find it.
