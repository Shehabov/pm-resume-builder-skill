# PM Resume Structure & Format

**Sources:** Harvard Career Services, IGotAnOffer, Exponent, HustleBadger, The Tech Resume Inside Out (ATS), Tech Interview Handbook (FAANG section order and formatting), r/EngineeringResumes (formatting mechanics).

PMs are screened on scope and outcomes, so the structure differs from an engineering resume in three ways: **keep a strong summary, put Experience first (not Skills), and lead each role with a company-context line.**

---

## Section order

### Experienced PM (3+ years), the default
```
1. Name  (centered, bold)
2. Title line  (e.g., "Senior Product Manager")  + location + contact line
3. SUMMARY            (3-5 lines, PM-specific)
4. EXPERIENCE         (reverse chronological, with company-context lines)
5. SKILLS             (compact, optional, tools + PM competencies)
6. EDUCATION          (abbreviated)
7. CERTIFICATIONS     (PM-relevant: Reforge, Product School, PMI-ACP, CSPO…)
8. AWARDS             (optional)
```

### Early-career / APM (0-3 years)
```
1. Name + Title + contact
2. SUMMARY            (2-3 lines)
3. EXPERIENCE         (internships/PM-adjacent, clearly labeled)
4. PROJECTS           (product case studies, side products, high value early on)
5. SKILLS
6. EDUCATION          (higher up; include if strong)
```

**Why Experience first (not Skills):** PMs are hired on what they shipped and the outcomes, not a tool list. Skills is a supporting, compact section, never the headline.

**Why keep the Summary:** unlike engineering resumes (which often skip it), PM resumes should carry a 3-5 line summary. It is where the recruiter reads years of experience, scope, and your signature outcome in the first 2 seconds.

---

## The Summary (PM-specific)

3-5 lines. Lead with **years of PM experience + leadership scope**, then your **signature quantified outcome**, then your **specialisation/archetype**, then the **role you are targeting**. No pronouns, no fluff.

> Senior Product Manager and ex-founder with 6 years building and scaling million-dollar B2B and B2C products. Launched consumer products used by 13M+ people and B2B AI platforms serving tens of thousands of businesses. Specialises in AI product development, discovery, and growth, turning ambiguous problems into focused roadmaps and shipped outcomes.

Avoid: "results-driven product manager passionate about building great products" (says nothing, uses banned filler).

---

## Contact line

Single line, centered, separated by pipes:
```
website.com  |  +CC (xxx) xxx xx xx  |  name@gmail.com  |  LinkedIn Name  |  github-handle
```
- Professional email (Gmail/Outlook).
- LinkedIn is expected for PMs (unlike the engineering-wiki opinion), include it.
- City/country is fine for PMs (relocation/timezone signals matter for product roles).
- Links are plain text, black, still clickable. No "Email:" / "LinkedIn:" prefixes, no https://www.
- No photo, no age, no marital status (US/UK/most markets).

---

## Experience block format

```
COMPANY, City, Country                                            Right-aligned
Job Title                                                          Dates (hyphen with spaces)
Company/product context in one line: what it is, its scale, what you owned.
• Outcome bullet (strategy/ownership) with a number
• Outcome bullet (execution) with a number
• …  (5-7 for the two most recent roles, 3-5 for older)
```

- **Company context line** is mandatory (see the flagship example). One line, sets stakes.
- Reverse chronological.
- Dates: a hyphen with spaces, "Present" for current, month + full year ("Aug 2024 - Present"). Right-aligned. Bullets do not extend past the dates.
- Group short advisory/mentorship/founder roles into their own section if they clutter the main timeline.

---

## Page layout & ATS mechanics

- **Single column.** No sidebars, text boxes, tables-for-layout, icons, photos, or progress bars, these break ATS parsing and waste the recruiter's scan.
- **Fonts (all ATS-safe):**
  - *Executive/serif templates:* Garamond or EB Garamond (name 18-20pt, headings 12-13pt, body 10.5-11pt).
  - *Modern/sans templates:* Calibri or Arial (name 16-18pt, headings 11.5-12pt, body 10.5pt).
  - Body never below **10.5pt**.
- **Margins:** 0.5-0.75 in. **Line spacing:** ~1.1-1.15.
- **Section headings:** bold, standard names, with a thin bottom rule. Names must be exactly: `Summary`, `Experience`, `Skills`, `Education`, `Certifications`, `Awards`, `Projects`.
- **Length:** 1 page under ~5 years; up to 2 pages beyond. Page 2 at least half full or condense to 1.
- **No headers/footers** for key content (some ATS skip them). Put everything in the body.

---

## Skills section for PMs (keep it tight)

Group into 2-4 labeled lines. Include the things a PM is actually screened on, not a laundry list:
- **Product:** discovery, roadmapping, prioritization (RICE/OKRs), product strategy, PLG, experimentation, GTM
- **Data & tools:** SQL, Amplitude/Mixpanel, A/B testing, Jira/Linear, Figma, Metabase
- **AI (if relevant):** LLMs, evals, RAG, prompt design
Do not include soft skills ("great communicator") or obvious tools (MS Office). Only list what you can defend in an interview and back with a bullet.

---

## Export & verification (mandatory)

Build the `.docx` with the `docx` skill, then:
```bash
soffice --headless --convert-to pdf resume.docx     # exact-format PDF
pdftotext resume.pdf -                               # must return real text (ATS-parseable)
pdfinfo resume.pdf                                   # confirm page count
```
Confirm the name, titles, and key metrics appear in the extracted text (catches truncation/encoding). Deliver **both** `.docx` and `.pdf`. A clean 1-2 page text PDF should be well under ~250KB.
