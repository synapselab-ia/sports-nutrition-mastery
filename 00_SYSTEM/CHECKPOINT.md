# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-10
**Canonical branch:** `main`
**Project state:** `F0_10_STUDY_PACKAGE_READY`

## Project foundation

- public repository initialized;
- canonical `AGENTS.md` / `START_HERE.md` resume protocol established;
- project mission/scope, evidence/research/privacy policies, pedagogical standard, QA gates and mastery protocol established;
- GitHub remains canonical; NotebookLM is a controlled study layer;
- production and learner validation remain separate;
- repository production must not persist private health data, secrets or non-redistributable third-party full text.

## Completed F0 production

### F0.1 — Scientific questions, hypotheses and operationalization

- `F0-A02` instructional unit approved;
- `F0-A03` NotebookLM package ready;
- canonical reasoning begins `question → target population → contrast → outcome → time → estimand`.

### F0.2 — Study designs and what they can answer

- `F0-A04` instructional unit approved;
- `F0-A05` NotebookLM package ready;
- design reasoning remains architecture-first rather than evidence-pyramid scoring.

### F0.3 — Bias, confounding, causal reasoning and validity

- `F0-A06` instructional unit approved;
- `F0-A07` NotebookLM package ready;
- causal appraisal remains `target causal question/estimand → causal structure → distortion mechanism → adjustment/conditioning → repairability/data limitation → calibrated conclusion`;
- DAGs encode assumptions rather than proving arrows.

### F0.4 — Descriptive statistics, distributions and sampling variation

- `F0-A08` instructional unit and quantitative entry diagnostic approved;
- `F0-A09` NotebookLM package ready;
- sample/population, parameter/statistic, sample distribution/sampling distribution and SD/SE remain distinct;
- quantitative diagnostic remains `UNOBSERVED`.

### F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance

- `F0-A10` instructional unit, independent assessment, answer key and production QA approved;
- `F0-A11` NotebookLM package ready;
- canonical interpretation remains `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`;
- significance is not practical importance and p-value is not posterior probability of a hypothesis.

### F0.6 — Power, Type I/II error, multiplicity and analytical flexibility

- `F0-A12` instructional unit/assessment/answer key/QA approved;
- `F0-A13` NotebookLM package ready;
- power remains prospective and conditional on effect/design/assumptions;
- observed/post-hoc power is not a completed-study interpretation tool;
- multiplicity includes outcomes, timepoints, subgroups, models and data-dependent analytical paths;
- prespecification improves auditability without guaranteeing validity.

### F0.7 — Systematic reviews, meta-analyses and heterogeneity

- `F0-A14` instructional unit/assessment/answer key/QA approved;
- `F0-A15` NotebookLM package ready;
- systematic review and meta-analysis remain distinct;
- pooling is compatibility-dependent and optional;
- inverse-variance weight is precision, not quality/certainty;
- fixed/random-effects target model-dependent quantities;
- random effects does not solve heterogeneity;
- clinical, methodological and statistical heterogeneity remain separate;
- I² is not a quality/sameness/automatic-invalidity score;
- subgroup/meta-regression/sensitivity reasoning preserves F0.6 multiplicity/prespecification safeguards;
- funnel/small-study signals are not diagnostic proof of publication bias.

### F0.8 — Risk of bias, certainty of evidence and applicability

- `F0-A16` instructional unit/assessment/answer key/QA approved;
- `F0-A17` NotebookLM package ready;
- reporting completeness, critical appraisal, result-level RoB, body/outcome certainty, applicability and recommendation strength remain separate objects;
- RoB is result-specific/domain-based, not a total quality score;
- randomized does not automatically mean low risk; observational does not automatically mean unusable;
- GRADE certainty is body/outcome/question specific and range/threshold aware;
- certainty is not effect magnitude;
- internal validity and applicability remain separate;
- certainty of one outcome does not determine recommendation strength.

### F0.9 — Critical reading of a complete paper

- `F0-A18` instructional unit/100-point assessment/answer key/QA approved;
- `F0-A19` NotebookLM package ready;
- fixed appraisal sequence remains `Question/estimand → Design/sampling → Intervention/exposure/comparator → Outcome measurement → Bias/confounding/missingness → Sample size/analysis plan → Effect estimate/uncertainty → Multiplicity/exploration → Result robustness → Applicability → Consistency with authors’ conclusion → What the paper does not establish`;
- PICO/estimand and result extraction precede narrative interpretation;
- within-group change is not between-group treatment effect;
- nonsignificance is not equivalence;
- registry/protocol/SAP timestamps determine what can be claimed about prespecification;
- reporting visibility is not validity;
- single-paper appraisal is not body-level certainty;
- blind performance source remains `F0-S30` with `F0-S31` registry companion; its full text is not republished in GitHub.

### F0.10 — Synthesis and communication of uncertainty

#### `F0-A20` — instructional unit

- `F0-A20` completed and approved at `foundations/F0-scientific-literacy/F0.10-synthesis-communication-uncertainty/`;
- verified files: `LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md`, production `QA_REPORT.md`;
- production QA decision: `PASS — APPROVED`;
- canonical workflow is `reconstructed evidence → invariant core → calibrated claim → audience translation → drift audit → update conditions`;
- invariant core has eight fields: `Target → Direction → Magnitude → Precision → Threshold → Certainty → Applicability → Boundaries/update conditions`;
- estimate + CI/range + practical threshold remain connected;
- `did not detect`, `evidence compatible with no meaningful effect` and formal equivalence are distinct claims;
- p-values do not determine truth, importance or absence;
- certainty is distinct from magnitude;
- uncertainty mechanisms remain separated as bias, imprecision, inconsistency, indirectness and missing/dissemination evidence;
- direct evidence can remain biased; low-RoB evidence can remain indirect;
- conflicting literature is weighted by claim fit/design/bias/magnitude/precision/directness/synthesis context rather than counted;
- avoiding false balance does not authorize a mechanical evidence pyramid;
- mechanistic outcomes do not automatically establish chronic performance/health effects;
- evidence statements remain separate from recommendations;
- technical, practitioner-facing and lay-facing versions must preserve identical epistemic content;
- audience simplification cannot broaden population/outcome/time context or strengthen causal/certainty language;
- update conditions must specify what new result, precision, target evidence, bias resolution or threshold change would materially alter the conclusion.

#### `F0-A21` — NotebookLM study package

- `F0-A21` completed at `notebooklm/F0.10-synthesis-communication-uncertainty/`;
- verified canonical files on `main`:
  - `MANIFEST.md`;
  - `STUDY_GUIDE.md`;
  - `QA_REPORT.md`;
- package decision: `PASS — READY_FOR_STUDY`;
- first-pass corpus v1 is intentionally limited to exactly six sources:
  1. canonical F0.10 lesson — `CORE`;
  2. `F0-S19` GRADE intervention-certainty principles — `CORE`;
  3. `F0-S18` GRADE overview — `SUPPORT`;
  4. `F0-S20` GRADE indirectness — `SUPPORT`;
  5. `F0-S08` ASA p-value statement — `SUPPORT`;
  6. `F0-S09` ASA Task Force statement — `CONTRAST`;
- source roles are non-redundant: lesson = complete workflow; F0-S19 = range/threshold certainty; F0-S18 = certainty/recommendation boundary; F0-S20 = target-PICO directness; F0-S08 = p-value misuse safeguards; F0-S09 = protection against the false binary `threshold worship` versus `p-values are useless`;
- external sources/links were rechecked on 2026-09-10 before package closure;
- ASA statement still exposes the six core p-value principles used here;
- ASA Task Force statement still emphasizes uncertainty, variability, multiplicity and replicability while retaining a role for properly interpreted p-values/significance tests;
- GRADE overview remains last modified `12 May 2026`;
- GRADE intervention-certainty principles remain last modified `21 August 2025` and retain body/outcome range-threshold reasoning;
- GRADE indirectness remains last modified `12 May 2026` and retains PICO-alignment/applicability logic;
- no new source ID was needed because every external package source already exists in `SOURCE_INDEX.md`;
- Study Guide contains 20 ordered passes from role definition and invariant-core construction through quantitative uncertainty, p-values, certainty, directness, false balance, recommendation boundary, three-audience translation, drift audit and update conditions;
- guided examples `G1`/`G2`/`G3` are fresh synthetic examples rather than the completed F0.10 assessment package;
- F0.10 `EXERCISES.md`, `ANSWER_KEY.md`, production QA, full `SOURCE_INDEX.md` and F0.4 `ENTRY_DIAGNOSTIC.md` remain outside the first-pass NotebookLM corpus;
- no third-party full text was persisted;
- package production changed no learner state and did not change the F0.4 diagnostic.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.10 STUDY_PACKAGE_READY`.

F0.1–F0.10 now all have approved instructional units and approved NotebookLM study packages. F0.4 additionally has a quantitative entry diagnostic, still `UNOBSERVED`.

The **cumulative F0 Exit Assessment has not yet been authored/executed as a final packet**. Its architecture already exists in `foundations/F0-scientific-literacy/ASSESSMENT_BLUEPRINT.md`.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from curriculum/package production.

## Exit-assessment canonical gate

Per `ASSESSMENT_BLUEPRINT.md` and `MASTERY_PROTOCOL.md`:

- total assessment = 100 points;
- Section A question/design/causal structure = 20;
- Section B quantitative interpretation = 25;
- Section C systematic review/certainty = 20;
- Section D full-paper critical appraisal = 25;
- Section E communication of uncertainty = 10;
- pass requires `>=85/100` total;
- every section must score at least 70% of its available points;
- any `CRITICAL_FAIL` blocks passage;
- `75–84` with no critical fail = `NEAR_PASS / TARGETED_REMEDIATION`;
- below 75 requires broader remediation mapped to the earliest broken prerequisite;
- a first strong exit performance may support `APPLIED`/`INTEGRATED`; it does not automatically authorize `MASTERED`, which requires robust/repeated performance over time.

## Pending learner validations

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
- F0.10 has not yet been studied or assessed by the learner;
- approved NotebookLM guides exist for F0.1–F0.10;
- no mastery-state change is authorized from production alone.

## Operational constraints

- repository is public;
- never persist sensitive personal/health data;
- do not publish copyrighted full text without redistribution permission;
- current/living methodological claims must be rechecked when materially relevant;
- NotebookLM is a study layer; GitHub remains canonical;
- answer keys and diagnostics must not contaminate first-pass retrieval/assessment;
- production can proceed while learner validation remains pending;
- F0.4 diagnostic remains `UNOBSERVED` until actual learner responses are produced.

## NEXT_ACTION

`F0-A22` — Author the complete cumulative **F0 Exit Assessment v1** from the already approved `ASSESSMENT_BLUEPRINT.md` without scoring or changing learner state. Create a dedicated exit-assessment packet under `foundations/F0-scientific-literacy/F0-exit-assessment/` containing at minimum `ASSESSMENT.md`, `ANSWER_KEY.md` and production `QA_REPORT.md`. Preserve the five-section 100-point structure exactly: A question/design/causal structure 20; B quantitative interpretation 25; C systematic review/certainty 20; D full-paper critical appraisal 25; E communication of uncertainty 10. Preserve the pass gate `>=85/100 + each section >=70% + no CRITICAL_FAIL`. Build section A from fresh synthetic question/design/DAG scenarios; section B from fresh distribution/SD-SE/effect-CI-threshold/p-value/power/multiplicity scenarios; section C from a fresh synthetic forest-plot/evidence-synthesis package plus review-method and certainty/applicability tasks; section D must use one legally accessible complete human exercise/nutrition paper with enough quantitative uncertainty and methodological detail for genuine appraisal, preferably a **different paper from F0-S30** to reduce answer memorization, with registration/protocol/supplement materials where feasible; section E must require technical and plain-language communication from the same evidence result with invariant epistemic content. Recheck every external source/paper actually used, add only actually used new sources to `SOURCE_INDEX.md`, and do not copy non-redistributable third-party full text into the public repository. The answer key must include point-by-point scoring, acceptable alternative reasoning, critical-fail triggers and remediation mapping to the earliest broken F0 dependency. Apply CONTENT/EVIDENCE/PEDAGOGICAL/MASTERY QA to the assessment itself. Preserve all F0.1–F0.10 learner states as pending and F0.4 diagnostic `UNOBSERVED`; do not mark `APPLIED`, `INTEGRATED` or `MASTERED` because no learner response exists. After verification, update this checkpoint and leave exactly one subsequent `NEXT_ACTION` for administering/studying toward the exit gate rather than silently inferring performance.