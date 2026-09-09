# F0.4 — NotebookLM Study Package QA Report

**Module:** `F0.4 — Descriptive statistics, distributions and sampling variation`
**Package version:** `1`
**Reviewed:** `2026-09-09`
**Package decision:** `PASS — READY_FOR_STUDY`
**Learner-state change:** none
**Quantitative diagnostic change:** none; remains `UNOBSERVED`

This report records QA of the NotebookLM package only. It does not record that the learner studied F0.4, does not score the entry diagnostic and does not authorize any mastery-state transition.

---

## 1. Package contents — PASS

Required files:

- `notebooklm/F0.4-descriptive-statistics/MANIFEST.md`;
- `notebooklm/F0.4-descriptive-statistics/STUDY_GUIDE.md`;
- `notebooklm/F0.4-descriptive-statistics/QA_REPORT.md`.

The package is aligned to:

- approved canonical lesson `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/LESSON.md`;
- prerequisite/diagnostic architecture in `ENTRY_DIAGNOSTIC.md`;
- F0.4 production QA;
- project NotebookLM protocol.

The package does not replace the canonical lesson or the independent diagnostic/assessment.

---

## 2. Corpus-size and auditability gate — PASS

The first-pass NotebookLM corpus is limited to **four sources**:

1. canonical F0.4 lesson — `CORE`;
2. NIST/SEMATECH Exploratory Data Analysis chapter — `CORE`;
3. Altman & Bland, *Standard deviations and standard errors* — `SUPPORT`;
4. ICH E9/E9(R1) official EMA page — `CONTRAST`.

This is intentionally smaller than the full quantitative F0 source registry.

### Why no additional statistics sources were added

F0.4 is foundational and descriptive. The canonical lesson already provides the self-contained definitions, calculations and synthetic applications. NIST adds an external EDA/graphics anchor, Altman/Bland targets the major SD/SE misconception, and ICH E9 supplies only a boundary contrast between descriptive summaries and the broader target-question/analysis chain.

Adding ASA p-value statements, power/sample-size planning material, Cochrane effect-measure chapters or general inferential textbooks would expand retrieval beyond the F0.4 target and risk prematurely teaching F0.5/F0.6.

No new source was registered merely to increase corpus size.

---

## 3. Source/file/link verification — PASS

Verification date: `2026-09-09`.

### Canonical F0.4 lesson

Verified on canonical `main` with production state `APPROVED`.

The preferred NotebookLM source is the raw project Markdown. If raw URL ingestion fails, the guide instructs the learner to upload the same canonical Markdown file rather than an AI summary.

### NIST/SEMATECH EDA

Verified official NIST resources:

- legacy e-Handbook remains accessible;
- direct Chapter 1 EDA endpoint remains available at `https://www.itl.nist.gov/div898/handbook/eda/eda.htm`;
- NIST's modern publication page identifies Heckert & Filliben's Chapter 1, published 2003, with NIST page update recorded as 12 October 2021.

The direct chapter endpoint is preferred for NotebookLM content ingestion because it exposes the actual EDA chapter navigation/content rather than only bibliographic metadata.

Instructional use is restricted to:

- exploratory inspection;
- graphical analysis;
- distribution structure;
- outliers/anomalies;
- descriptive reasoning.

NIST's later hypothesis-testing/modeling material is outside F0.4.

### Altman & Bland — SD versus SE

Verified BMJ article:

- Altman DG, Bland JM;
- *Standard deviations and standard errors*;
- BMJ 2005;331:903;
- DOI `10.1136/bmj.331.7521.903`;
- article remains available on BMJ.

The article explicitly targets the distinction between data variability and sampling/inferential precision. F0.4 uses:

- SD = variability among observations;
- SE = sampling variability/precision of an estimate;
- simple mean relation `SE = SD/√n`.

Confidence-interval content in the note remains deferred to F0.5.

### ICH E9/E9(R1)

Verified current EMA page:

- ICH E9 Statistical Principles for Clinical Trials — Step 5;
- ICH E9(R1) Addendum on Estimands and Sensitivity Analysis — Step 5;
- no replacement current version was located on the official page on 2026-09-09.

F0.4 uses this only as a contrast source for objective/variable/target/analysis alignment. Regulatory detail and advanced estimand/sensitivity-analysis machinery are explicitly outside the study target.

---

## 4. Role-assignment QA — PASS

### `CORE` — canonical F0.4 lesson

Function:

- exact project vocabulary;
- self-contained formulas and examples;
- scope boundaries;
- integrated descriptive reasoning sequence;
- sports/exercise-flavored synthetic transfer without substantive nutrition claims.

Limitation:

- project-authored instructional source; external methodological traceability remains required.

### `CORE` — NIST EDA

Function:

- external institutional support for graphical/exploratory inspection;
- distribution structure;
- anomalies/outliers;
- evidence that EDA is more than one-number summarization.

Limitation:

- engineering/general-statistics context and broader methods than F0.4.

### `SUPPORT` — Altman & Bland

Function:

- focused correction of SD-versus-SE confusion;
- sample-size effect on SE of a simple mean.

Limitation:

- concise note, not comprehensive statistics training; CI content belongs later.

### `CONTRAST` — ICH E9/E9(R1)

Function:

- show that descriptive summaries live inside a larger question/outcome/target/analysis framework;
- prevent descriptive group differences from being silently relabeled as causal treatment effects.

Limitation:

- regulatory/technical clinical-trial guidance; not a universal descriptive-statistics manual.

Each source therefore has a distinct instructional function.

---

## 5. Required F0-A09 learning-sequence coverage — PASS

### Variable type

Pass 1 requires classification from semantic meaning rather than numeric encoding.

### Distribution inspection

Pass 2 requires shape, skew, bounds, clusters and extremes to be described before summary selection.

### Center + dispersion choice

Passes 2–3 require explicit justification of mean/median/mode plus range/variance/SD/IQR/quantiles.

### Outlier handling

Pass 4 requires provenance investigation before exclusion/correction/retention decisions.

### Visualization choice/audit

Pass 5 covers graph selection and deliberate misleading-graph scenarios: truncated axes, hidden distributions, incompatible scales, selective windows and bin choices.

### Population/sample and parameter/statistic

Pass 6 repeatedly separates target population properties from sample-computed statistics.

### Sample distribution versus sampling distribution

Pass 7 uses repeated-sampling thought experiments and makes this a major gate rather than a vocabulary item.

### SD versus SE

Pass 8 explicitly requires object identification before formula use.

### Sample-size consequences

Pass 9 separates what larger `n` can stabilize from what it cannot automatically change, including individual SD, systematic bias and representativeness.

### `SE(mean) ≈ SD/√n`

Pass 8 uses this only for the simple independent-observation mean and explicitly warns against generalizing it to clustered/paired/weighted/model-based estimators.

### F0.5/F0.6 boundaries

Every major pass prohibits importing full CI, p-value, effect-size, power or multiplicity material.

---

## 6. Diagnostic and answer-leakage control — PASS

Excluded from the initial NotebookLM corpus:

- `ENTRY_DIAGNOSTIC.md`;
- `EXERCISES.md`;
- `ANSWER_KEY.md`;
- production `QA_REPORT.md`;
- full `SOURCE_INDEX.md`.

This is especially important because F0.4 `ANSWER_KEY.md` contains both diagnostic and unit-assessment answers.

The study guide makes the honest validation sequence explicit:

1. if the diagnostic is unobserved, complete it independently first;
2. score/route only from observed responses;
3. complete any real P1/P2-QB remediation;
4. then study F0.4;
5. complete `EXERCISES.md` independently after study;
6. consult answers only after the first attempt.

Package creation itself does not alter the diagnostic state.

---

## 7. Scientific-boundary QA — PASS

The package preserves all approved F0.4 safeguards:

- variable encoding is not confused with measurement meaning;
- right skew is not defined by the non-universal shortcut `mean > median`;
- median/IQR are not declared universally superior;
- quantile-convention differences are acknowledged;
- outlier does not mean error;
- histogram is distinct from bar chart;
- scatterplot association is not causality;
- axis truncation is analyzed rather than mechanically forbidden;
- sample distribution and sampling distribution are distinct objects;
- SD is not SE;
- larger n is not represented as automatic SD reduction;
- larger n is not a cure for F0.3 systematic bias;
- observed range can widen with larger samples;
- transformations do not repair bias/design;
- synthetic sports/nutrition examples do not create intervention recommendations.

---

## 8. Inferential-scope QA — PASS

The package does **not** teach as F0.4 competencies:

- 95% CI interpretation;
- p-values/NHST;
- standardized/raw effect-size interpretation;
- smallest effect of practical interest;
- formal power/sample-size planning;
- Type I/II error;
- multiplicity;
- advanced estimator variance;
- meta-analysis.

Altman/Bland and ICH E9 contain concepts that extend beyond F0.4, but the manifest and guide explicitly limit retrieval prompts to assigned portions.

---

## 9. Pedagogical QA — PASS

The package progresses through:

`data meaning → distribution → descriptive summaries → anomalies → graphics → population/sample → repeated-sampling intuition → SD/SE → sample-size prediction → transformation boundary → inferential boundary → mixed integration`

The learner must repeatedly:

- retrieve definitions without answer exposure;
- calculate manually;
- justify choices;
- compare near-neighbor concepts;
- predict consequences;
- audit graphs;
- repair exaggerated claims;
- state bounded conclusions.

This prevents passing through formula memorization alone.

---

## 10. Mastery-practice QA — PASS

The study guide supports practice at:

- `K1` definitions/classification;
- `K3` compare related statistical objects;
- `K4` interpret data/graphs;
- `K5` predict outlier/sample-size consequences;
- `K6` calculate and select summaries;
- `K7` integrate descriptive reasoning with F0.2/F0.3 boundaries;
- `K8` identify unsupported interpretation.

The independent F0.4 assessment remains outside NotebookLM and is required for observed progression evidence.

---

## 11. Copyright/public-repository QA — PASS

The GitHub package contains only:

- project-authored Markdown;
- bibliographic citations;
- official/public links;
- study instructions.

No third-party PDF or copyrighted chapter text was copied into the public repository.

If a source must be uploaded manually to NotebookLM, it should be obtained lawfully by the learner and not recommitted to this public repository without redistribution permission.

No personal, clinical or sensitive learner information is stored.

---

## 12. Learner-state integrity — PASS

Before package creation:

- F0.1 learner validation: pending;
- F0.2 learner validation: pending;
- F0.3 learner validation: pending;
- F0.4 learner state: `UNSEEN`;
- F0.4 quantitative diagnostic: `UNOBSERVED`.

After package creation:

- all remain unchanged;
- package readiness is production metadata only;
- no `P1_REPAIR` or `P2-QB_REQUIRED` state can be inferred without real diagnostic responses;
- `MASTERED` remains impossible without observed and later repeated performance.

---

## 13. Final Study Package gate

Question:

> Can a capable learner with the required quantitative bridge use this small, auditable corpus to classify variables, inspect distributions, choose defensible summaries/graphs, investigate outliers, distinguish sample/population and sample/sampling distributions, explain SD versus SE, predict sample-size consequences and preserve inferential boundaries—without contaminating the entry diagnostic or independent assessment?

**Decision:** yes.

**Package state:** `READY_FOR_STUDY`.
