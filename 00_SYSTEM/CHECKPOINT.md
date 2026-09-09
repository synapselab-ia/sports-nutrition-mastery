# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-09
**Canonical branch:** `main`
**Project state:** `F0_5_UNIT_APPROVED`

## Completed

### Project foundation

- public repository initialized;
- canonical `AGENTS.md` / `START_HERE.md` resume protocol established;
- project mission/scope, privacy/public-repository policy, evidence policy, research protocol, pedagogical standard, QA gates and mastery protocol created;
- NotebookLM protocol/manifest pattern created;
- macro curriculum, source registry/claim ledger and learner/mastery/error/study-history artifacts initialized;
- `F0-A01` completed: F0.1–F0.10 architecture, prerequisite graph and exit-assessment blueprint created.

### F0.1 — Scientific questions, hypotheses and operationalization

- `F0-A02` completed: approved instructional unit;
- `F0-A03` completed: approved NotebookLM package;
- canonical reasoning begins with `question → target population → contrast → outcome → time → estimand`;
- learner state remains unvalidated.

### F0.2 — Study designs and what they can answer

- `F0-A04` completed: approved instructional unit;
- `F0-A05` completed: approved NotebookLM package;
- design reasoning remains architecture-first and target-trial emulation remains a design benchmark rather than retroactive randomization;
- learner state remains unvalidated.

### F0.3 — Bias, confounding, causal reasoning and validity

- `F0-A06` completed: approved instructional unit;
- `F0-A07` completed: approved NotebookLM package;
- causal appraisal sequence remains `target causal question/estimand → causal structure → distortion mechanism → adjustment/conditioning → repairability/data limitation → calibrated conclusion`;
- DAGs encode assumptions and do not prove arrows;
- larger sample size is not represented as a cure for systematic bias;
- formal RoB 2/ROBINS-I/GRADE application remains deferred to F0.8;
- current `ROBINS-I V2` remains recorded as a draft posted 20 November 2025 and subject to change;
- learner state remains unvalidated.

### F0.4 — Descriptive statistics, distributions and sampling variation

- `F0-A08` completed: approved instructional unit plus quantitative entry diagnostic;
- `F0-A09` completed: approved NotebookLM package;
- canonical distinctions remain: variable meaning before summary; sample versus population; parameter versus statistic; sample distribution versus sampling distribution; SD versus SE; larger n can reduce SE without automatically reducing individual SD or systematic bias;
- first-pass NotebookLM corpus uses canonical lesson, NIST EDA, Altman/Bland SD-SE note and ICH E9/E9(R1);
- `ENTRY_DIAGNOSTIC.md`, independent exercises and answer key remain outside the initial NotebookLM corpus;
- F0.4 quantitative diagnostic remains `UNOBSERVED` because no learner response has been observed.

### F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance

#### `F0-A10` — instructional unit

- `F0-A10` completed: complete fifth instructional unit created and production QA passed;
- approved unit path: `foundations/F0-scientific-literacy/F0.5-estimates-confidence-pvalues-effect-sizes/`;
- verified canonical files:
  - `LESSON.md` — `APPROVED`;
  - `EXERCISES.md` — 100-point active-recall/application assessment;
  - `ANSWER_KEY.md` — commented scoring key;
  - `QA_REPORT.md` — CONTENT, EVIDENCE, PEDAGOGICAL and MASTERY gates passed;
- F0.5 begins by separating parameter, estimator and estimate, then point versus interval estimates;
- standard error is carried forward from F0.4 as uncertainty/precision of an estimate rather than individual spread;
- generic CI structure is introduced as `estimate ± critical value × SE`, with `1.96` explicitly restricted to a simple normal-approximation example rather than treated as universal;
- a frequentist 95% CI is taught as a repeated-sampling coverage property of the procedure under assumptions, not as a 95% posterior probability that the fixed parameter lies inside one observed interval;
- compatibility language is used cautiously: a CI identifies values relatively compatible with the data/model under assumptions, without claiming equal probability inside the interval or impossibility outside it;
- null value is explicitly scale-specific: `0` for difference measures and `1` for ratio measures;
- the six ASA p-value principles are taught explicitly and operationally;
- p-values are treated as model-conditional incompatibility measures, not probabilities that H0 is true, not effect magnitude and not practical importance;
- `p=0.049` versus `p=0.051` is not represented as a scientific discontinuity;
- binary significance labels are repeatedly replaced by direction + magnitude + precision + model/statistical output + practical threshold/context;
- mean difference (MD) and standardized mean difference (SMD) are separated; SMD labels such as small/medium/large are not treated as universal importance thresholds;
- binary effect measures explicitly distinguish risk difference (RD), risk ratio (RR), odds and odds ratio (OR);
- RR and OR are never treated as interchangeable;
- relative-effect interpretation requires absolute baseline context when practical meaning depends on baseline;
- the same `RR=0.50` is contrasted across `20%→10%` and `2%→1%` to show different absolute effects (`−10 pp` versus `−1 pp`);
- logarithmic-scale intuition for ratio measures is introduced only at P1 level: null `1`, reciprocal symmetry after log transformation, no manual log calculation required;
- smallest effect of interest / decision threshold is taught as a context-dependent, justifiable target rather than a universal statistical constant;
- CI interpretation is explicitly tied to practical zones/thresholds so the learner can distinguish:
  - statistically detectable but practically small effects;
  - imprecise results compatible with both trivial and relevant effects;
  - precise near-null results that can exclude effects considered important;
- “absence of evidence” is separated from sufficiently precise evidence excluding a prespecified meaningful magnitude;
- forest-plot reading uses the required six-block sequence `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`;
- the independent performance task includes both a synthetic continuous forest-plot row and a synthetic binary trial table;
- continuous integrated example was independently recalculated before publication: `MD=1.4`, `SE≈1.141`, normal-approximate 95% CI `≈−0.84 to +3.64`, two-sided p `≈0.22`;
- binary integrated example was independently recalculated: A `12/100`, B `20/100`, `RR=0.60`, log-RR 95% CI `≈0.31–1.16`, p `≈0.13`, RD point estimate `−8 percentage points`;
- critical-fail conditions block `p<0.05 = true/important`, `p>0.05 = no effect`, p-value as probability of H0/chance, frequentist CI as posterior probability, CI crossing null as proof of uselessness, CI excluding null as proof of importance, relative effects without baseline context, universal SMD importance labels, OR=RR and precision as a cure for systematic bias;
- local exercise gate is `>=80/100` plus no critical fail and applies only after observed learner performance;
- formal Type I/II-error operating characteristics, power calculations, multiplicity, FWER/FDR, analytical flexibility and prespecification machinery remain deliberately deferred to F0.6;
- no substantive sports-nutrition recommendation is made from the synthetic examples.

#### F0.5 source/version decisions

- `F0-S06` Cochrane Handbook Chapter 6 rechecked on 2026-09-09; current Handbook version remains v6.5 and the chapter page states last update August 2023; used for MD/SMD/RD/RR/OR scale logic;
- `F0-S08` ASA p-value statement rechecked on 2026-09-09 and all six official principles preserved in paraphrased form;
- `F0-S09` ASA 2021 Task Force rechecked on 2026-09-09; used to avoid both ritual thresholding and the false lesson that p-values are intrinsically useless;
- `F0-S12` NIST/SEMATECH rechecked for frequentist CI/repeated-sampling concepts;
- `F0-S13` Lakens 2022 rechecked and used only for smallest-effect/informativeness reasoning in F0.5; formal power/sample-size planning remains F0.6;
- `F0-S27` Altman & Bland remains the F0.4→F0.5 bridge for SD versus SE;
- new `F0-S28` added: Greenland et al. 2016, *Statistical tests, P values, confidence intervals, and power: a guide to misinterpretations*, used specifically for CI/p-value misinterpretation safeguards and compatibility language; open-access source status recorded;
- `SOURCE_INDEX.md` updated on 2026-09-09 with all F0.5 source checks and F0-S28.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.5 APPROVED`.

F0.1–F0.4 each have an approved instructional unit and approved NotebookLM package. F0.5 now has an approved instructional unit, independent assessment, commented answer key and production QA.

The F0.5 NotebookLM study package is the next production artifact.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from production activity.

## F0.5 canonical production decisions

- interpretation sequence is `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`;
- point estimate is never interpreted without its scale/context and, when available, interval uncertainty;
- CI precision is not causal validity;
- frequentist confidence level is a property of repeated-sampling procedure coverage, not posterior probability of the fixed parameter;
- p-values are model-conditional outputs and never probability statements about H0;
- binary significance categories are insufficient summaries;
- p-value does not measure effect magnitude or practical importance;
- MD remains in original units; SMD standardizes by a dispersion quantity and is not automatically clinically/practically meaningful;
- RD is absolute; RR and OR are relative ratio measures with null `1`; RR and OR remain distinct;
- practical interpretation of relative effects requires baseline absolute context;
- smallest effect of interest/decision threshold is contextual and should be justified rather than inferred from the observed p-value;
- precise near-zero estimates can be informative when they exclude prespecified meaningful magnitudes;
- wide CIs crossing the null can remain compatible with important benefit/harm and must not be summarized as “no effect”;
- systematic bias, design validity and applicability remain separate from statistical precision;
- formal power/multiplicity/analytical-flexibility machinery remains F0.6.

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner;
- F0.2 has not yet been studied or assessed by the learner;
- F0.3 has not yet been studied or assessed by the learner;
- F0.4 has not yet been studied or assessed by the learner;
- F0.4 quantitative diagnostic = `UNOBSERVED`;
- F0.5 has not yet been studied or assessed by the learner;
- approved NotebookLM guides exist for F0.1–F0.4;
- no mastery-state change is authorized from curriculum/package production alone.

## Operational constraints

- repository is public;
- never persist sensitive personal/health data;
- do not publish copyrighted PDFs/chapters without redistribution permission;
- current methodological claims must be researched and sourced;
- NotebookLM is a study layer; GitHub remains canonical;
- living/versioned sources must be rechecked when materially relevant;
- answer keys and prerequisite diagnostics must not contaminate first-pass retrieval/assessment;
- synthetic sports/nutrition numerical examples must not become substantive nutrition recommendations;
- production can proceed while learner validation remains pending, but F0.5 learner validation requires F0.4 as P2 and F0.6 learner validation requires F0.4 + F0.5;
- F0.4 diagnostic remains `UNOBSERVED` until actual learner responses are produced.

## NEXT_ACTION

`F0-A11` — Produce the complete NotebookLM study package for `F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance`. Create `notebooklm/F0.5-estimates-confidence-pvalues-effect-sizes/MANIFEST.md`, `STUDY_GUIDE.md` and package `QA_REPORT.md` using the approved F0.5 lesson and a deliberately limited, auditable source corpus drawn only from sources needed for the learning objectives. Assign `CORE`/`SUPPORT`/`CONTRAST` roles and explain the instructional function and limitation of every source. The package must repeatedly enforce `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`; require correct frequentist CI interpretation without posterior-probability language; require all six ASA p-value principles and explicit repair of common p-value errors; contrast MD/SMD and RD/RR/OR; require absolute baseline context for relative effects; use smallest-effect/decision-threshold reasoning to distinguish imprecision, practically trivial effects and precise exclusion of meaningful effects; and include forest-plot-row plus synthetic trial-table practice. Preserve the F0.4 SD-versus-SE distinction and keep formal Type I/II error, power, multiplicity and analytical-flexibility machinery deferred to F0.6. Exclude F0.5 `EXERCISES.md` and `ANSWER_KEY.md` from the initial NotebookLM corpus so independent assessment remains uncontaminated; exclude the F0.4 entry diagnostic as well and preserve its state as `UNOBSERVED`. Recheck all external source links/version status used in the manifest, apply STUDY PACKAGE QA and copyright/public-repository controls, preserve F0.1–F0.5 learner states as pending, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.
