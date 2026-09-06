# PM Resume Templates (5 supported, all ATS-guaranteed)

Every template here is **single-column, standard-font, text-based, and free of tables-for-layout, icons, and graphics**, so it parses cleanly in Greenhouse, Workday, Lever, Ashby, iCIMS, and Taleo. "ATS-guaranteed" means the exported PDF returns clean, ordered text via `pdftotext` (the skill verifies this on export).

Previews live in `templates/<id>/preview.png`. Each template folder also has a `spec.md` with exact fonts, sizes, and spacing for the `docx` build.

When the user picks a template (by number, name, or trigger phrase), load that folder's `spec.md` and build to it.

---

## 01 · Executive Serif  🎩
**Best for:** Senior / Lead / Group PM, Director / Head of Product, CPO. Also great for ex-founders and consultants.
**Look:** Classic Garamond serif, centered name + title, thin-rule section headings, company-context line under every role, dedicated Certifications & Awards. The most "senior and credible" of the set. This is the style of the flagship example (`examples/Shehab-Beram-Senior-PM-Resume.pdf`).
**Sections:** Summary · Experience (with context lines) · Advisory & Mentorship (optional) · Education · Certifications · Awards
**Font:** EB Garamond / Garamond, name 18-20pt, headings 12-13pt, body 10.5-11pt.
**Trigger:** *"Build my PM resume in the Executive Serif template"* · *"use template 1"* · *"make it like the senior PM example"*

## 02 · Modern Minimal  ▤
**Best for:** Mid-level Product Manager at a modern tech/SaaS company; the safe default for most PMs.
**Look:** Clean Calibri/Arial sans, compact heading rules, generous whitespace, no summary bloat. Reads fast and neutral.
**Sections:** Summary · Experience · Skills · Education · Certifications (optional)
**Font:** Calibri or Arial, name 16-18pt, headings 11.5-12pt, body 10.5pt.
**Trigger:** *"Modern Minimal template"* · *"use template 2"* · *"clean modern PM resume"*

## 03 · Growth / Metrics-Forward  📈
**Best for:** Growth PM, Data PM, or any PM whose story is fundamentally about moving numbers.
**Look:** Modern sans with a **"Selected Impact"** strip near the top, 3-5 headline metrics (e.g., "activation +18% · $4M revenue · 6M users") as a scannable band, then metric-led bullets throughout.
**Sections:** Summary · Selected Impact · Experience · Skills (data/experimentation first) · Education
**Font:** Calibri/Arial. Impact strip in bold, one line, no graphics (plain text, ATS-safe).
**Trigger:** *"Growth Metrics template"* · *"use template 3"* · *"metrics-forward PM resume"*

## 04 · AI Product Manager  🤖
**Best for:** AI / ML Product Manager, or a PM targeting AI-native companies.
**Look:** Modern sans with an **"AI Product Highlights"** line and bullets that foreground evals, quality/latency/cost tradeoffs, and shipped AI features. Skills lead with the AI stack (LLMs, RAG, evals).
**Sections:** Summary · AI Product Highlights · Experience · Skills (AI + data first) · Education · Certifications
**Font:** Calibri/Arial.
**Trigger:** *"AI Product template"* · *"use template 4"* · *"AI PM resume"*

## 05 · Associate One-Pager  🌱
**Best for:** APM / Associate PM / aspiring PM / career-switcher, strictly one page.
**Look:** Compact sans, Education kept near the top, a **Projects** section (product case studies / side products) that carries weight when work history is thin. Every line earns its place.
**Sections:** Summary (2-3 lines) · Experience · Projects · Skills · Education
**Font:** Calibri/Arial, tuned to fit one page cleanly.
**Trigger:** *"Associate one-pager"* · *"use template 5"* · *"entry-level / APM PM resume"*

---

## How to trigger a template (for the user)

Say any of the following to Claude once the skill is active:

- *"Rebuild my resume using the **Executive Serif** template"* (or template 1-5 by number)
- *"I'm a Growth PM, use the right template"*, Claude recommends **03**
- *"I'm applying for an AI PM role at an early-stage startup"*, Claude recommends **04**
- *"Not sure which, recommend one"*, Claude picks by seniority + archetype and explains why

## How Claude chooses when the user is unsure

| Situation | Recommend |
|---|---|
| Senior / Lead / Director / Head / CPO, or ex-founder | 01 Executive Serif |
| Mid-level PM, modern company, no strong angle | 02 Modern Minimal |
| Story is about growth/retention/conversion numbers | 03 Growth / Metrics |
| AI/ML product role | 04 AI Product |
| APM / <3 years / career switch | 05 Associate One-Pager |
