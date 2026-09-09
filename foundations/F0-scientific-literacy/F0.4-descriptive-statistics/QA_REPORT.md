# F0.4 — QA report

**Unit:** `F0.4 — Descriptive statistics, distributions and sampling variation`

**Reviewed:** 2026-09-09

**Production decision:** `APPROVED`

This report records production QA only. It does **not** record learner performance, does not score the entry diagnostic and does not change any mastery state.

---

## 1. Scope gate — PASS

### Required by COURSE_MAP / NEXT_ACTION

- quantitative entry diagnostic — created in `ENTRY_DIAGNOSTIC.md`;
- fractions/ratios/percentages — diagnostic coverage;
- percentage versus percentage-point change — diagnostic coverage;
- one-step algebra — diagnostic coverage;
- scientific notation — diagnostic coverage;
- table/basic x-y reading — diagnostic coverage;
- mean-versus-median intuition — diagnostic coverage;
- probability 0–1/0–100% — diagnostic coverage;
- explicit P1 versus conditional P2-QB routing — defined;
- no learner deficit inferred before observed responses — explicit;
- variable types — covered;
- nominal/ordinal/interval/ratio measurement scales — covered with caveat against mechanical use;
- mean, median, mode — covered;
- range, variance, SD, IQR and quantiles — covered;
- distributions, symmetry/skew and outliers — covered;
- data visualization — dot/strip plots, histograms, boxplots, bar charts and scatterplots covered;
- misleading visual choices — axis truncation, hidden distribution, incompatible scales/areas/window selection covered;
- sample versus population — covered;
- parameter versus statistic — covered;
- sampling variability — covered conceptually;
- sample distribution versus sampling distribution — explicitly separated;
- SD versus SE — explicitly separated and calculated for simple means;
- sample-size intuition — quadruplicating n approximately halves mean SE when SD remains similar;
- transformations — introduced conceptually only;
- four-dataset summary-choice performance task — `EXERCISES.md` Part B;
- visualization audit — `EXERCISES.md` Part D;
- sample-size/variability reasoning — `EXERCISES.md` Parts E/F.

### Intentionally deferred

The unit does **not** teach in full:

- confidence intervals — F0.5;
- p-values/NHST — F0.5;
- effect-size interpretation — F0.5;
- smallest effect of interest — F0.5;
- formal power/sample-size planning — F0.6;
- Type I/II error — F0.6;
- multiplicity/analytical flexibility — F0.6;
- formal distribution theory/proofs;
- advanced transformation/model diagnostics.

This keeps F0.4 as the quantitative descriptive/sampling bridge rather than collapsing F0.5–F0.6 into it.

---

## 2. Quantitative entry diagnostic QA — PASS

The diagnostic has eight independently scorable 2-point domains:

1. fraction/decimal/percentage conversion;
2. ratio and relative change;
3. percentage versus percentage-point change;
4. one-step algebra;
5. scientific notation;
6. table/basic x-y reading;
7. mean versus median intuition;
8. probability scale conversion.

### Routing logic

`READY_FOR_F0.4`:

- 14–16/16;
- no zero domain.

`P1_REPAIR`:

- localized weakness with at least six domains showing some competence.

`P2-QB_REQUIRED`:

- <=9/16; or
- three or more zero domains; or
- fewer than six domains showing any competence.

This operationalizes the prerequisite graph's rule that structural failure means inability across a majority/broad set of basic operations rather than a single arithmetic mistake.

### State integrity

No diagnostic response exists in the repository. Therefore:

`F0.4 quantitative diagnostic = UNOBSERVED`

No learner-specific remediation state is assigned.

---

## 3. External source recheck — PASS

Research/check date: `2026-09-09`.

### `F0-S12` — NIST/SEMATECH e-Handbook

Current NIST pages were rechecked and remain available as the institutional statistical reference.

Relevant functions used in F0.4:

- exploratory data analysis;
- graphical examination of distributions;
- detection of outliers/anomalies;
- descriptive statistical concepts;
- distribution-aware interpretation.

The NIST context is engineering/general statistics, so the project supplies its own sports/exercise-flavored examples without presenting those examples as substantive nutrition evidence.

### `F0-S14` — ICH E9/E9(R1)

The EMA official page was rechecked on 2026-09-09.

Current status observed:

- ICH E9 Step 5 remains the adopted statistical-principles guideline;
- ICH E9(R1) estimands/sensitivity addendum remains Step 5/current;
- no new E9 replacement was located in the official current-version page.

F0.4 uses E9 only as a methodological boundary reminder that objectives, variables/endpoints, summaries and analyses must align. Regulatory drug-trial detail is not imported into a basic descriptive-statistics lesson.

### `F0-S27` — Altman & Bland, SD versus SE

BMJ Statistics Note rechecked on 2026-09-09:

- Altman DG, Bland JM. *Standard deviations and standard errors*. BMJ. 2005;331:903. doi:10.1136/bmj.331.7521.903.

Instructional function:

- direct separation of SD as variability of observations from SE as sampling variability/precision of an estimate;
- simple mean-SE relation `SE = SD/√n`;
- explicit warning against using SE to describe individual spread.

Although published in 2005, the distinction is mathematical/stable rather than a changing clinical recommendation. It is included because it precisely targets a major F0.4 misconception and remains available in BMJ.

No new source was added for decoration.

---

## 4. CONTENT_QA — PASS

Checked:

- categorical nominal versus ordinal is distinguished correctly;
- numerical discrete versus continuous is distinguished conceptually rather than by storage precision;
- interval versus ratio scales are taught as reasoning aids rather than automatic analysis rules;
- mean is not represented as universally superior;
- median is described as robust/resistant to extremes without claiming it is universally preferable;
- mode is allowed to be absent/non-unique;
- sample variance uses `n−1` in worked calculations and this choice is labeled as sample variance;
- SD is the square root of variance and returns to the original measurement unit;
- range is not conflated with IQR;
- quantile-convention differences in small samples are acknowledged;
- right skew is defined by tail shape, not by the non-universal mnemonic `mean > median`;
- outlier is not equated with data error;
- histogram is distinguished from bar chart;
- scatterplot association is not converted into causality;
- axis truncation is treated as a visual-scaling issue, not automatically forbidden;
- population, sample, parameter and statistic remain distinct;
- sampling variability is taught as expected variation across samples;
- sample distribution is values; sampling distribution is repeated-sample statistics;
- SE is defined as the SD of a sampling distribution;
- `SE(mean) ≈ s/√n` is used only with the stated simple independent-observation context;
- quadruplicating n → approximately half the mean SE when SD is similar;
- increasing n is not claimed to reduce SD or systematic bias;
- larger samples may exhibit larger range because more extreme values can be observed;
- transformations are represented as scale changes, not a method to erase bias or force acceptable results.

Worked arithmetic was independently checked.

---

## 5. EVIDENCE_QA — PASS

Safeguards:

- methodological/statistical claims use methodological sources rather than exercise/nutrition primary studies;
- no sports-nutrition example is treated as proof of a substantive intervention effect;
- no current clinical recommendation is made;
- NIST is used within its general statistical scope;
- ICH E9 is used only for alignment/statistical-principle context, with regulatory scope acknowledged;
- Altman/Bland is used for a stable mathematical distinction, not a clinical claim;
- F0.3 systematic-bias lessons are preserved when discussing why large n cannot cure bias;
- inferential claims about CI/p-values/power are deferred.

No cherry-picking problem applies to a contested intervention claim because F0.4 is methodological/foundational rather than a substantive treatment question.

---

## 6. PEDAGOGICAL_QA — PASS

### Prerequisites

- F0.1 remains the structural conceptual prerequisite;
- entry numeracy is measured through the diagnostic rather than assumed;
- isolated gaps route to P1;
- broad structural gaps route to conditional P2-QB only after observed responses.

### Progression

The lesson follows:

`data object → variable type → measurement scale → distribution → center → dispersion → skew/outliers → visualization → population/sample → parameter/statistic → sampling variation → sample vs sampling distribution → SD vs SE → sample-size intuition → transformations → worked examples → error rejection`

### Autossuficiência

Essential concepts and calculations are taught within the lesson. External sources provide traceability rather than outsourcing definitions.

### Anti-memorization

The assessment requires:

- selecting summaries for four structurally different datasets;
- calculating descriptive statistics;
- auditing misleading visualizations;
- explaining sample versus sampling distributions;
- predicting what changes when n changes;
- integrating descriptive choice with distribution shape.

---

## 7. MASTERY_QA — PASS

`EXERCISES.md` tests:

- `K1` — definitions/types;
- `K3` — compare mean/median, range/IQR, SD/SE, sample/sampling distributions;
- `K4` — interpret descriptive/visual evidence;
- `K5` — predict effect of outliers and larger n;
- `K6` — calculate and choose summaries;
- `K7` — integrate F0.3 bias boundary with sampling variation and visual interpretation;
- `K8` — identify limits/misleading summaries.

A learner cannot pass through term recognition alone because 80% of the assessment includes justification, calculation, visualization audit or integration.

### Critical-fail targets

Critical fails block progression when the learner:

- uses SE as individual variability;
- treats more n as automatic SD reduction;
- cannot separate sample from sampling distribution;
- automatically deletes outliers;
- reads magnitude from distorted visual scale alone;
- converts descriptive association into causality.

These are structural errors that would contaminate F0.5/F0.6.

---

## 8. Public repository/privacy QA — PASS

- no personal/health-identifying information;
- no learner response or deficit is recorded;
- all examples are synthetic/hypothetical;
- no third-party PDF is copied into the repository;
- only citations/links are registered;
- no individualized nutrition prescription is provided.

---

## 9. Production/learning-state separation — PASS

Production state:

`APPROVED`

Learning state remains:

- F0.1: pending/unvalidated;
- F0.2: pending/unvalidated;
- F0.3: pending/unvalidated;
- F0.4: `UNSEEN`;
- F0.4 quantitative diagnostic: `UNOBSERVED`.

No score is fabricated from material production.

---

## 10. Final gate

> Can a capable learner with the required numeracy bridge learn how to classify variables, choose defensible descriptive summaries/graphs, recognize skew/outliers, distinguish individual variability from sampling variability, explain SD versus SE and predict the consequences of increasing sample size without prematurely relying on CI/p-values/power?

**Decision:** yes — `APPROVED`.

NotebookLM packaging is outside `F0-A08` and should be produced only under the next canonical action.