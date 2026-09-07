---
name: pm-resume-builder
description: "Use this skill whenever the user wants to create, improve, rewrite, review, tailor, or ATS-optimize a PRODUCT MANAGER resume or CV. Triggers include any mention of 'PM resume', 'product manager resume', 'product resume', 'PM CV', 'product management CV', plain-language asks like 'create my resume', 'build my CV', 'optimize my resume', 'improve my CV', 'review my resume', 'make it ATS-friendly', 'tailor my resume to this job description', 'help me get hired', and the Spanish terms 'hoja de vida' or 'curriculum vitae', or a request to turn product/PM experience into a resume, quantify product impact, write PM bullet points, add product metrics (activation, retention, revenue, adoption), tailor a PM resume to a job description, pick a PM resume template, or prepare a resume for an APM / PM / Senior PM / Lead PM / Group PM / Director of Product / Head of Product / CPO application. Also use for AI Product Manager, Growth PM, Platform/Technical PM, and Product Owner resumes. Do NOT use for engineering-only resumes, LinkedIn profile rewrites, portfolios, or cover letters unless the resume is the main deliverable."
---

# Product Manager Resume Builder, Recruiter-Grade, ATS-Guaranteed

## What this skill does

Turns a product manager's messy history into a sharp, recruiter-grade, ATS-safe resume. It is tuned for how PMs are actually screened: a recruiter spends 6-8 seconds on the first pass and looks for **years of PM experience, scope owned, and quantified product outcomes** (activation, retention, revenue, adoption, launches). Every choice here optimizes for that scan and for clean ATS parsing.

**Before doing any resume work, read the reference files you need:**
- `references/pm-resume-structure.md`, sections, order, layout, fonts, PDF export
- `references/pm-bullet-writing.md`, the PM bullet formula, action verbs, before/after
- `references/pm-metrics-and-impact.md`, which metrics to show per PM archetype
- `references/pm-templates.md`, the 5 supported templates + how to trigger each
- `references/ats-and-keywords.md`, ATS reality, PM keyword bank, tailoring
- `references/common-mistakes.md`, the PM-specific traps to avoid
- `references/qa-review-agents.md`, the two mandatory QA passes (FAANG Recruiter, Head of Product) to run before delivery

Then use the **`docx` skill** to produce the file, and always deliver **both `.docx` and `.pdf`**.

---

## The flow (default: rebuild from an existing CV)

This is the primary path the user expects: *take my old CV, ask me questions, ship the perfect one in the template I choose.*

### Step 0, Read their current CV
If the user attaches or points to an existing resume, **read it fully first** (PDF/DOCX/text). Extract: roles, companies, dates, scope, any numbers, education, certs. Do not start asking questions until you have read what they already have. If they have no CV, skip to Step 2 and gather from scratch.

**If an MCP is connected, use it for inputs.** When the user has a Google Drive, filesystem, Gmail, Notion, or web/fetch MCP available, read the source directly instead of asking for an upload: pull the CV from Drive or a local path, read a job description from a Gmail thread or a posting URL, or pull role context from Notion. Only fall back to asking the user to paste or attach when no MCP can reach the source.

### Step 1, Diagnose (say what is weak, briefly)
In 3-6 lines, tell them what is holding the current resume back, using this skill's standards: missing metrics, vague "responsible for" bullets, "worked cross-functionally" filler, no scope/context per role, wrong section order, over-length, weak summary. Be specific and kind. This earns trust and sets up the questions.

### Step 2, Ask targeted questions (only what you actually need)
Ask in one batched, numbered list. Prioritise the gaps that will move the resume most. Cover:

1. **Target role + seniority**, APM / PM / Senior / Lead / Group / Director / Head / CPO, and the kind of company (B2B SaaS, consumer, marketplace, fintech, AI, etc.).
2. **PM archetype**, Growth, Core/Feature, Platform/Technical, AI/ML, Monetization, 0 to 1, or generalist. This decides which metrics to feature (see `pm-metrics-and-impact.md`).
3. **Template choice**, show the 5 templates from `pm-templates.md` and let them pick (or recommend one for their seniority/archetype).
4. **Scope per role**, for each role: what did you own (surface, product line, teams), how big was the team you worked with, who were the users (B2B/B2C, how many), and the business context of the company.
5. **The numbers**, this is where most PM resumes fail. For each headline achievement, get: the metric that moved, by how much, over what baseline/time, and the business result ($ revenue, retention, adoption, activation, NPS, time-to-market). If they do not have exact numbers, get honest estimates or scale indicators ("~", "tens of thousands of users", "3 core product lines").
6. **Length + market**, 1 page (<5 yrs) or 2 pages (5+ yrs); US/global English by default.
7. **Certs / awards / education**, especially PM-relevant (Reforge, Product School, PMI-ACP, CSPO, etc.).

**Do not fabricate metrics.** If a number is unknown, ask, or use an honest qualitative scope statement. Everything on the resume must survive an interview.

### Step 3, Choose the template
Confirm the template. Map it to the layout spec in `references/pm-templates.md`. If unsure, recommend:
- **Senior/Lead/Director/Head**, `01-executive-serif`
- **Mid-level PM, modern company**, `02-modern-minimal`
- **Growth/Data PM**, `03-growth-metrics`
- **AI/ML PM**, `04-ai-product`
- **APM/Associate/early-career**, `05-associate-onepager`

### Step 4, Write the content
Follow `references/pm-bullet-writing.md`. Core rules:
- **Every bullet is an outcome, not a duty.** Lead with the result or the action, never with "Responsible for" or "Worked on".
- **PM bullet formula:** `Action verb + what you shipped/owned + for whom (scope/domain) + the measurable result`. Push the metric toward the front when you have one.
- **Show the arc: strategy, execution, impact.** Senior resumes lead with strategy/ownership bullets; early-career lead with shipped features and data.
- **Cross-functional is table stakes**, never write "worked cross-functionally" as an achievement. Instead: *what* you drove *with whom* to *what result* ("aligned eng, design, and 3 CSM teams to cut setup time from 40 to under 10 minutes").
- **Quantify like a PM:** revenue, ARR, GMV, activation, retention, DAU/MAU, adoption, conversion, CAC/LTV, NPS, time-to-market, cost saved, users reached. Use digits (18%, $600K, 14M).
- **Company context line** under each role (1 line): what the company/product is, its scale, and what you owned. This is the PM version of "domain context" and it is the single biggest differentiator (see the flagship example).
- **Summary (include it for PMs):** 3-5 lines. Lead with years of PM experience + years of leadership, signature outcome, archetype/specialisation, and the role targeted. Unlike engineering resumes, PM resumes should keep a strong summary.

### Step 5, Format in the chosen template
Follow `references/pm-resume-structure.md` and the specific template spec. Build with the `docx` skill. Single column, ATS-safe font, no tables-for-layout, no icons/graphics, standard section names, right-aligned dates with a hyphen.

### Step 6, Run the two QA agents (mandatory)
Before exporting, put the draft through two strict review passes from `references/qa-review-agents.md`. Adopt each persona fully and give the user both reports in plain language.

1. **The FAANG Recruiter** grades it like a real screen: outcome bullets, metrics with a baseline, ATS mechanics, archetype match, no fabrication, and the sameness trap (near-identical bullets, or content so generic it could belong to any PM). Verdict: SCREEN or PASS, plus the fixes that flip it.
2. **The Head of Product** reads it as a career story: throughline, growing scope, arc within roles, and any gaps, date overlaps, or discrepancies between the summary's promise and the experience.

Apply every fix that needs no new fact. For anything that needs a number, a date, or a decision only the user knows, **ask, do not invent.** When two bullets say the same thing, or a story has a hole, surface it to the user rather than shipping it quietly. Re-run the affected checklist items after edits.

### Step 7, Export PDF + verify (mandatory)
Deliver **both** `.docx` (to edit) and `.pdf` (to send).
- Convert via LibreOffice: `soffice --headless --convert-to pdf resume.docx`
- **Verify it is text-based / ATS-parseable:** `pdftotext resume.pdf -` and confirm the name, titles, and metrics come out as real text.
- Check page count with `pdfinfo` and that nothing truncates.
- Run the **delivery checklist** below.
- **If an MCP is connected, deliver where the user keeps their files.** Save both `.docx` and `.pdf` back to the Google Drive folder or local path they name, or draft a Gmail reply with the resume ready to attach. Ask before sending anything or writing outside the location they asked for.

---

## PM Quick Decision Framework

| User asks | Do this |
|---|---|
| "Rebuild my PM resume from my old one" | The full flow above (read, diagnose, ask, template, write, export) |
| "Make my PM resume from scratch" | Skip Step 0, gather in Step 2, then build |
| "Tailor my PM resume to this JD" | Extract the JD's outcomes + keywords, map to their experience, reorder bullets and summary, do not invent |
| "Review my PM resume" | Run both QA agents (`qa-review-agents.md`) plus the delivery checklist, give specific rewrites and flag story gaps |
| "Is my resume too generic / will it stand out?" | Run the FAANG Recruiter pass and the sameness-trap checks (`common-mistakes.md`, `ats-and-keywords.md`), differentiate on specifics |
| "Quantify my bullets" | For each bullet, ask for metric + baseline + result, apply the PM formula |
| "Which template should I use?" | Recommend by seniority/archetype from `pm-templates.md` |
| "Make it ATS-friendly" | Enforce single column, standard headings, text-based PDF, JD keyword mirroring |

---

## Delivery checklist (run before handing over)

**First-scan (6-8 seconds):**
- [ ] Current title + seniority obvious at the top
- [ ] Years of PM experience + leadership scope visible in the summary
- [ ] Top of page 1 carries the strongest quantified outcome

**Content:**
- [ ] Every bullet is an outcome; none start with "Responsible for" / "Worked on" / "Helped"
- [ ] No "worked cross-functionally" as a standalone achievement
- [ ] Metrics use digits and show baseline/scale ($600K, 18%, 14M users, 40 to 10 min)
- [ ] Each role has a 1-line company/scope context
- [ ] Summary is 3-5 lines, PM-specific, targeted at the role
- [ ] Bullets: 5-7 for the two most recent roles, 3-5 for older
- [ ] No personal pronouns; no periods ending bullets; past tense for past roles
- [ ] Archetype metrics match the target role (growth vs platform vs AI, see reference)
- [ ] No buzzwords without substance (synergy, results-driven, ninja, guru)

**Format / ATS:**
- [ ] Single column, no tables-for-layout, no icons/graphics/photos
- [ ] ATS-safe font (Garamond/Calibri/Arial), body ≥ 10.5pt, name ≤ 18pt
- [ ] Standard section names (Summary, Experience, Education, Skills, Certifications)
- [ ] Dates right-aligned with a hyphen, "Present" for current
- [ ] 1 page (<5 yrs) or 2 pages (5+ yrs); page 2 at least half full
- [ ] Links are plain text, black, clickable

**QA agents (both passes run and reported):**
- [ ] FAANG Recruiter verdict is SCREEN, or the remaining PASS reasons are surfaced to the user
- [ ] No two bullets make the same point; near-duplicates merged or split by metric, scope, or decision
- [ ] Nothing reads generic enough to belong to any PM (the sameness trap)
- [ ] Head of Product throughline is clear, scope rises over time
- [ ] Story gaps, date overlaps, and summary-vs-experience discrepancies flagged to the user, none invented away

**Delivery:**
- [ ] PDF generated and verified text-based with `pdftotext`
- [ ] Page count correct, nothing truncated
- [ ] Both `.docx` and `.pdf` delivered
