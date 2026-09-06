# Installation & Usage Guide

The **PM Resume Builder** is a Claude Skill: a packaged set of instructions and references that Claude loads automatically whenever you ask it to build or improve a product-manager resume.

There are three ways to use it.

---

## Option 1 — Install in Claude.ai (easiest)

1. Download **[`pm-resume-builder.skill`](../pm-resume-builder.skill)** from this repository.
2. In Claude.ai, open **Settings → Capabilities → Skills** (or **Settings → Skills**).
3. Click **Upload skill** and select the `.skill` file.
4. Start a chat and say: *"Help me build my product manager resume."* Attach your current CV if you have one.

> **What is a `.skill` file?** A zip of the skill's instructions (`SKILL.md`) and reference guides. Once uploaded, Claude uses it automatically when your request is about a PM resume — you don't have to invoke it manually.

**Requirement:** the skill uses Claude's **`docx`** capability to produce the Word file and a PDF. This works in Claude.ai and Claude Code where document tools are available.

---

## Option 2 — Use with Claude Code / the Agent SDK

Clone and drop the skill into your user skills directory:

```bash
git clone https://github.com/Shehabov/pm-resume-builder-skill.git
cp -r pm-resume-builder-skill/skill/ ~/.claude/skills/user/pm-resume-builder/
```

Then, in any Claude Code session, ask: *"Rebuild my PM resume from this file"* and attach or point to your CV. Claude will read the skill, run the flow, and write both `.docx` and `.pdf`.

---

## Option 3 — Read the guides manually (no install)

The reference files in [`skill/references/`](../skill/references/) are standalone playbooks you can apply by hand:

| File | What you'll learn |
|---|---|
| [`pm-bullet-writing.md`](../skill/references/pm-bullet-writing.md) | The PM bullet formula, action verbs, before/after rewrites |
| [`pm-metrics-and-impact.md`](../skill/references/pm-metrics-and-impact.md) | Which metrics to show by PM archetype, how to quantify vague wins |
| [`pm-resume-structure.md`](../skill/references/pm-resume-structure.md) | Section order, summary, layout, fonts, ATS export |
| [`ats-and-keywords.md`](../skill/references/ats-and-keywords.md) | ATS reality + a PM keyword bank + JD tailoring |
| [`common-mistakes.md`](../skill/references/common-mistakes.md) | The PM-specific traps that get resumes screened out |
| [`pm-templates.md`](../skill/references/pm-templates.md) | The 5 templates and how to trigger each |

---

## How to use it (the flow)

Once installed, the skill runs a simple, guided flow:

1. **Give it your current CV** (attach a PDF/DOCX, or paste it). No CV? It builds from scratch by asking.
2. **Claude diagnoses it** in a few lines — what's weak and why.
3. **Claude asks targeted questions** — target role, PM archetype (Growth / Core / Platform / AI / Monetization / 0→1), scope per role, and the missing numbers.
4. **You pick a template** (or ask Claude to recommend one for your seniority + archetype).
5. **Claude ships the resume** in that template as **both `.docx` (to edit) and `.pdf` (to send)**, then runs an ATS + quality checklist.

### Things to try
- *"Rebuild my resume in the Executive Serif template."*
- *"I'm a Growth PM — recommend a template and quantify my bullets."*
- *"Tailor my PM resume to this job description:"* (paste the JD)
- *"Review my PM resume against best practices."*

### Choosing a template quickly
| You are… | Template |
|---|---|
| Senior / Lead / Director / Head / CPO, or ex-founder | **01 Executive Serif** |
| Mid-level PM, modern company | **02 Modern Minimal** |
| Growth / Data PM | **03 Growth / Metrics** |
| AI / ML PM | **04 AI Product** |
| APM / early-career / switcher | **05 Associate One-Pager** |

See the previews in [`templates/`](../templates/).

---

## Notes & good practice

- **Nothing is fabricated.** If a metric is unknown, Claude asks for it or uses an honest scale statement. Everything on the resume must survive an interview.
- **Both files, every time.** You always get a `.docx` for future edits and a text-based `.pdf` for applications, verified to be ATS-parseable.
- **One page under ~5 years, two pages beyond.** Older roles get fewer bullets.
