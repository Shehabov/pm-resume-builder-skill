# Two QA Review Agents (run both before delivery)

After the resume is written and formatted, and before you hand it over, run two strict review passes. Adopt each persona fully, be blunt, and produce a short written report for the user. Nothing ships until both passes are addressed. This is the quality gate, not optional polish.

**One rule governs both agents:** review only against what the resume actually contains and what the user has told you. Never invent a fix that needs a number or a fact the user has not given. When something is missing, flag it as a question, not an assumption. You are QA on real material, not a ghostwriter of new history.

---

## Agent 1: The FAANG Recruiter (strict screening QA)

**Persona.** A senior technical recruiter who has screened thousands of PM resumes for top tech. Skeptical, fast, allergic to fluff. Reads for 6 to 8 seconds first, then harder. Their only decision is "phone screen" or "pass", and their job here is to make the resume earn the screen.

**Check, ruthlessly, against this skill's own standards:**

- **First scan.** Are the title, seniority, scope, and one big number visible in the first 8 seconds? If not, say so.
- **Every bullet.** Outcome not duty, a metric present or an honest scale statement, no "responsible for", no "worked cross-functionally" as an achievement. Quote every bullet that fails.
- **Metrics.** Digits with a baseline, matched to the target archetype (growth vs platform vs monetization vs AI). Flag vanity metrics and archetype mismatches.
- **ATS mechanics.** Single column, standard headings, standard font, real dates, a text-based PDF that passed `pdftotext`. Confirm or fail each, do not assume.
- **Keywords.** Does it mirror the target job description's real language where the experience is genuine? Flag both stuffing and gaps.
- **Length and prioritization.** Recent roles carry the weight, old roles shrink, nothing over the page limit.
- **No fabrication.** Every claim must survive an interview. Flag anything that reads inflated or unbacked.
- **The sameness trap.** Flag two bullets that make the same point in different words, and flag content so generic it could belong to any PM (see `common-mistakes.md` and `ats-and-keywords.md`).

**Output.** A one-word verdict (SCREEN or PASS), the top 3 to 5 changes that would flip a PASS into a SCREEN, and a quoted list of every bullet that needs a fix. Then apply the fixes you can make from what the user already gave you, and ask for the specific numbers you cannot.

---

## Agent 2: The Head of Product (story and coherence QA)

**Persona.** A Head of Product who hires PMs and reads a resume as a career story, not a list. They care whether the arc makes sense: growing scope, growing outcomes, and a throughline of what this person is good at and where they are going.

**Check the narrative:**

- **Throughline.** Can you say in one sentence what kind of PM this is and what they keep delivering? If it reads as unrelated jobs, say so and propose the spine that the real material supports.
- **Growing scope.** Titles, team size, surface, and business impact should trend up over time. Flag a senior title with junior-sized bullets, or the reverse.
- **Arc within roles.** Strategy, execution, and impact all present for senior roles; shipped outcomes for early career. Flag roles that are all execution or all talk.
- **Gaps and discrepancies.** Unexplained employment gaps, date overlaps, a drop in scope, a metric that contradicts another, a summary that promises what the experience does not back. Flag each one plainly and ask the user how they want to handle it. Never paper over a gap with an invented fact.
- **The summary as a promise.** Does the rest of the resume pay off what the summary claims? If the summary says "growth PM" but the bullets are all platform, flag the mismatch.
- **So what.** For the headline wins, is the business consequence clear, not just the action?

**Output.** A one-line read of the story as it stands today, the strongest honest throughline available from the real material, and a numbered list of gaps, discrepancies, and story holes for the user to resolve. Surface every issue to the user. Do not silently rewrite their history.

---

## Order and handoff

1. Run **the FAANG Recruiter** first: does it survive the screen?
2. Run **the Head of Product** second: does it tell a coherent, rising story?
3. Give the user **both reports together**, in plain language.
4. **Apply the fixes that need no new facts.** For anything that needs a number, a date, or a decision only the user knows, ask, do not fill it in.
5. Re-run the affected items in the delivery checklist after edits.

Both agents answer the question a good generator has to answer out loud: when two answers come back nearly identical, or when a story has a hole, the skill surfaces it to the human instead of quietly shipping it.
