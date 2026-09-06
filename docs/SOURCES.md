# Sources & Research

Every source consulted to build this skill, and where each insight is applied. This skill was tailored for product managers on top of a general resume-builder foundation, so it carries both the foundational resume sources and new PM-specific research.

---

## 1. Product-manager-specific sources (new for this skill)

| Source | What was extracted |
|---|---|
| [IGotAnOffer — Product Manager Resume (13 FAANG examples)](https://igotanoffer.com/blogs/product-manager/product-manager-resume) | PM section order, the "40 PM resume keywords" bank, outcome-over-duty bullets, metric expectations, one-page-per-decade guidance, real Google/Meta/Amazon examples |
| [Exponent — How to Write the Perfect Product Manager Resume (2026)](https://www.tryexponent.com/blog/how-to-write-the-perfect-product-manager-resume) | Section order by seniority, the "skill: accomplishment" bullet formula, metric-to-archetype matching (Growth/Platform/Monetization/AI), 3-5 line summary structure, 2026 signals (metrics ownership + AI product work), keyword-by-role bank |
| [HustleBadger — Write a PM Resume](https://www.hustlebadger.com/what-do-product-teams-do/write-a-pm-resume/) | TAR/CAR bullet structure, "impact not process", why "worked cross-functionally" is not an achievement, 6-8 second recruiter scan, PM-specific quantification |
| Reforge (PLG, Growth, Product Strategy programs) | Growth-metric vocabulary (activation, retention, funnel, PLG loops), how growth PMs frame impact |
| Amplitude / Mixpanel product-analytics conventions | Standard metric definitions (DAU/MAU, D1/D7/D30 retention, cohort analysis) used in `pm-metrics-and-impact.md` |
| Lenny Rachitsky & Shreyas Doshi (product-thinking principles) | Strategy vs execution vs impact framing; product sense signals recruiters read for |

---

## 2. Foundational resume sources (carried over and adapted for PMs)

| Source | What was extracted |
|---|---|
| [Harvard Career Services — Create a Strong Resume](https://careerservices.fas.harvard.edu/resources/create-a-strong-resume/) | Language principles (specific, active, fact-based, scannable), top-5 mistakes, action-verb tables, do/don't list |
| [r/EngineeringResumes wiki](https://www.reddit.com/r/EngineeringResumes/wiki/index/) | Formatting mechanics: single column, dates/en-dashes, "Present", no periods on bullets, digits not words, plain-text URLs, ATS-safe fonts |
| [The Tech Resume Inside Out — ATS Myths Busted & Hiring Pipeline](https://thetechresume.com/samples/ats-myths-busted) | ATS is a human workflow tool (not an auto-rejecting robot), the fabricated "75%" stat, PDF is fine, tailor for humans |
| [Google XYZ formula](https://www.inc.com/bill-murphy-jr/google-recruiters-say-using-this-6-second-trick-doubled-their-number-of-quality-interviews.html) | "Accomplished [X] as measured by [Y] by doing [Z]" — adapted into the PM bullet formula |
| [Columbia University — STAR bullet points](https://www.careereducation.columbia.edu/resources/resumes-impact-creating-strong-bullet-points) | Situation-Task-Action-Result condensed bullets |
| [Lever — ATS Myths Debunked](https://www.lever.co/blog/applicant-tracking-system-myths/) | How recruiters actually use the ATS; no "gaming" it |

---

## 3. Source-to-file mapping

| Skill file | Primary sources |
|---|---|
| `SKILL.md` | Exponent (flow + archetypes), HustleBadger (impact-not-process), IGotAnOffer, Harvard |
| `references/pm-bullet-writing.md` | Exponent, HustleBadger, IGotAnOffer, Google XYZ, Columbia STAR, Harvard verbs |
| `references/pm-metrics-and-impact.md` | Exponent (metric-to-role), Reforge, Amplitude/Mixpanel, Lenny |
| `references/pm-resume-structure.md` | IGotAnOffer, Exponent, Harvard, r/EngineeringResumes (mechanics), Tech Resume (ATS) |
| `references/ats-and-keywords.md` | Tech Resume Inside Out, Exponent, IGotAnOffer keyword bank, Lever |
| `references/common-mistakes.md` | IGotAnOffer, Exponent, HustleBadger, Harvard top-5 |
| `references/pm-templates.md` | Synthesis + the flagship real example (`examples/`) |

---

## 4. Key adaptations from the general resume standard to PM

| Topic | General/engineering standard | PM adaptation in this skill |
|---|---|---|
| Summary | Often skipped | **Kept** — PMs are read on years + scope + signature outcome first |
| First section | Skills first (for engineers) | **Experience first** — PMs hired on shipped outcomes, Skills is compact/supporting |
| Metrics | Technical (latency, throughput) | **Product metrics** by archetype (activation, retention, revenue, adoption, AI evals) |
| "Cross-functional" | Fine to mention | **Flagged** — it is the core job, never an achievement on its own |
| Domain context | Industry/system type | **Company-context line** per role (scale, what you owned) — the PM differentiator |
| Bullet formula | XYZ (measured by Y) | **TAR / skill:accomplishment**, metric pushed to the front |
