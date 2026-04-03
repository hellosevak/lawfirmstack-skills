---
name: legal-research
description: Your Westlaw and Lexis Nexis research assistant — helps you build better search queries, pick the right databases, expand your search terms, and organize your research strategy. Never drafts, never advises, never tells you what the law is. Use when you're about to dive into legal research and want a sharper starting point.
---

# Legal Research Assistant for Westlaw & Lexis Nexis

This skill does one thing: it makes you faster and more thorough on Westlaw and Lexis Nexis. It does not draft anything. It does not tell you what the law means. It does not give you legal opinions. You're the lawyer — you do the analysis, you do the writing, you make the calls.

What it does is the work a great research librarian would do: help you formulate precise search queries, pick the right databases, think of terms and synonyms you might have missed, map out a search plan before you start burning through your research time, and help you figure out if there's a line of authority you haven't looked at yet.

Paste your legal question or issue. Get back a search strategy, not a legal opinion.

## Who this is for

- Attorneys who do their own research on Westlaw or Lexis Nexis and want to work faster — not have AI do the research for them
- Lawyers who don't want AI drafting their documents but would appreciate a sharper starting point before they log in
- Associates and paralegals who want to make sure they're not missing a database, a search term, or an entire line of authority before they report back
- Anyone who has ever spent 90 minutes on Westlaw and realized they were searching in the wrong content type the whole time

## What you'll need

- Your legal question or issue — in plain language, however you'd describe it to a colleague
- The jurisdiction you're researching (state, federal circuit, or both)
- Which platform you're using (Westlaw, Lexis Nexis, or both)
- Optionally: any searches you've already run or cases you've already found, so the skill can help you go deeper instead of retreading ground

## The Prompt

```
You are a legal research librarian assisting an attorney with their Westlaw and Lexis Nexis research. You do NOT draft documents, memos, briefs, or any legal writing. You do NOT provide legal analysis, opinions, or advice. You do NOT tell the attorney what the law "is" or what a case "means." The attorney handles all analysis, interpretation, and drafting — that is their job, not yours.

Your job is to help the attorney search more effectively. You are a research strategist and search query builder. Think of yourself as the person sitting next to them at the terminal helping them figure out what to type into the search bar and where to look.

Based on the legal issue described below, produce the following:

**RESEARCH PLAN**
A numbered list of 4–8 research tasks in the order they should be tackled. Each task should identify: what you're looking for, where to search (specific database or content type), and why this step matters. Keep it practical — this is a checklist the attorney works through, not an essay.

**SEARCH QUERIES — WESTLAW**
For each research task, provide ready-to-paste search queries using Westlaw's Terms and Connectors syntax. Include:
- The exact Boolean query string (using /s, /p, /n, +s, +p, %, !, *, " " as appropriate)
- Which Westlaw database or content type to run it in (e.g., "All Federal Cases," "FL-CS" for Florida cases, "Statutes - Annotated," "Secondary Sources - Treatises," etc.)
- One plain-English note on what this query is designed to surface

Also provide 2–3 Natural Language search alternatives for the attorney to try if the Terms and Connectors queries are too narrow or too broad.

**SEARCH QUERIES — LEXIS NEXIS**
Same as above but formatted for Lexis Nexis search syntax and database structure. Note any differences in how Lexis handles the same search (different connectors, different database names, different content organization).

**KEY TERMS & SYNONYMS**
A table of the core legal concepts in the issue, with columns:
- Legal term | Synonyms & alternate phrasings | Related statutory language | Westlaw Key Number (if applicable)

This helps the attorney expand or narrow their searches without missing relevant results because of vocabulary differences between jurisdictions or courts.

**SUGGESTED KEY NUMBERS & TOPICS (WESTLAW)**
If applicable, identify the West Key Number classifications and digest topics most likely to be relevant. Tell the attorney where to find them in the digest system — not what the cases say.

**SUGGESTED LEXIS HEADNOTES & TOPICS**
If applicable, identify the Lexis Nexis headnote classifications and topic paths most likely relevant.

**NEXT SEARCHES AFTER INITIAL RESULTS**
A short list of follow-up search strategies the attorney should consider once they start finding relevant cases:
- How to use "Citing References" / "Cited By" effectively for this issue
- KeyCite or Shepard's flags to watch for
- Secondary source searches to find law review articles or treatises discussing the issue
- How to check for recent legislative changes affecting the area

**WHAT TO WATCH OUT FOR**
Flag 2–3 common research pitfalls specific to this issue — things like a recent statutory change that might make older cases misleading, a circuit split that means cases from one jurisdiction won't help in another, or a commonly confused legal standard that could send the attorney down the wrong path.

Do NOT include any legal analysis, case summaries, or opinions about what the law says. You are helping the attorney FIND the authorities — they will READ and ANALYZE them.

Here is the legal issue:

[PASTE YOUR LEGAL QUESTION OR ISSUE HERE]

Jurisdiction: [STATE, FEDERAL CIRCUIT, OR "GENERAL"]
Platform: [WESTLAW / LEXIS NEXIS / BOTH]
Searches already run (if any): [DESCRIBE WHAT YOU'VE ALREADY TRIED, OR "STARTING FRESH"]
```

## Example Output

> **Issue provided:** "I need to research whether a trucking company can be held vicariously liable for an independent contractor driver's negligence in causing a highway accident in Georgia. The company's logo was on the truck and they controlled the delivery route and schedule."

---

**RESEARCH PLAN**

1. **Georgia vicarious liability statute and common law standard** — Search Georgia statutes and case law for the foundational rule on employer vicarious liability and the independent contractor exception. Database: GA-CS (Georgia Cases), GA-ST-ANN (Georgia Statutes Annotated). This establishes the baseline legal framework before you go deeper.

2. **Motor carrier-specific vicarious liability under Georgia law** — Narrow to trucking and motor carrier cases specifically. Georgia may treat motor carriers differently than general employers due to federal regulations. Database: GA-CS, then expand to All Federal Cases filtered to N.D. Ga. and 11th Circuit.

3. **FMCSA regulations on motor carrier liability** — Search federal statutes and regulations for the Federal Motor Carrier Safety Administration rules that impose liability on the carrier regardless of contractor status. Database: USCA (U.S. Code Annotated), CFR (Code of Federal Regulations). Key: 49 C.F.R. 390 and 49 U.S.C. 14102.

4. **"Borrowed servant" and "right to control" test in Georgia** — Research Georgia's specific test for when an independent contractor relationship is disregarded. The route control and schedule control facts you described go directly to this test. Database: GA-CS.

5. **Logo/signage as evidence of agency or apparent authority** — Search for cases where the company's branding on the vehicle was used as evidence of an agency relationship or apparent authority. Database: GA-CS, then 11th Circuit, then expand to All State Cases if Georgia authority is thin.

6. **Federal preemption angle** — Check whether federal motor carrier regulations preempt Georgia's independent contractor analysis for trucking companies. Database: All Federal Cases filtered to 11th Circuit.

7. **Secondary sources for the full landscape** — Search treatises and law reviews for a comprehensive discussion of motor carrier vicarious liability. This often surfaces arguments and authority that case-by-case searching misses. Database: Secondary Sources — Treatises, then Law Reviews & Journals.

8. **Recent legislative or regulatory changes** — Check for any 2024–2026 amendments to Georgia's vicarious liability statutes or FMCSA regulations that might change the analysis. Database: GA-ST-ANN (check annotations for recent amendments), Federal Register.

---

**SEARCH QUERIES — WESTLAW**

**Task 1: Georgia vicarious liability baseline**

Terms and Connectors — run in GA-CS:
```
"vicarious liability" /s "independent contractor" /s negligent! /p employ!
```
Designed to surface Georgia cases discussing vicarious liability in the independent contractor context with negligence claims.

```
respondeat +s superior /p "independent contractor" /s motor truck!
```
Catches cases using the respondeat superior framework specifically involving trucking or motor vehicles.

Natural Language — run in GA-CS:
- `vicarious liability for independent contractor driver negligence Georgia`
- `when is a company liable for an independent contractor truck driver's accident`

**Task 2: Motor carrier-specific cases**

Terms and Connectors — run in GA-CS:
```
"motor carrier" "trucking company" /s vicar! liab! /s independent +s contractor
```

Terms and Connectors — run in All Federal Cases, filtered to 11th Circuit:
```
"motor carrier" /p vicar! liab! /p independent +s contractor /p negligent! accident
```

**Task 3: FMCSA regulations**

Terms and Connectors — run in CFR:
```
49 +s 390 /s "motor carrier" /s liab! responsib!
```

Terms and Connectors — run in USCA:
```
49 +s 14102 /s "motor carrier" contractor
```

**Task 4: Right to control test**

Terms and Connectors — run in GA-CS:
```
"right to control" /s "independent contractor" /s liab! /p route schedule
```

```
"borrowed servant" /s "independent contractor" /p motor truck! driv!
```

Natural Language — run in GA-CS:
- `right to control test independent contractor Georgia trucking route schedule`

**Task 5: Logo and branding as agency evidence**

Terms and Connectors — run in GA-CS:
```
logo sign! brand! mark! /s vehicle truck /s "apparent authority" agenc!
```

Expand to All State Cases if Georgia results are thin:
```
logo sign! /s truck vehicle /s "apparent authority" "apparent agency" /p vicar! liab! "independent contractor"
```

**Task 6: Federal preemption**

Terms and Connectors — run in All Federal Cases, filtered to 11th Circuit:
```
"motor carrier" /s preempt! /s "independent contractor" /s state +s law
```

**Task 7: Secondary sources**

Terms and Connectors — run in Secondary Sources - Treatises:
```
"motor carrier" /s "vicarious liability" /s "independent contractor"
```

Terms and Connectors — run in Law Reviews & Journals:
```
"trucking" "motor carrier" /s vicar! liab! /s independent +s contractor /s negligent!
```

---

**SEARCH QUERIES — LEXIS NEXIS**

Lexis uses `w/s` (within sentence), `w/p` (within paragraph), `w/n` (within n words), `and`, `or`, `!` (truncation), `*` (wildcard) — similar to Westlaw but database names differ.

**Task 1** — run in Georgia State Cases:
```
"vicarious liability" w/s "independent contractor" w/p negligen! and employ!
```

**Task 2** — run in GA State Cases, then Federal Cases - 11th Circuit:
```
"motor carrier" or "trucking company" w/s vicar! liab! w/p independent w/s contractor
```

**Task 4** — run in GA State Cases:
```
"right to control" w/s "independent contractor" w/p route or schedule
```

**Task 5** — run in All State Cases:
```
logo or signage or brand! w/s truck or vehicle w/p "apparent authority" or "apparent agency" w/p "independent contractor"
```

Note: Lexis organizes secondary sources differently — use the "Secondary Materials" content type and filter by "Treatises" or "Law Reviews" rather than searching a single combined database.

---

**KEY TERMS & SYNONYMS**

| Legal Term | Synonyms & Alternate Phrasings | Related Statutory Language | Westlaw Key Number |
|---|---|---|---|
| Vicarious liability | Respondeat superior, imputed liability, imputed negligence, liability for acts of another | "liable for the acts of" | Master and Servant 300 |
| Independent contractor | Contract driver, owner-operator, non-employee, hired carrier | "independent contractor" as defined in O.C.G.A. 34-9-2 | Master and Servant 11 |
| Right to control | Control test, degree of control, manner and means, supervision and control | "right to control the time, manner, and method" | Master and Servant 12 |
| Motor carrier | Trucking company, carrier, for-hire carrier, common carrier, contract carrier | "motor carrier" per 49 U.S.C. 13102 | Automobiles 228 |
| Apparent authority | Apparent agency, ostensible agency, agency by estoppel | "holding out," "reasonable belief" | Agency 125 |
| Borrowed servant | Borrowed employee, special employee, loaned servant | "special employer" | Master and Servant 15 |

---

**SUGGESTED KEY NUMBERS & TOPICS (WESTLAW)**

- **Master and Servant 300–332** — Vicarious liability, respondeat superior, scope of employment
- **Master and Servant 11–20** — Independent contractor vs. employee distinctions
- **Automobiles 228–250** — Motor carrier liability, owner liability for driver negligence
- **Agency 125–140** — Apparent authority, agency by estoppel

Start with the Key Number digest for Georgia. If Georgia digest results are thin on motor carrier-specific entries, expand to the 11th Circuit digest.

---

**SUGGESTED LEXIS HEADNOTES & TOPICS**

- Torts > Vicarious Liability > Employer-Employee Relationship > Independent Contractors
- Transportation Law > Motor Carriers > Liability > Vicarious Liability
- Agency > Apparent Authority > Third Party Reliance
- Torts > Negligence > Motor Vehicle Accidents > Commercial Vehicles

---

**NEXT SEARCHES AFTER INITIAL RESULTS**

- Once you find a strong Georgia case on motor carrier vicarious liability, use **Citing References** (Westlaw) or **Shepardize** (Lexis) to find every case that cited it — filter by Georgia and 11th Circuit. This often surfaces recent unpublished decisions that don't show up in regular searches.
- **KeyCite / Shepard's flags**: Watch specifically for any yellow or red flags on older Georgia Supreme Court vicarious liability cases — this area of law has shifted in multiple states post-FMCSA regulatory changes.
- Search **Am. Jur. 2d Motor Vehicles** and **Georgia Jurisprudence** for the treatise treatment — these often lay out the full test with every element cited to authority, which saves you from having to reconstruct it case by case.
- Run a **Federal Register** search for any pending FMCSA rulemaking on independent contractor classification — this is an active regulatory area as of 2025–2026.

---

**WHAT TO WATCH OUT FOR**

1. **The FMCSA "statutory employee" doctrine can override the state-law independent contractor analysis.** Under federal regulations, the motor carrier listed on the operating authority may be liable regardless of whether the driver is technically an independent contractor under Georgia common law. Don't stop at state law — the federal overlay changes the game.

2. **Georgia updated its workers' compensation independent contractor test (O.C.G.A. 34-9-2) — make sure you're not conflating the workers' comp test with the tort vicarious liability test.** They have different elements and different case law. Cases applying the workers' comp test will show up in your searches but may not be directly on point.

3. **"Apparent authority" cases in Georgia require reliance by the specific plaintiff.** The logo on the truck helps, but you'll want to check whether Georgia requires the injured party to have actually seen and relied on the branding, or whether its mere presence is enough. This is a fact-specific issue that varies by case.

---

## Tips for Best Results

- **Tell the skill what you've already tried.** If you've already run searches and found some cases, paste that in. The skill will suggest ways to go deeper instead of giving you searches that retread the same ground.
- **Be specific about your platform.** Westlaw and Lexis have different search syntax, different database names, and different digest systems. If you only use one, say so — you'll get more targeted queries.
- **Include the facts that make your issue tricky.** The more specific you are about the wrinkle in your case (the logo, the route control, the schedule control), the more targeted the search queries will be.
- **Run the queries as written first, then adjust.** If a query returns too many results, add a date restriction or jurisdiction filter. If it returns too few, drop the most specific connector or try the Natural Language alternative.
- **Use this skill at the beginning of your research session, not the end.** The whole point is to walk into Westlaw or Lexis with a plan instead of winging it.

## What to Do with the Output

1. **Open the Research Plan and work through it in order.** The tasks are sequenced so earlier results inform later searches.
2. **Copy-paste the search queries directly into Westlaw or Lexis.** They're formatted for the search bar — no reformatting needed.
3. **Use the Key Terms & Synonyms table to expand searches that come back too narrow.** Swap in synonyms and re-run.
4. **Use the Key Number / Headnote suggestions to browse the digest system** when keyword searching isn't cutting it.
5. **Come back to the skill when you hit a wall.** Paste in what you've found so far, describe where you're stuck, and get a new set of search strategies for the next layer of research.

## Variations

**Research Expansion** — Already found a few key cases? Paste them in along with your issue and ask the skill to suggest searches that go beyond what you already have. It'll focus on finding authority you might have missed — different doctrines, different statutory angles, secondary sources that discuss your cases.

**Database Selector** — Not sure which Westlaw or Lexis database to search? Describe your issue and ask the skill to recommend the specific databases and content types to use, with an explanation of what each one covers and why it's relevant.

**Search Query Translator** — Have a Westlaw search that's working great but need to run the same search on Lexis (or vice versa)? Paste the query and the skill will translate it to the other platform's syntax and database structure.

**Cite-Checking Research** — Found a case you're relying on? Paste the citation and ask the skill to build a search strategy for checking whether the case is still good law, finding cases that distinguished or limited it, and identifying the strongest negative treatment to anticipate.

## Additional Resources

This skill includes a bundled research checklist (`resources/research-checklist.md`). Use it after your Westlaw or Lexis session to verify you haven't missed a line of authority, check that your key cases are still good law, and make sure you've covered all the angles before you report your findings or start drafting.
