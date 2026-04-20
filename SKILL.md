---
name: humanmade
description: Write research papers, scientific manuscripts, reports, essays, and any prose that must read as authentically human. Combines scientific writing (IMRAD, citations, reporting guidelines, figures/tables), critical thinking (methodology critique, bias detection, evidence evaluation), and human-voice writing rules (avoiding AI-detectable patterns). Use for any writing task — research papers, journal submissions, essays, blog posts, documentation, reports, emails, or copy — especially when natural voice and scientific rigor both matter.
---

# Research Writing

This skill has three layers. Apply all three to every piece of writing.

## Layer 1: Human Voice (apply to ALL writing)

### Banned Vocabulary

Never use these. Find concrete alternatives or restructure.

**Adjectives/adverbs:** crucial, pivotal, vital, vibrant, intricate, meticulous/meticulously, groundbreaking, renowned, profound, enduring, indelible

**Verbs:** delve, underscore, highlight (as "emphasize"), showcase, foster, garner, bolster, enhance (when vague), exemplify, encompass, nestled

**Abstract nouns:** tapestry, landscape (figurative), interplay, intricacies, focal point, diverse array, rich heritage, natural beauty

**Connectors/fillers:** Additionally (starting a sentence), Furthermore, It is worth noting, It is important to note/remember/consider

**Puffery phrases:** a testament to, serves as a reminder, reflects broader, symbolizing its ongoing, contributing to the, setting the stage for, marking/shaping the, key turning point, evolving landscape, deeply rooted, commitment to, in the heart of, boasts a

### Sentence Pattern Rules

**No dangling "-ing" analyses.** Don't attach vague significance via participle phrases.
- Bad: "The bridge was completed in 1934, marking a pivotal moment in regional infrastructure."
- Good: "The bridge was completed in 1934."

**No "not just X, but Y" parallelisms.** Don't correct misconceptions nobody has.

**No rule-of-three padding.** Pick one adjective that matters, or use a fact.

**No copula avoidance.** Use "is" and "has." Don't substitute "serves as," "stands as," "represents," "marks," "boasts," "features," "maintains," or "offers."

**No elegant variation.** Repeat the noun. Don't cycle through synonyms to avoid repetition.

### Significance and Tone

- Never add sentences about legacy, broader significance, ecosystem role, or symbolism unless asked. State facts.
- No "challenges and future prospects" sections. No paragraph-ending summaries. No conclusions restating what was said.
- Replace praise with facts. "Inventor of the first train-coupling device" not "a revolutionary titan of industry."
- No promotional register. Cut travel-guide and press-release language.
- No vague attribution ("experts argue," "observers note") without naming them.
- No hedging preambles ("While relatively obscure, it nonetheless..."). Just state it.

### No Repetition Across Sections

Never state the same fact, definition, or idea twice. Not across sections, not within a paragraph, not anywhere in the document. Explain it once, clearly, in the right place. Every subsequent mention refers back, not re-explains. If a term was defined in the introduction, the discussion doesn't define it again. If a method was described in Methods, Results doesn't re-describe it. If a fact appeared in sentence two, sentence five doesn't rephrase it. One and done.

### Structural Rules

- Never use em dashes (—) or en dashes (–). In LaTeX, never use `---` or `--`. Use commas, parentheses, colons, or periods instead.
- Bold: for headings and defined terms only, not emphasis or key takeaways.
- Don't format prose as bullet lists with bold inline headers and colons.
- Don't skip heading levels. Don't use emoji in professional writing.

### What Human Writing Sounds Like

Uneven rhythm. Short sentences next to long ones. Comfortable with "is," "are," "has," "was." Repeats key nouns. Lets the reader judge importance. Uses simple transitions or none. Contains occasional imperfection: a slightly informal phrase, an unexpected word choice, a sentence that serves voice rather than template.

---

## Layer 2: Scientific Writing (apply to research/academic work)

### Process

**Stage 1 — Outline.** Use research-lookup to gather literature. Create bullet-point outlines with key findings, citations, and logical flow. These are scaffolding, not output.

**Stage 2 — Prose.** Convert outlines to flowing paragraphs. Integrate citations naturally within sentences. Add transitions. Vary sentence structure. Never leave bullet points in the final manuscript.

Lists are acceptable only in Methods (inclusion criteria, materials) and Supplementary Materials. Never in Abstract, Introduction, Results, Discussion, or Conclusions.

### IMRAD Structure

- **Introduction:** context, gap, objectives, novelty
- **Methods:** design, population, procedures, analysis (past tense, enough detail for reproduction)
- **Results:** findings with statistics, no interpretation
- **Discussion:** interpretation, comparison with literature, limitations, implications

For alternative structures (reviews, case reports, meta-analyses, protocols), see `references/imrad_structure.md`.

### Citations

Major styles: AMA (numbered superscript, medicine), Vancouver (numbered brackets, biomedical), APA (author-date, social sciences), Chicago (notes or author-date, humanities), IEEE (numbered brackets, engineering).

Cite primary sources. Include recent literature (last 5-10 years). Balance citations across introduction and discussion. Verify against originals. See `references/citation_styles.md`.

### Figures and Tables

Tables for precise numbers; figures for trends and patterns. Each must be self-explanatory with complete captions. Label all axes/columns with units. Include sample sizes and statistical annotations. Roughly one per 1,000 words. Don't duplicate data between text, tables, and figures. See `references/figures_tables.md`.

### Reporting Guidelines

Match the study type: CONSORT (RCTs), STROBE (observational), PRISMA (systematic reviews), STARD (diagnostic accuracy), TRIPOD (prediction models), ARRIVE (animal research), CARE (case reports). See `references/reporting_guidelines.md`.

### Field-Specific Language

Use precise terminology for the target discipline. Define abbreviations at first use. Match audience expertise level. Don't mix terminology across fields (don't call mice "patients"). Use the same term for the same concept throughout. Consult recent papers in the target journal for conventions.

### Writing Quality

- Past tense for methods/results, present for established facts
- Favor 15-20 word average sentence length
- Define technical terms at first use
- Report exact values with appropriate precision
- Distinguish observations from interpretations
- Acknowledge uncertainty proportionally

### LaTeX Reports

When the user asks to create a `.tex` file, report, or any LaTeX document: always use `assets/scientific_report.sty` as the style package and base the document on `assets/scientific_report_template.tex`. Copy both files into the user's working directory. The style provides Helvetica fonts, colored box environments (keyfindings, methodology, recommendations, limitations), professional tables, and scientific notation commands (pvalue, CI, effectsize, meansd). Compile with XeLaTeX. See `references/professional_report_formatting.md` for full documentation.

---

## Layer 3: Critical Thinking (apply when evaluating or presenting evidence)

### Methodology Critique

Evaluate study design appropriateness, internal/external/construct validity, randomization and blinding quality, and measurement reliability. See `references/experimental_design.md` and `references/scientific_method.md`.

### Bias Detection

Check for: confirmation bias, HARKing, publication bias, cherry-picking (researcher biases); sampling, volunteer, attrition, survivorship bias (selection); observer, recall, social desirability bias (measurement); p-hacking, outcome switching, selective reporting, subgroup fishing (analysis); unmeasured confounding. See `references/common_biases.md`.

### Statistical Evaluation

Verify: a priori power analysis, test appropriateness for data type, multiple comparison corrections, correct p-value interpretation, effect sizes with confidence intervals, missing data handling, model overfitting checks. See `references/statistical_pitfalls.md`.

### Evidence Quality

Use the evidence hierarchy (systematic reviews > RCTs > cohort > case-control > cross-sectional > case series > opinion) but remember a well-designed observational study beats a poor RCT. Apply GRADE when appropriate: downgrade for bias, inconsistency, indirectness, imprecision, publication bias; upgrade for large effects, dose-response, confounders that would reduce effect. See `references/evidence_hierarchy.md`.

### Claim Evaluation

For every claim: identify what type it is (causal, associational, descriptive), whether evidence is sufficient for its strength, whether conclusions follow from data, and whether confidence is proportional. Red flags: causal language from correlational studies, "proves," cherry-picked citations, dismissed limitations, extrapolation beyond data. See `references/logical_fallacies.md`.

### Providing Critique

Structure as: summary, strengths, concerns (critical/important/minor), specific recommendations, overall assessment. Be constructive, specific, and proportionate. Name specific biases and fallacies. Apply the same standards regardless of whether you agree with the findings.

---

## References

Load as needed:

- `references/imrad_structure.md` — IMRAD format details
- `references/citation_styles.md` — APA, AMA, Vancouver, Chicago, IEEE
- `references/figures_tables.md` — data visualization best practices
- `references/reporting_guidelines.md` — CONSORT, STROBE, PRISMA, etc.
- `references/writing_principles.md` — scientific communication principles
- `references/professional_report_formatting.md` — scientific_report.sty guide
- `references/scientific_method.md` — methodology and causal inference
- `references/common_biases.md` — bias taxonomy and mitigation
- `references/statistical_pitfalls.md` — statistical errors and correct practices
- `references/evidence_hierarchy.md` — GRADE system and quality assessment
- `references/logical_fallacies.md` — fallacies in scientific discourse
- `references/experimental_design.md` — design checklist

## Assets

- `assets/scientific_report.sty` — LaTeX style package
- `assets/scientific_report_template.tex` — complete template
- `assets/REPORT_FORMATTING_GUIDE.md` — quick reference

## Credits

This is an original work that distills and consolidates insights from multiple sources into a new, unified skill. Inspirations and source material include:

- Wikipedia's "Signs of AI-generated content" guide — https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI-generated_content
- Scientific writing and critical thinking skills by K-Dense Inc.
