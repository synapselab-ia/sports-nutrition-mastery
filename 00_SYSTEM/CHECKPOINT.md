# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-10
**Canonical branch:** `main`
**Project state:** `F0_9_UNIT_APPROVED`

## Completed

### Project foundation

- public repository initialized;
- canonical `AGENTS.md` / `START_HERE.md` resume protocol established;
- project mission/scope, privacy/public-repository policy, evidence policy, research protocol, pedagogical standard, QA gates and mastery protocol created;
- NotebookLM protocol/manifest pattern created;
- macro curriculum, prerequisite graph, assessment blueprint, source registry/claim ledger and learner/mastery/error/study-history artifacts initialized;
- `F0-A01` completed: F0.1–F0.10 architecture and exit-assessment blueprint established.

### F0.1 — Scientific questions, hypotheses and operationalization

- `F0-A02` completed: approved instructional unit;
- `F0-A03` completed: approved NotebookLM package;
- canonical reasoning begins `question → target population → contrast → outcome → time → estimand`;
- learner state remains unvalidated.

### F0.2 — Study designs and what they can answer

- `F0-A04` completed: approved instructional unit;
- `F0-A05` completed: approved NotebookLM package;
- design reasoning is architecture-first; target-trial emulation is a benchmark rather than retroactive randomization;
- learner state remains unvalidated.

### F0.3 — Bias, confounding, causal reasoning and validity

- `F0-A06` completed: approved instructional unit;
- `F0-A07` completed: approved NotebookLM package;
- causal appraisal remains `target causal question/estimand → causal structure → distortion mechanism → adjustment/conditioning → repairability/data limitation → calibrated conclusion`;
- DAGs encode assumptions and do not prove arrows;
- learner state remains unvalidated.

### F0.4 — Descriptive statistics, distributions and sampling variation

- `F0-A08` completed: approved instructional unit plus quantitative entry diagnostic;
- `F0-A09` completed: approved NotebookLM package;
- canonical distinctions include sample/population, parameter/statistic, sample distribution/sampling distribution and SD/SE;
- larger n may reduce SE without reducing individual SD or systematic bias;
- F0.4 quantitative diagnostic remains `UNOBSERVED`.

### F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance

- `F0-A10` completed: approved instructional unit, independent assessment, answer key and production QA;
- `F0-A11` completed: approved NotebookLM package;
- canonical interpretation remains `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`;
- frequentist CI is not posterior probability; p-value is not `P(H0|data)` and does not measure importance;
- learner state remains unvalidated.

### F0.6 — Power, Type I/II error, multiplicity and analytical flexibility

- `F0-A12` completed: approved instructional unit, 100-point assessment, answer key and production QA;
- `F0-A13` completed: approved NotebookLM package;
- power remains prospective/effect-design-assumption dependent rather than probability that H1 is true;
- observed/post hoc power is not a completed-study interpretation tool;
- multiplicity includes endpoints, timepoints, subgroups, models/paths and data-dependent choices;
- prespecification improves auditability but does not guarantee validity;
- learner state remains unvalidated.

### F0.7 — Systematic reviews, meta-analyses and heterogeneity

- `F0-A14` completed: approved instructional unit, 100-point assessment, answer key and production QA;
- `F0-A15` completed: approved NotebookLM package;
- systematic review and meta-analysis remain distinct; pooling is optional and compatibility-dependent;
- inverse-variance weight is precision, not quality/certainty;
- fixed-effect/random-effects target different model-dependent quantities;
- random effects does not solve heterogeneity;
- pooled CI is not between-study effect spread;
- clinical, methodological and statistical heterogeneity remain separate;
- I² is not a quality/sameness/automatic-invalidity score;
- subgroup/meta-regression/sensitivity analyses preserve F0.6 prespecification/multiplicity safeguards;
- funnel/small-study signals remain non-diagnostic for publication/non-reporting bias;
- PRISMA remains reporting guidance rather than RoB/certainty certification;
- learner state remains unvalidated.

### F0.8 — Risk of bias, certainty of evidence and applicability

#### `F0-A16` — instructional unit

- `F0-A16` completed: approved unit at `foundations/F0-scientific-literacy/F0.8-risk-of-bias-certainty-applicability/`;
- verified files: `LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md`, production `QA_REPORT.md`;
- reporting completeness, broad critical appraisal, result-level risk of bias, body/outcome certainty, applicability/transportability and recommendation strength are separate objects;
- RoB judgments are result-specific/domain-based rather than total study-quality scores;
- randomized design does not automatically certify low risk of bias;
- non-randomized evidence requires explicit confounding/selection reasoning but is not dismissed by label;
- RoB 2 for individually randomized parallel-group trials remains current version `22 August 2019`;
- ROBINS-I V2 remains the revised **draft posted 20 November 2025**, subject to change;
- GRADE certainty remains body/outcome/question specific and threshold/range aware;
- four certainty categories remain `High`, `Moderate`, `Low`, `Very low`;
- five core downgrading domains taught are risk of bias, inconsistency, indirectness, imprecision and dissemination/publication/non-reporting bias;
- F0.5 magnitude/CI/threshold reasoning is mandatory for imprecision;
- F0.7 heterogeneity/missing-evidence reasoning is mandatory for inconsistency/dissemination-bias judgments;
- applicability compares evidence versus target population/intervention or exposure/comparator/outcome/time/setting/decision context;
- internal validity and applicability are not interchangeable;
- certainty of one outcome is distinct from recommendation strength;
- required audit sequence has 13 fields: `Target question/outcome → Reporting visibility → Design/effect of interest → Result-level RoB mechanisms → RoB judgment/rationale → Body estimate + threshold → Inconsistency → Indirectness → Imprecision → Missing/dissemination evidence → Overall certainty → Applicability to target → Recommendation-strength boundary`;
- local assessment gate remains `>=80/100 + no critical fail`, applicable only after observed learner performance.

#### `F0-A17` — NotebookLM study package

- `F0-A17` completed: approved F0.8 NotebookLM package created at `notebooklm/F0.8-risk-of-bias-certainty-applicability/`;
- verified canonical files: `MANIFEST.md`, `STUDY_GUIDE.md`, `QA_REPORT.md`;
- package decision: `PASS — READY_FOR_STUDY`;
- first-pass corpus is intentionally limited to exactly six sources: canonical F0.8 lesson, riskofbias.info, GRADE overview, GRADE intervention-certainty principles, GRADE indirectness and STROBE as reporting-versus-quality contrast;
- package creation changed no learner state and did not change the F0.4 quantitative diagnostic.

### F0.9 — Critical reading of a complete paper

#### `F0-A18` — instructional unit

- `F0-A18` completed: complete ninth instructional unit created and production QA passed;
- approved unit path: `foundations/F0-scientific-literacy/F0.9-critical-reading-complete-paper/`;
- verified canonical files on `main`:
  - `LESSON.md` — `APPROVED`;
  - `EXERCISES.md` — 100-point independent assessment;
  - `ANSWER_KEY.md` — commented scoring key;
  - `QA_REPORT.md` — `PASS — APPROVED` across scope, CONTENT, EVIDENCE, PEDAGOGICAL and MASTERY gates;
- F0.9 requires the fixed full-paper sequence `Question/estimand → Design/sampling → Intervention/exposure/comparator → Outcome measurement → Bias/confounding/missingness → Sample size/analysis plan → Effect estimate/uncertainty → Multiplicity/exploration → Result robustness → Applicability → Consistency with authors’ conclusion → What the paper does not establish`;
- article anatomy, supplements, registry/protocol/SAP, data/code repositories, provenance and publication timeline are taught as navigation/audit objects rather than validity scores;
- the learner must extract a compact PICO/estimand table and a result table before accepting narrative interpretation;
- F0.1–F0.8 are explicitly integrated rather than replaced by a new checklist;
- within-group change is explicitly separated from between-group treatment effect;
- `p>0.05` is explicitly not treated as proof of no effect or equivalence;
- post-study/observed-power calculations are not allowed to rescue a completed-study interpretation; estimate + CI + practical threshold + design/bias remain primary;
- multiplicity and prespecification require a timeline comparison of study conduct against registry/protocol/SAP timestamps;
- retrospective registration can improve transparency but cannot prove prospective prespecification;
- result robustness is separated from result-shopping, and data/code sharing is treated as auditability rather than automatic validity;
- applicability is audited across population, intervention/exposure, comparator, outcome, time, setting and decision context;
- single-paper appraisal is explicitly separated from body-of-evidence GRADE certainty;
- reporting guidelines remain maps for locating information rather than validity/quality scores;
- local assessment gate is `>=80/100 + no critical fail`; checklist-only responding is capped at 60/100;
- the blind performance task uses `F0-S30`, Klemp et al. 2025, a legally accessible human randomized exercise/nutrition trial, with `F0-S31` ClinicalTrials.gov `NCT05922475` as the registry/timeline companion;
- `F0-S30` is open access under CC BY 4.0; no article full text, figure, table or third-party PDF was copied into the repository;
- the selected trial provides a nontrivial appraisal case: 12-week three-arm resistance-training study in older previously untrained men; 32 randomized/enrolled and 30 completed/analyzed; post-exercise protein, pre-sleep protein and training-only conditions; multiple muscle-thickness/strength outcomes and timepoints; mixed-effects analysis; reported longitudinal CIs; retrospective registry; named OSF data repository; and a post-study sensitivity-power analysis;
- the performance task requires distinguishing PRP-versus-PSP timing from supplemented-versus-training-only contrasts, recognizing that the latter also changes nutrient/energy exposure;
- the answer key distinguishes reported improvements over time from evidence that one intervention group outperformed another and does not invent unreported between-group CIs;
- the study reports no statistically significant group-related differences, but the module rejects converting that into formal equivalence without direct uncertainty relative to a defensible margin/threshold;
- trial registry timing was verified: study start September 2017, completion May 2019, first submission/posting in 2023; therefore the public registry is retrospective for the completed trial;
- the paper reports these data as a subset of a larger project with additional outcomes; this is treated as a selection/multiplicity opportunity requiring audit, not proof of selective reporting;
- applicability to trained competitive athletes is deliberately limited by age, sex, training status, baseline dietary context, training dose, specific supplement product/dose, outcomes and duration;
- critical fails explicitly include abstract-only appraisal, design-label-only appraisal, checklist-as-validity, binary p-value reasoning, observed-power rescue, ignoring multiplicity/prespecification, reporting=low RoB, one paper-level RoB/certainty shortcut, within-group-as-treatment-effect, unsupported acute/mechanistic extrapolation, copying authors’ conclusion without reconstruction, inventing missing information and assigning one paper a body-level GRADE rating.

#### F0.9 source/version decisions

- current methodological sources actually used were rechecked on 2026-09-10;
- `F0-S01` CONSORT 2025 remains the current general randomized-trial reporting standard with a 30-item checklist; it is used for reporting visibility/navigation only, never as a validity score;
- `F0-S07` riskofbias.info recheck confirmed RoB 2 for individually randomized parallel-group trials remains version `22 August 2019`; licensed tool documents were not republished;
- `F0-S18` GRADE Book overview remains last modified `12 May 2026` and continues to separate body-level certainty from recommendation strength;
- `F0-S19` intervention-certainty principles remain last modified `21 August 2025` and continue threshold/range-aware body/outcome reasoning;
- `F0-S30` and `F0-S31` were added to `SOURCE_INDEX.md` because they are actually used in the F0.9 performance task;
- `SOURCE_INDEX.md` was advanced to `Last researched: 2026-09-10`;
- no other new source ID was created;
- no third-party full text was persisted.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.9 APPROVED`.

F0.1–F0.8 have approved instructional units and approved NotebookLM study packages.

F0.9 now has:

- approved self-contained integration lesson;
- 100-point independent assessment with a blind full-paper task;
- commented answer key;
- approved production QA;
- registered full-paper and registry sources (`F0-S30`, `F0-S31`).

The F0.9 NotebookLM study package is the next production artifact. F0.10 remains deferred until that package is complete.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from production activity.

## F0.9 canonical production decisions

- never appraise a paper from title/abstract alone;
- extract the PICO/estimand and result table before narrative interpretation;
- design labels inform appraisal but do not complete it;
- reporting guidelines locate information and are not quality/validity scores;
- temporal evidence determines whether registration/protocol/SAP can support prospective-prespecification claims;
- retrospective registration improves transparency but cannot establish prospectivity;
- within-group change and between-group treatment effect are separate objects;
- nonsignificance and equivalence are separate claims;
- completed-study interpretation uses estimate + CI + practical threshold + design/bias, not observed/post hoc power;
- multiplicity concerns the available claim/analysis family, not one highlighted p-value;
- risk-of-bias reasoning remains result-specific;
- robustness is not result-shopping and open data do not retroactively fix design;
- applicability is a target-context comparison independent of internal validity;
- single-paper appraisal is not a body-of-evidence certainty rating;
- every appraisal ends with strongest defensible inference, authors’ conclusion audit and explicit boundaries on what the paper does not establish;
- the F0.9 blind performance paper is `F0-S30` with `F0-S31` as registry/timeline companion.

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner;
- F0.2 has not yet been studied or assessed by the learner;
- F0.3 has not yet been studied or assessed by the learner;
- F0.4 has not yet been studied or assessed by the learner;
- F0.4 quantitative diagnostic = `UNOBSERVED`;
- F0.5 has not yet been studied or assessed by the learner;
- F0.6 has not yet been studied or assessed by the learner;
- F0.7 has not yet been studied or assessed by the learner;
- F0.8 has not yet been studied or assessed by the learner;
- F0.9 has not yet been studied or assessed by the learner;
- approved NotebookLM guides exist for F0.1–F0.8;
- no mastery-state change is authorized from curriculum production alone.

## Operational constraints

- repository is public;
- never persist sensitive personal/health data;
- do not publish copyrighted PDFs/chapters/articles without redistribution permission;
- current methodological claims must be researched and sourced;
- NotebookLM is a study layer; GitHub remains canonical;
- living/versioned sources must be rechecked when materially relevant;
- answer keys and prerequisite diagnostics must not contaminate first-pass retrieval/assessment;
- the real F0.9 performance paper may be linked as legally accessible source, but the project does not need to republish its full text;
- production can proceed while learner validation remains pending;
- F0.9 learner validation requires F0.1–F0.8 as P2;
- F0.10 learner validation requires F0.5 + F0.7 + F0.8 + F0.9;
- F0.4 diagnostic remains `UNOBSERVED` until actual learner responses are produced.

## NEXT_ACTION

`F0-A19` — Produce the complete NotebookLM study package for `F0.9 — Critical reading of a complete paper`. Create `notebooklm/F0.9-critical-reading-complete-paper/MANIFEST.md`, `STUDY_GUIDE.md` and package `QA_REPORT.md` using the approved F0.9 lesson and a deliberately limited, auditable corpus. The initial corpus must include the canonical F0.9 lesson, the legally accessible `F0-S30` full paper and its `F0-S31` trial-registry record, plus only the minimum methodological support needed to preserve reporting-versus-validity, result-specific RoB, completed-study uncertainty/power and single-paper-versus-body-certainty boundaries. Assign `CORE`/`SUPPORT`/`CONTRAST` roles and explain every source’s instructional function and limitation. The package must train the fixed 12-step F0.9 appraisal sequence; article/supplement/registry/protocol/SAP/data navigation; provenance and version/timeline checks; PICO/estimand extraction; result-table extraction; within-group versus between-group inference; magnitude/CI/practical-threshold reasoning; rejection of `p>0.05 = equivalence` and observed-power rescue; multiplicity/prespecification classification using timestamps; result-specific bias mechanisms without total quality scores; robustness versus result-shopping; applicability across population/intervention/comparator/outcome/time/setting/context; authors’ conclusion proportionality; and explicit `what the paper does not establish` boundaries. Use the Klemp paper as a guided full-paper study object without embedding the completed blind-assessment answer key into the initial notebook corpus. Keep F0.9 `EXERCISES.md` and `ANSWER_KEY.md` outside the initial NotebookLM corpus so independent assessment remains uncontaminated; keep F0.4 `ENTRY_DIAGNOSTIC.md` outside and preserve it as `UNOBSERVED`. Recheck every external source/link/version actually used in the manifest, apply STUDY PACKAGE QA plus copyright/public-repository controls, preserve F0.1–F0.9 learner states as pending, keep F0.10 production deferred, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.