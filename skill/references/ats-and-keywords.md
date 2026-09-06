# ATS & PM Keyword Bank

**Sources:** The Tech Resume Inside Out (ATS myths and the hiring pipeline), Tech Interview Handbook (FAANG and ATS friendly formatting), r/EngineeringResumes (community tested mechanics), Exponent, IGotAnOffer ("40 PM resume keywords"), Lever.

---

## ATS reality (do not over-optimise for a robot)

An ATS is a **database + workflow tool** for recruiters, not an AI gatekeeper. Most systems do **not** auto-reject on a score. The steep dropoff is a **human** spending 6-8 seconds, not a robot. So the priorities are, in order:

1. **Be parseable**, single column, standard headings, text-based PDF/DOCX, no tables-for-layout, no images.
2. **Be scannable by a human**, title, seniority, scope, and a big number visible instantly.
3. **Mirror the JD's language**, use the exact terms the job description uses *when you genuinely have that experience*.

**Myths to ignore:** "PDFs break ATS" (false for all modern ATS), "you need X% keyword density" (false), "white-text keywords" (never, it gets flagged), "75% auto-rejected by bots" (a fabricated stat from vendors). Standard, clean formatting wins.

**FAANG and big-tech formatting rules** (Tech Interview Handbook, r/EngineeringResumes), which the templates already follow:

- One column only. Two-column layouts scramble in the parser and bury the right-hand column.
- Standard section headings a parser expects: Summary, Experience, Skills, Education. No clever renames.
- Reverse chronological order, most recent role first, with clear "Present" on the current role.
- Real dates on the right (Mon YYYY), consistent format across every role.
- No text inside headers, footers, images, or text boxes, parsers routinely drop those regions.
- Standard fonts, plain bullet characters, digits not spelled-out numbers, plain-text URLs.
- Export a text-based PDF and confirm it with `pdftotext`, if the text comes back clean and ordered, the ATS reads it the same way.

---

## PM keyword bank (use the ones that are true for you)

**Universal PM (most roles):**
product strategy, product roadmap, product lifecycle, product discovery, prioritization, OKRs, KPIs, success metrics, North Star metric, stakeholder management, cross-functional leadership, go-to-market (GTM), user research, customer interviews, A/B testing, experimentation, data-driven decisions, backlog, requirements (PRDs), MVP, product-market fit, agile/scrum

**Growth PM:**
activation, retention, churn, conversion, funnel analysis, cohort analysis, CAC, LTV, LTV/CAC, PLG (product-led growth), onboarding, lifecycle marketing, growth loops, SQL, Amplitude, Mixpanel, referral

**Platform / Technical PM:**
APIs, SDKs, platform, developer experience, latency, uptime/SLA, scalability, system design, data pipelines, infrastructure, integrations, technical tradeoffs

**Monetization PM:**
pricing, packaging, ARPU, ARR/MRR, expansion revenue, upsell, billing, paywall, gross margin, monetization experiments

**AI / ML PM:**
LLMs, RAG, agents/agentic, model evaluations (evals), prompt engineering, embeddings, vector databases, fine-tuning, hallucination rate, latency/cost/quality tradeoffs, human-in-the-loop, guardrails, AI product strategy

**B2B / Enterprise PM:**
enterprise, SaaS, B2B, onboarding, admin/permissions, SSO, compliance, SLAs, customer success, seat expansion, sales enablement, RFPs

**Tools (only if used):** Jira, Linear, Productboard, Figma, Miro, Amplitude, Mixpanel, Metabase, Looker, GA4, Notion, Confluence, Pendo, Optimizely, LaunchDarkly, dbt

**Do not** list soft skills as keywords ("team player", "detail-oriented") or tools you cannot discuss.

---

## Tailoring a PM resume to a job description

1. **Extract the JD's outcomes + language:** what the role owns, the metrics it cares about (growth? platform? monetization?), the seniority signals (strategy, mentoring, 0 to 1), and the exact tool/keyword phrasing.
2. **Map to your experience:** for each JD priority, find your matching bullet. If it is true but missing, add it.
3. **Reorder, don't fabricate:** move the most relevant bullets to the top of each role, retune the summary's targeted role and lead metric, and adjust the Skills lead line. Never add experience you do not have, you will be asked about everything in the interview.
4. **Match the metric family** to the role (see `pm-metrics-and-impact.md`).
