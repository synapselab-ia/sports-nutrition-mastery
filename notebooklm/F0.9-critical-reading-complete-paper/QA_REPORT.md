# F0.9 — NotebookLM Package QA Report

**Action:** `F0-A19`

**Module:** `F0.9 — Critical reading of a complete paper`

**Package:** `notebooklm/F0.9-critical-reading-complete-paper/`

**QA date:** `2026-09-10`

**Files reviewed:**

- `MANIFEST.md`
- `STUDY_GUIDE.md`
- canonical F0.9 `LESSON.md`
- source registry entries actually used by manifest v1

**Package decision:** `PASS — READY_FOR_STUDY`

---

# 1. Corpus-scope QA — PASS

Manifest v1 uses exactly **seven sources**:

1. canonical F0.9 lesson — `CORE`;
2. `F0-S30` Klemp et al. 2025 full paper — `CORE`;
3. `F0-S31` ClinicalTrials.gov `NCT05922475` — `SUPPORT`;
4. `F0-S01` CONSORT 2025 — `SUPPORT`;
5. `F0-S07` RoB 2 current official resource — `SUPPORT`;
6. `F0-S29` Heinsberg & Weeks 2022 post-hoc power paper — `SUPPORT`;
7. `F0-S18` GRADE Book overview — `CONTRAST`.

This is deliberately smaller than loading all F0.1–F0.8 sources into NotebookLM.

Every external source has a non-redundant instructional job:

- full paper → real appraisal object;
- registry → timeline/prespecification audit;
- CONSORT → reporting visibility/navigation;
- RoB 2 → result-specific bias architecture;
- Heinsberg & Weeks → completed-study power safeguard;
- GRADE overview → one-paper-versus-body certainty boundary.

No extra source is present merely because it appeared in a prior unit.

---

# 2. Mandatory source inclusion QA — PASS

The current `NEXT_ACTION` required the initial corpus to include:

- approved F0.9 lesson;
- legally accessible `F0-S30` full paper;
- `F0-S31` registry record.

All three are present.

The package does not replace the real paper with an AI summary or answer-key reconstruction.

---

# 3. External source/link/version recheck — PASS

All living/current external sources actually used in manifest v1 were rechecked on `2026-09-10`.

## F0-S30 — Klemp et al. 2025

Verified through the current PMC record:

- title remains *Neither pre-sleep nor post-exercise protein consumption influences resistance exercise training adaptations in older adults*;
- publication remains 2025, *Journal of the International Society of Sports Nutrition*, 22(1):2519511;
- DOI remains `10.1080/15502783.2025.2519511`;
- PMC full text remains accessible;
- PMC states the article is Open Access under **CC BY 4.0**;
- the article explicitly identifies `NCT05922475` as its ClinicalTrials.gov identifier.

No full-text copy is committed to GitHub by this package.

## F0-S31 — ClinicalTrials.gov NCT05922475

Verified:

- official URL `https://clinicaltrials.gov/study/NCT05922475` resolves to the public registry resource;
- it remains the registry companion identified by the paper;
- the package tells the learner to inspect dates/version history directly rather than providing a completed prespecification verdict in the Study Guide.

## F0-S01 — CONSORT 2025

Verified through the current BMJ statement:

- CONSORT 2025 remains the current general randomized-trial reporting statement;
- the checklist contains **30 items**;
- current reporting includes trial registration, protocol/SAP access, data sharing/open science, changes after trial commencement, analysis populations, missing-data handling and intervention delivery;
- the source is reporting guidance, not a validity/RoB score.

## F0-S07 — RoB 2

Verified through `riskofbias.info`:

- current version for individually randomized parallel-group trials remains **22 August 2019**;
- official materials remain licensed **CC BY-NC-ND 4.0**;
- the package links the official resource and does not republish tool documents/templates.

## F0-S29 — Heinsberg & Weeks 2022

Verified through PMC:

- article remains *Post hoc Power is Not Informative*, *Genetic Epidemiology* 2022;46(7):390–394;
- DOI remains `10.1002/gepi.22464`;
- the paper explicitly argues that post-hoc/observed power based on completed-study observed results is misleading/redundant for interpretation and recommends attention to confidence intervals/design context instead.

F0.9 applies this narrowly: a post-study power/sensitivity calculation is not posterior evidence and cannot substitute for observed treatment-effect uncertainty.

## F0-S18 — GRADE Book overview

Verified through the living official GRADE Book:

- chapter remains *Overview of the GRADE approach*;
- last modified remains **12 May 2026**;
- certainty is handled at evidence/question/outcome level;
- GRADE explicitly separates certainty assessment from the process of formulating recommendations.

F0.9 uses this as a contrast boundary only; it does not perform a full GRADE body rating from one paper.

No source-version change required revision of the approved F0.9 lesson before package approval.

---

# 4. Source-registry QA — PASS

All seven manifest sources are already registered in `foundations/F0-scientific-literacy/SOURCE_INDEX.md`:

- `F0-S01`;
- `F0-S07`;
- `F0-S18`;
- `F0-S29`;
- `F0-S30`;
- `F0-S31`;
- project lesson is locally identified as `F0-R09` in this package.

No new external source ID is required for F0-A19.

The source index was already advanced to `Last researched: 2026-09-10` during F0-A18, so this package does not create duplicate entries.

---

# 5. STUDY PACKAGE QA — PASS

Required checks from `00_SYSTEM/QA_PROTOCOL.md`:

- sources exist and are intended → PASS;
- source priority/function explained → PASS;
- questions cover concept, mechanism, critique and integration → PASS;
- no protected source improperly published → PASS;
- manifest version matches current F0.9 unit → PASS.

The corpus is small enough to audit manually and broad enough to support the target competence.

---

# 6. Twelve-step sequence QA — PASS

The Study Guide repeatedly trains the canonical sequence:

`Question/estimand → Design/sampling → Intervention/exposure/comparator → Outcome measurement → Bias/confounding/missingness → Sample size/analysis plan → Effect estimate/uncertainty → Multiplicity/exploration → Result robustness → Applicability → Consistency with authors’ conclusion → What the paper does not establish`

The sequence is not presented as a scoring checklist. Each field requires substantive reasoning and source retrieval.

---

# 7. Article-navigation/provenance QA — PASS

The package requires learners to distinguish and navigate:

- main paper;
- supplement/appendix;
- registry;
- protocol;
- SAP;
- data/code repository.

The Study Guide includes a provenance pass before interpretation and explicitly separates:

`identity/version/access facts`

from:

`methodological judgment`.

The learner must use timestamps to determine what a registration/protocol/SAP can establish about prespecification.

---

# 8. Extraction-before-interpretation QA — PASS

The package requires:

## PICO/estimand table

- Population;
- Intervention/exposure;
- Comparator;
- Outcome;
- Time;
- Estimand/contrast;
- Analysis population;
- Target context.

## Material-result table

- Outcome/timepoint;
- Contrast;
- Effect measure;
- Point estimate;
- CI/SE;
- p-value;
- Analysis population;
- Prespecification status;
- Practical threshold;
- Caveat.

The Study Guide explicitly instructs the learner to write `NOT CLEARLY REPORTED` / `UNCLEAR` rather than invent missing information.

---

# 9. Quantitative-inference QA — PASS

The package preserves F0.5/F0.6 reasoning:

- within-group change is not automatically a between-group treatment effect;
- p-values do not replace effect estimates;
- `p>0.05` does not prove no effect;
- `p>0.05` does not prove equivalence;
- formal equivalence/non-inferiority requires an appropriate margin/design/analysis;
- completed-study interpretation prioritizes estimate + CI + practical threshold/context + design/bias;
- observed/post-hoc power cannot rescue the interpretation of a completed result.

The Study Guide requires the learner to classify prospective power planning, observed precision and post-study power as different objects.

---

# 10. Prespecification/multiplicity QA — PASS

The package requires a chronological audit using paper + registry rather than assuming prospectivity from document existence.

It also requires the learner to reconstruct the available claim family across:

- outcomes;
- timepoints;
- arms/contrasts;
- pairwise comparisons;
- transformations/models;
- sensitivity analyses;
- subgroup/exploratory analyses when present.

The guide warns against both extremes:

- ignoring multiplicity;
- accusing selective reporting merely because multiple analyses/outcomes exist.

---

# 11. Risk-of-bias QA — PASS

RoB is taught result-specifically.

The learner must articulate:

`mechanism → result affected → plausible direction/impact → evidence or uncertainty`.

The package blocks:

- `RCT = low risk`;
- global numerical quality scores;
- transfer of one result's RoB judgment to every outcome;
- reporting completeness as a substitute for bias reasoning.

The package uses the current RoB 2 architecture without embedding or redistributing licensed templates.

---

# 12. Robustness QA — PASS

The Study Guide distinguishes:

`robustness = stability under defensible assumptions`

from:

`result-shopping = searching for an analysis that gives a preferred answer`.

Open data/code are treated as auditability/reproducibility resources, not retroactive design repair.

---

# 13. Applicability QA — PASS

The package requires structured evidence-target comparison across:

`Population → Intervention/exposure → Comparator → Outcome → Time → Setting → Decision context`.

Learners must explain why a mismatch could matter rather than mechanically penalizing demographic differences.

Internal validity and applicability remain separate axes.

---

# 14. Single-paper versus body-certainty QA — PASS

`F0-S18` is intentionally a `CONTRAST` source.

The package requires the learner to understand:

- one paper can be appraised for result-specific bias, uncertainty and applicability;
- one paper cannot by itself define the certainty of a reconstructed evidence body;
- one favorable/low-RoB RCT does not automatically equal high-certainty field consensus;
- recommendation strength cannot be inferred from a single result alone.

This preserves F0.8 and prevents premature F0.10 reasoning.

---

# 15. Blind-assessment contamination QA — PASS

The initial NotebookLM corpus explicitly excludes:

- F0.9 `EXERCISES.md`;
- F0.9 `ANSWER_KEY.md`;
- F0.9 production `QA_REPORT.md`;
- full `SOURCE_INDEX.md`;
- F0.4 `ENTRY_DIAGNOSTIC.md`.

The Study Guide does **not** provide the completed appraisal of the Klemp paper.

It asks the learner to discover:

- paper/registry timeline;
- exact contrasts;
- outcome/result architecture;
- uncertainty;
- bias concerns;
- multiplicity/prespecification issues;
- applicability;
- proportionality of authors' conclusions.

Generic hints describe categories of reasoning but do not provide the answer-key conclusion for the paper.

The paper title/abstract themselves remain part of the real study object and are not artificially hidden; the learner is trained to treat them as claims to audit.

---

# 16. Copyright/public-repository QA — PASS

- no user/private health data persisted;
- no credentials/secrets persisted;
- no third-party full-text file copied into GitHub;
- `F0-S30` is linked through its legal PMC source and is CC BY 4.0;
- `F0-S31` is linked as a public registry record;
- RoB 2 licensed documents are not copied;
- CONSORT/GRADE/Heinsberg sources are linked/cited rather than republished;
- package Markdown is original project-authored content.

---

# 17. Pedagogical QA — PASS

The Study Guide contains **22 ordered passes**:

1. paper-as-argument orientation;
2. source-layer anatomy;
3. provenance;
4. question/estimand;
5. design/sampling;
6. intervention/comparator;
7. outcome architecture;
8. result-table extraction;
9. within-versus-between inference;
10. magnitude/CI/threshold;
11. nonsignificance/equivalence;
12. sample size/precision/power;
13. prespecification timeline;
14. multiplicity;
15. result-specific RoB;
16. reporting-versus-validity;
17. robustness;
18. applicability;
19. paper-versus-body certainty;
20. authors' conclusion audit;
21. what-is-not-established boundaries;
22. complete blind integration.

This progression moves from navigation/extraction to quantitative and causal judgment, then to integrated appraisal.

---

# 18. Critical-fail coverage — PASS

The package explicitly blocks:

- title/abstract-only appraisal;
- design-label-only appraisal;
- reporting-checklist validity scoring;
- `p<0.05 = true/important` reasoning;
- `p>0.05 = no effect/equivalence` reasoning;
- observed/post-hoc-power rescue;
- ignoring registry/protocol/SAP timing;
- ignoring multiplicity;
- global quality/RoB scoring;
- within-group change as treatment effect;
- result-shopping mislabeled as robustness;
- open-data-as-validity shortcut;
- unsupported extrapolation;
- single-paper GRADE certainty;
- copying authors' conclusion without independent reconstruction;
- invention of unreported information.

---

# 19. Production versus learning-state QA — PASS

F0-A19 is package production only.

Therefore:

- F0.1–F0.9 learner states remain pending/unvalidated;
- F0.9 is not marked studied from package creation;
- no module becomes `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`;
- F0.4 quantitative diagnostic remains `UNOBSERVED`;
- F0.10 production remains deferred until this package is closed in the canonical checkpoint.

---

# 20. Gate decision

Question from the canonical QA protocol:

> Can a capable learner use this package to learn the content, understand where conclusions come from, recognize limitations and demonstrate the target competence without hidden gaps?

**Decision:** `YES`.

The first-pass F0.9 NotebookLM package is approved as:

`PASS — READY_FOR_STUDY`
