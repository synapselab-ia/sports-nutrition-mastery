# F0.10 — NotebookLM Package QA Report

**Action:** `F0-A21`
**Module:** `F0.10 — Synthesis and communication of uncertainty`
**QA date:** `2026-09-10`
**Manifest version:** `1`
**Package decision:** `PASS — READY_FOR_STUDY`

Files reviewed:

- `MANIFEST.md`
- `STUDY_GUIDE.md`
- approved F0.10 `LESSON.md`
- source/link/version status for every external source in the manifest

---

## 1. Package scope — PASS

The package implements the exact F0-A21 target.

It trains:

`reconstructed evidence → invariant core → calibrated claim → audience translation → drift audit → update conditions`

The guide requires the eight-field invariant core:

1. target;
2. direction;
3. magnitude;
4. precision;
5. threshold;
6. certainty;
7. applicability;
8. boundaries/update conditions.

The package does not introduce a new substantive nutrition recommendation and does not execute the cumulative F0 exit assessment.

---

## 2. Corpus-size and auditability QA — PASS

Initial corpus contains exactly **six sources**:

1. `F0-R10` — canonical F0.10 lesson — `CORE`;
2. `F0-S19` — GRADE intervention-certainty principles — `CORE`;
3. `F0-S18` — GRADE overview — `SUPPORT`;
4. `F0-S20` — GRADE indirectness — `SUPPORT`;
5. `F0-S08` — ASA p-value statement — `SUPPORT`;
6. `F0-S09` — ASA Task Force statement — `CONTRAST`.

No redundant source was added merely to increase corpus size.

Source functions are distinct:

- lesson = complete workflow and learner-facing integration;
- F0-S19 = threshold/range-aware body-level certainty;
- F0-S18 = certainty categories and certainty-versus-recommendation boundary;
- F0-S20 = indirectness/applicability boundary;
- F0-S08 = p-value misuse safeguards;
- F0-S09 = contrast against both ritual thresholding and simplistic abandonment of p-values.

This is small enough for source attribution and broad enough for all material F0.10 boundaries.

---

## 3. External source/link/version QA — PASS

Every external manifest source was rechecked on `2026-09-10`.

### F0-S08 — ASA Statement on p-Values

Verified from the official ASA-hosted statement:

- the six core principles remain available;
- p-values do not provide the probability that the studied hypothesis is true;
- conclusions should not be based only on whether a threshold is crossed;
- p-values/statistical significance do not measure effect size or importance;
- a p-value alone is not a complete evidential summary.

Package use is accurate: p-values remain one output, not a truth/importance/absence detector.

### F0-S09 — ASA President’s Task Force statement

Verified from the ASA-hosted 2021 statement:

- properly applied/interpreted p-values and significance tests retain a legitimate role;
- broader sound inference requires attention to uncertainty, variability, multiplicity and replicability.

Package use is accurate: the source is deliberately a `CONTRAST` against the false binary “threshold worship versus p-values are useless.”

### F0-S18 — GRADE overview

Verified from the living GRADE Book:

- page remains `Last modified: 12 May 2026`;
- certainty continues to use four categories;
- GRADE continues to distinguish certainty of evidence from recommendation processes.

Package use is accurate: certainty is not converted into recommendation strength.

### F0-S19 — GRADE intervention-certainty principles

Verified from the living GRADE Book:

- page remains `Last modified: 21 Aug 2025`;
- certainty is defined relative to confidence that the true effect lies within a range or above/below a threshold of interest;
- certainty is assessed across a body of evidence for an outcome, not as a quality grade for one paper.

Package use is accurate: estimate/range/threshold and body/outcome certainty are kept distinct from magnitude labels.

### F0-S20 — GRADE indirectness

Verified from the living GRADE Book:

- page remains `Last modified: 12 May 2026`;
- indirectness continues to cover applicability/generalizability/transferability through alignment of evidence PICO with the target PICO, plus indirect comparisons.

Package use is accurate: audience translation may not silently broaden the target population/intervention/comparator/outcome.

No source-version change required revision of the approved lesson or manifest. No new source ID is needed; all five external sources already exist in `SOURCE_INDEX.md`.

---

## 4. Claim alignment QA — PASS

The manifest and guide preserve the approved F0.10 claims:

- simplification cannot erase uncertainty;
- p-values do not determine truth, importance or absence;
- estimate + CI/range + practical threshold remain connected;
- `did not detect` is not the same as excluding a meaningful effect;
- nonsignificant superiority is not formal equivalence;
- certainty is not magnitude;
- bias, imprecision, inconsistency, indirectness and missing/dissemination evidence are distinct uncertainty mechanisms;
- direct evidence can be biased;
- conflicting studies are weighted, not counted;
- source hierarchy is not mechanical;
- mechanistic evidence does not automatically establish chronic performance/health outcomes;
- evidence statements remain distinct from recommendations;
- technical/practitioner/lay versions preserve one epistemic core;
- update conditions are explicit rather than generic calls for more research.

No claim in the package is stronger than the approved F0.10 lesson.

---

## 5. Pedagogical progression QA — PASS

The Study Guide uses **20 ordered passes**:

1. role of F0.10;
2. invariant core;
3. estimate/CI/threshold;
4. three distinct claims around absence/equivalence;
5. ASA six-principle boundary;
6. anti-overcorrection on p-values;
7. certainty versus magnitude;
8. threshold/range certainty;
9. mechanisms of uncertainty;
10. directness versus internal validity;
11. PICO scope preservation;
12. conflict without vote counting;
13. anti-mechanical hierarchy;
14. mechanism versus outcome proof;
15. evidence versus recommendation;
16. technical synthesis;
17. practitioner translation;
18. lay translation;
19. drift audit;
20. update conditions and final integration.

Progression is from concept → numerical interpretation → evidence weighting → communication → integration.

Active recall is required before source consultation in each pass.

---

## 6. Fresh-example QA — PASS

The guided examples are synthetic and distinct from the completed independent F0.10 assessment package.

Examples include:

- `G1`: `MD -9 s [95% CI -27,+9]`, threshold `-20 s`, moderate certainty mainly limited by imprecision;
- `G2`: `MD -3 s [95% CI -11,+5]`, threshold `-20 s`, high certainty;
- `G3`: conflicting direct meta-analysis/RCT, observational cohort and acute mechanistic biomarker with threshold `+0.8`.

These examples train the same competency without exposing the assessment answer key.

They are educational/fictitious and are not nutrition prescriptions.

---

## 7. Assessment-contamination QA — PASS

Explicitly excluded from the first-pass corpus:

- F0.10 `EXERCISES.md`;
- F0.10 `ANSWER_KEY.md`;
- F0.10 production `QA_REPORT.md`;
- full `SOURCE_INDEX.md`;
- F0.4 `ENTRY_DIAGNOSTIC.md`.

The Study Guide directs the learner to close NotebookLM before the independent assessment and open the answer key only after the attempt.

No completed F0.10 assessment solution is embedded in the manifest or Study Guide.

---

## 8. Critical-fail coverage — PASS

The package actively trains detection/repair of:

- `p<0.05 = true/important`;
- `p>0.05 = no effect`;
- nonsignificant superiority = equivalence;
- deleting material CI/threshold information to simplify prose;
- `low certainty = no effect`;
- `high certainty = large/important effect`;
- `direct evidence = unbiased evidence`;
- rhetorical 50/50 balance between inferentially unequal sources;
- automatic RCT supremacy without claim-specific appraisal;
- mechanistic outcome → chronic performance/health claim;
- certainty of one outcome → strong recommendation;
- population/outcome/time/context expansion during translation;
- stronger causal verbs than the design supports;
- practitioner/lay language becoming more certain than technical language;
- generic “more research is needed” without an update condition.

---

## 9. Public-repository/copyright QA — PASS

- no personal or private health information is persisted;
- no credentials/secrets are persisted;
- no ASA PDF content, GRADE chapter text or other third-party full text is republished;
- repository contains only original educational Markdown, references and links;
- external-source URLs are used for access/attribution;
- fictional examples do not identify real people or prescribe individual nutrition.

---

## 10. Production-versus-learning-state QA — PASS

F0-A21 is package production only.

Therefore:

- F0.1–F0.10 learner states remain pending/unvalidated;
- no module is marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`;
- F0.4 quantitative diagnostic remains `UNOBSERVED`;
- NotebookLM study activity does not itself authorize mastery;
- cumulative F0 exit assessment remains a separate subsequent action.

---

## 11. STUDY PACKAGE QA checklist — PASS

- manifest sources exist and are the intended sources: PASS;
- source priority/function/limitation documented: PASS;
- concept coverage: PASS;
- numerical uncertainty/threshold coverage: PASS;
- p-value interpretation coverage: PASS;
- certainty/applicability coverage: PASS;
- critical evidence weighting and false-balance coverage: PASS;
- three-audience translation coverage: PASS;
- drift-audit coverage: PASS;
- update-condition coverage: PASS;
- answer-key leakage prevention: PASS;
- copyright/public-repository compliance: PASS;
- manifest version matches current approved module: PASS.

---

## 12. Final decision

`PASS — READY_FOR_STUDY`

A capable learner using only the approved corpus and Study Guide can learn how to preserve the same scientific uncertainty across technical, practitioner and lay communication, identify where communication drifts beyond evidence, and demonstrate the competency independently without hidden prerequisite content or answer-key contamination.
