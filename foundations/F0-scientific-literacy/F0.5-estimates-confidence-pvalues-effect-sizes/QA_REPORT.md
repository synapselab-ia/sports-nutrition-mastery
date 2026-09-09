# F0.5 — Production QA report

**Unit:** `F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance`

**Reviewed:** 2026-09-09

**Production decision:** `APPROVED`

This report records production QA only. It does **not** record that the learner studied F0.5 and does not alter any mastery state.

---

## 1. Scope gate — PASS

Required by `COURSE_MAP.md` / `F0-A10`:

- point estimate versus interval estimate — covered;
- parameter/estimator/estimate distinction — covered;
- frequentist confidence-interval meaning — covered;
- common CI misinterpretations — covered;
- p-value definition — covered;
- all six ASA principles — covered explicitly;
- magnitude/precision versus binary significance — central teaching spine;
- raw mean difference — covered;
- standardized mean difference — covered with anti-label caveat;
- risk difference — covered;
- risk ratio — covered;
- odds and odds ratio — covered;
- absolute versus relative effects — covered with paired baseline examples;
- ratio/log-scale intuition — P1 bridge included;
- smallest effect of interest / decision threshold — covered;
- statistical versus practical importance — covered;
- compatibility/range-of-effects reasoning — covered;
- CI not converted into Bayesian posterior probability — explicit critical fail;
- SD versus SE distinction from F0.4 preserved;
- standard error used as uncertainty input without reteaching F0.4 as formula-only content;
- forest-plot-row performance task — included;
- synthetic trial-table performance task — included;
- every performance task separates direction, magnitude, precision, statistical output, practical meaning and unsupported claims;
- formal Type I/II error, power, multiplicity and analytical-flexibility machinery — deferred to F0.6.

No required element is missing.

---

## 2. External source recheck — PASS

Verification date: `2026-09-09`.

### `F0-S06` — Cochrane Handbook Chapter 6

Current Cochrane page verified:

- Chapter 6: *Choosing effect measures and computing estimates of effect*;
- Cochrane Handbook version 6.5 (2024);
- chapter page states last updated August 2023;
- current key points distinguish continuous and dichotomous outcome measures and identify mean difference, standardized mean difference, risk difference, risk ratio and odds ratio as distinct effect measures.

Instructional use in F0.5:

- effect-measure definitions and scale;
- difference versus ratio measures;
- raw versus standardized continuous effects;
- absolute versus relative binary effects.

Limitation preserved: Cochrane is written for systematic-review/evidence-synthesis work and contains analysis detail beyond F0.5.

### `F0-S08` — ASA Statement on p-values

Official ASA PDF and current ASA statement index remain accessible.

The six principles were directly rechecked on the official ASA PDF:

1. p-values can indicate incompatibility of data with a specified statistical model;
2. p-values do not provide the probability that the studied hypothesis is true or that chance alone produced the data;
3. scientific/business/policy conclusions should not depend only on crossing a p-value threshold;
4. proper inference requires full reporting/transparency;
5. p-value/statistical significance does not measure effect size or importance;
6. p-value alone is not a sufficient measure of evidence regarding a model/hypothesis.

F0.5 paraphrases these principles rather than reproducing the statement as a substitute for teaching.

### `F0-S09` — ASA 2021 Task Force

Current ASA-hosted page remains accessible.

Instructional use:

- p-values/significance tests remain useful tools when properly applied;
- sound inference requires uncertainty, variability, multiplicity, replicability and context;
- F0.5 therefore rejects both ritual thresholding and the simplistic claim that p-values must never be used.

Formal multiplicity mechanics remain deferred to F0.6.

### `F0-S12` — NIST/SEMATECH e-Handbook

Current NIST confidence-interval pages remain accessible.

The handbook explicitly presents confidence level as a repeated-sampling coverage property: repeated intervals constructed by the procedure cover the true parameter at the nominal long-run rate under assumptions.

Instructional use:

- frequentist CI construction intuition;
- standard error as a precision component;
- repeated-sampling interpretation.

The lesson does not adopt the potentially misleading shortcut that the fixed parameter has a 95% probability of lying inside one observed frequentist interval.

### `F0-S13` — Lakens 2022

Current open article verified at University of California Press.

Instructional use:

- informational value should follow inferential goals;
- smallest effect size of interest / decision-relevant effect concept;
- precision can be planned around effects that matter rather than around statistical significance alone.

F0.5 uses only the threshold/informativeness concepts. Formal a-priori power/sample-size calculations remain F0.6.

### `F0-S27` — Altman & Bland, SD versus SE

Current BMJ article remains available.

Instructional use:

- preserve the F0.4 distinction between variability among observations (SD) and sampling variability/precision of an estimate (SE);
- support the bridge from SE to interval estimation.

### `F0-S28` — Greenland et al. 2016

Open-access peer-reviewed methods article verified through PMC:

- Greenland S, Senn SJ, Rothman KJ, et al. *Statistical tests, P values, confidence intervals, and power: a guide to misinterpretations*. Eur J Epidemiol. 2016;31:337-350. doi:10.1007/s10654-016-0149-3;
- PMCID `PMC4877414`;
- article is distributed under CC BY 4.0;
- it catalogues common misinterpretations of p-values, CIs and power and emphasizes effect estimates/confidence limits over binary significance classification.

Instructional use:

- block probability-reversal errors;
- reinforce frequentist CI coverage logic;
- reinforce “compatibility” language without treating all points as equally probable;
- distinguish a large p-value from evidence that the null is true.

No copyrighted third-party full text was copied into the repository.

---

## 3. CONTENT_QA — PASS

### Parameters and estimates

Verified:

- parameter = target population/process quantity;
- estimator = rule/statistic used to estimate it;
- estimate = realized result in the observed data;
- point and interval estimates remain distinct.

### Confidence intervals

Verified:

- 95% confidence is assigned to long-run procedure coverage under assumptions;
- no posterior probability is assigned to the fixed parameter in the frequentist interpretation;
- CI is described as a range of parameter values relatively compatible with data/model, with explicit caveat that values are not equally probable;
- CI width is treated as precision information, not causal validity;
- systematic bias can remain despite a narrow CI.

### Standard error

Verified:

- SD and SE are not conflated;
- `estimate ± critical value × SE` is presented as a generic conceptual structure, not a universal exact formula;
- `1.96` is labeled as a normal approximation example rather than a constant for every estimator/design.

### P-values

Verified:

- p-value is conditioned on the specified model/test assumptions;
- p-value is not `P(H0 | data)`;
- p-value is not probability that chance generated the result;
- p small does not imply magnitude/practical importance;
- p large does not prove no effect;
- discontinuity at 0.05 is rejected;
- selective analysis/reporting is acknowledged as a validity threat and handed to F0.6.

### Effect measures

Verified calculations:

Continuous example:

- A=6.0, B=4.5 → MD=1.5;
- standardizing by SD=3.0 → SMD=0.50.

Binary example:

- A=12/100=0.12;
- B=20/100=0.20;
- RD=-0.08=-8 percentage points;
- RR=0.60;
- odds A=0.12/0.88≈0.136;
- odds B=0.20/0.80=0.25;
- OR≈0.545.

The lesson explicitly states RR ≠ OR.

### Baseline-risk examples

Verified:

- 20%→10%: RR=0.50, RD=-10 pp;
- 2%→1%: RR=0.50, RD=-1 pp.

Same relative effect, materially different absolute effect.

### Threshold reasoning

Verified:

- threshold is contextual and requires justification;
- it is not generated automatically from p-value/CI;
- examples distinguish intervals entirely above benefit threshold, entirely inside trivial zone and spanning multiple practical zones;
- “absence of evidence” is separated from precise exclusion of effects considered important.

### Integrated numeric examples

Continuous synthetic trial:

- A n=40, mean change 4.2, SD 5.0;
- B n=40, mean change 2.8, SD 5.2;
- MD=1.4;
- independent-means SE≈1.141;
- normal-approximate 95% CI≈[-0.84, 3.64];
- normal-approximate two-sided p≈0.22.

Binary synthetic trial:

- RR=0.60;
- approximate log-RR SE≈0.337;
- approximate 95% CI≈0.31–1.16;
- approximate two-sided p≈0.13.

Numbers were independently recalculated before publication.

---

## 4. EVIDENCE_QA — PASS

- statistical claims rely on statistical/methodological sources rather than exercise-nutrition intervention papers;
- all sports/nutrition-flavored examples are explicitly synthetic;
- no synthetic number is converted into a nutrition recommendation;
- effect size is not treated as causal evidence independent of design/bias;
- p-value is not treated as evidential certainty;
- confidence-interval precision is not represented as protection from confounding/selection/measurement bias;
- standardized effects are not assigned universal importance labels;
- relative measures are not interpreted without absolute baseline context when practical meaning depends on baseline;
- scope and limitations of each source are preserved.

No cherry-picking issue exists for a substantive intervention claim because the unit is methodological rather than a treatment recommendation.

---

## 5. PEDAGOGICAL_QA — PASS

### Prerequisite integrity

P2 = F0.4.

The lesson assumes but briefly reconnects:

- sample/population;
- parameter/statistic;
- sampling variability;
- SD versus SE.

It does not re-teach F0.4 as rote formula memorization.

### Progression

The lesson follows:

`parameter/estimate → point/interval → SE/CI → frequentist meaning → null scales → p-value → ASA principles → effect size → continuous measures → binary measures → absolute/relative → log-ratio intuition → practical threshold → compatibility → forest/trial interpretation → integrated limits`

This is concept-first, not threshold-first.

### Anti-memorization

Exercises require:

- repairing false statements;
- effect-measure calculations;
- comparing narrow/wide CIs;
- interpreting same RR at different baselines;
- applying practical thresholds;
- producing structured forest-plot and trial-table appraisals.

A learner cannot pass by listing definitions alone.

---

## 6. MASTERY_QA — PASS

`EXERCISES.md` tests:

- `K1` — parameter/estimate/CI/p/effect-measure definitions;
- `K3` — MD vs SMD, RD vs RR vs OR, narrow vs wide CI;
- `K4` — forest/trial statistical interpretation;
- `K5` — predict how different precision/baseline changes interpretation;
- `K6` — calculate effect measures;
- `K7` — integrate F0.1 question, F0.3 bias and F0.4 sampling logic with F0.5 uncertainty;
- `K8` — identify unsupported probability, significance and practical-importance claims.

Local gate:

`>=80/100 + no critical fail`.

This gate affects learning state only after actual observed performance.

### Critical-fail coverage

The assessment explicitly blocks:

- `p<0.05 = true/important`;
- `p>0.05 = no effect`;
- p-value as probability of H0/chance;
- 95% CI as 95% posterior probability;
- CI-crosses-null = useless;
- CI-excludes-null = important;
- relative effect without baseline context;
- SMD universal importance labels;
- OR treated as RR;
- precision treated as cure for systematic bias.

---

## 7. F0.5 → F0.6 boundary QA — PASS

F0.5 permits only the minimum conceptual bridge that:

- sample size/SE affect precision;
- multiple/selected analyses can affect p-value interpretation;
- p-values are part of repeated-use statistical procedures.

F0.5 deliberately does **not** teach formal:

- alpha/beta operating characteristics;
- Type I/II error calculations;
- power formulas;
- post hoc observed power critique in depth;
- multiplicity corrections;
- FWER/FDR;
- endpoint hierarchy algorithms;
- subgroup multiplicity;
- sequential testing;
- preregistration/SAP mechanics.

These remain canonical F0.6 content.

---

## 8. Public repository/privacy/copyright QA — PASS

- no personal, clinical or health-identifying learner data;
- no learner attempt is fabricated;
- all numerical examples are synthetic;
- no third-party PDF/full chapter is committed;
- repository contains only project-authored Markdown, citations and links;
- open-access/source-license status is recorded where relevant;
- no individualized nutrition prescription exists.

---

## 9. Production/learning-state separation — PASS

After F0-A10 production:

- F0.1 learner state remains pending/unvalidated;
- F0.2 remains pending/unvalidated;
- F0.3 remains pending/unvalidated;
- F0.4 remains pending/unvalidated;
- F0.4 quantitative diagnostic remains `UNOBSERVED`;
- F0.5 learning state remains `UNSEEN`.

No module is promoted from content production.

---

## 10. Final gate

> Can a capable learner who has the F0.4 prerequisite interpret a point estimate, confidence interval, p-value and major continuous/binary effect measures; distinguish magnitude from precision and statistical output from practical importance; use a defensible decision threshold; and reject common CI/p-value errors without prematurely requiring F0.6 power/multiplicity machinery?

**Decision:** yes.

**Production state:** `APPROVED`.

NotebookLM packaging is not part of F0-A10 and must be produced only by a subsequent canonical action.
