# F0.3 — NotebookLM Study Package QA Report

**Module:** `F0.3 — Bias, confounding, causal reasoning and validity`
**Package version:** `1`
**Reviewed:** `2026-09-09`
**Package decision:** `PASS — READY_FOR_STUDY`
**Learner-state change:** none

This report records QA of the NotebookLM package only. It does not record that the learner studied F0.3 and does not authorize any transition from `UNSEEN`.

---

## 1. Package contents — PASS

Required files exist in the intended package path:

- `notebooklm/F0.3-bias-confounding-causal-validity/MANIFEST.md`;
- `notebooklm/F0.3-bias-confounding-causal-validity/STUDY_GUIDE.md`;
- `notebooklm/F0.3-bias-confounding-causal-validity/QA_REPORT.md`.

The package is aligned to the approved instructional unit:

- `foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/LESSON.md`.

The package does not alter or replace the canonical instructional lesson.

---

## 2. Corpus-size and auditability gate — PASS

The initial corpus is limited to **six sources**:

1. canonical F0.3 lesson — `CORE`;
2. Hernán & Robins, `Causal Inference: What If` — `CORE`;
3. Feeney, Hartwig & Davies 2025 BMJ DAG guide — `CORE`;
4. Catalogue of Bias — `SUPPORT`;
5. official ROBINS-I V2 webpage — `SUPPORT` / boundary source;
6. Hernán et al. 2025 target-trial framework — `CONTRAST`.

This is deliberately smaller than the complete F0 source registry.

### Redundancy decision

Additional DAG tutorials, individual bias pages and full formal risk-of-bias documents were not added because:

- the canonical lesson already translates the F0.3 curriculum;
- the 2025 BMJ DAG guide provides a current practical causal-diagram anchor;
- the Catalogue of Bias supplies enough concrete examples without loading dozens of near-redundant pages;
- full RoB 2/ROBINS-I mechanics belong to F0.8;
- a small corpus is easier to audit and reduces retrieval noise.

### Scope decision

`Causal Inference: What If` is included because F0.3 is the first formal causal-reasoning unit, but the study guide explicitly restricts use to introductory counterfactual, exchangeability, randomization and confounding/selection concepts. Advanced longitudinal causal methods are not part of F0.3 mastery.

---

## 3. Source/file/link verification — PASS

Verification date: `2026-09-09`.

### Canonical F0.3 lesson

Verified on canonical `main`:

- path: `foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/LESSON.md`;
- production state: `APPROVED`;
- prerequisite structure: F0.1 + F0.2;
- required causal-validity content is present.

Preferred NotebookLM URL uses raw project Markdown. If raw URL ingestion fails, the guide instructs upload of the same file rather than replacement with an AI-generated summary.

### Causal Inference: What If

Verified official authors' landing page:

- `https://miguelhernan.org/whatifbook`;
- citation remains Hernán MA, Robins JM (2020), *Causal Inference: What If*;
- page explicitly states that the online text may be revised/corrected and instructs readers to use the latest version from that page;
- the current linked PDF observed during verification is dated `19aug26`.

The package therefore points to the maintained authors' page rather than freezing an old mirrored PDF URL.

### BMJ DAG guide

Verified current article:

- Feeney T, Hartwig FP, Davies NM;
- *How to use directed acyclic graphs: guide for clinical researchers*;
- BMJ 2025;388:e078226;
- DOI `10.1136/bmj-2023-078226`;
- published 21 March 2025.

The article explicitly treats DAGs as representations of hypothesized/assumed causal mechanisms and uses them to reason about confounding, selection and covariate choice. The package correctly prevents DAGs from being treated as empirical proof generators.

### Catalogue of Bias

Verified current Catalogue of Bias index:

- `https://catalogofbias.org/biases/`;
- site is active under the Centre for Evidence-Based Medicine;
- current index includes directly relevant entries such as attrition bias, collider bias, selection bias and confounding;
- the site itself states that entries continue to be added over time.

The package uses the catalogue as mechanism/example support, not as a checklist whose labels substitute for causal reasoning.

### riskofbias.info / ROBINS-I V2

Verified official site and V2 page:

- hub remains `https://www.riskofbias.info/` and exposes RoB 2, ROBINS-I, ROBINS-E and ROB ME;
- ROBINS-I V2 page remains `https://www.riskofbias.info/welcome/robins-i-v2`;
- the official page states that the revised V2 was posted **20 November 2025**;
- the page explicitly says this is still a **draft version** and is subject to change;
- current displayed V2 domains include confounding, intervention classification, selection into the study, missing data, outcome measurement and selection of the reported result;
- the site states the tool resources are licensed under CC BY-NC-ND 4.0.

### Correction relative to previous project note

The previous project record said `30 November 2025`. Current direct verification of the official page shows `20 November 2025`. The package uses the verified date and the source registry should be corrected accordingly.

### Target-trial framework

Verified free full text:

- Hernán MA, Dahabreh IJ, Dickerman BA, Swanson SA;
- *The Target Trial Framework for Causal Inference From Observational Data: Why and When Is It Helpful?*;
- Ann Intern Med. 2025;178(3):402-407;
- DOI `10.7326/ANNALS-24-01871`;
- free full text remains available via PMC.

The article explicitly distinguishes design-induced biases that target-trial emulation can help prevent from data limitations such as unmeasured confounding that the framework does not itself resolve.

---

## 4. Role assignment QA — PASS

Each source has a defined instructional function.

### `CORE`

**Canonical F0.3 lesson**

Function:

- supplies the project's exact reasoning sequence;
- integrates all F0.3 mechanisms at the intended depth;
- defines repairability/calibrated-conclusion requirements;
- preserves the F0.3/F0.8 scope boundary.

**Causal Inference: What If**

Function:

- anchors counterfactual and exchangeability intuition;
- explains why causal identification differs between randomized and observational settings;
- provides deeper methodological authority beneath the lesson's accessible translation.

**BMJ DAG guide**

Function:

- operationalizes simple DAG construction;
- connects assumed causal structure to confounder/mediator/collider/selection roles;
- anchors adjustment decisions to the target estimand and causal assumptions.

### `SUPPORT`

**Catalogue of Bias**

Function:

- supplies concrete named examples;
- strengthens transfer from abstract structure to recognizable research failure modes;
- is explicitly prevented from becoming a memorization exercise.

**ROBINS-I V2 webpage**

Function:

- exposes contemporary domain separation;
- teaches version literacy and the difference between conceptual bias mechanisms and later formal tool application;
- reinforces that a risk-of-bias framework is not a single quality score.

### `CONTRAST`

**Target-trial framework**

Function:

- contrasts preventable design-induced bias with persistent data limitations;
- provides a concrete bridge from F0.2 target-trial introduction to F0.3 causal-validity reasoning;
- reinforces that emulation is not randomized assignment.

No source is assigned a role outside its methodological purpose.

---

## 5. Required F0-A07 reasoning-sequence coverage — PASS

The package repeatedly enforces:

`target causal question/estimand`

`→ temporal/causal structure`

`→ confounder/mediator/collider/selection/measurement/missingness mechanism`

`→ valid versus invalid adjustment/conditioning`

`→ repairability/data limitation`

`→ calibrated conclusion`

This sequence appears in:

- manifest learning objectives;
- claims to master;
- active recall/integration prompts;
- NotebookLM task rules;
- study-guide universal template;
- each applied study pass;
- the integrated evidence-critique task;
- the final mixed causal-validity examination.

A learner therefore cannot satisfy the package by naming a bias without explaining its mechanism.

---

## 6. DAG reasoning QA — PASS

The package requires the learner to:

- define the target causal question before drawing;
- identify exposure/intervention and outcome;
- encode assumed temporal/causal directions;
- include measured and unmeasured variables when relevant;
- classify confounder, mediator and collider relative to the estimand;
- select adjustment based on structure rather than prediction/association alone;
- challenge at least one arrow and reconsider the adjustment set;
- explicitly state that arrows are assumptions.

The package does **not** claim that:

- a DAG proves causality;
- one DAG is automatically true because it is published;
- drawing a DAG eliminates unmeasured confounding;
- a minimally sufficient adjustment set remains valid when the causal structure is wrong.

---

## 7. Randomized versus observational bias-pathway QA — PASS

Study Pass 10 requires stage-by-stage comparison of:

- baseline assignment/confounding;
- adherence/deviations;
- follow-up/missingness;
- outcome measurement;
- analysis/reporting;
- applicability.

This protects against two opposite errors:

- `RCT = perfect truth`;
- `randomization offers no special causal protection`.

The intended conclusion is that randomized assignment powerfully addresses baseline treatment-assignment confounding in expectation, while later bias mechanisms require separate design/conduct/analysis protections.

---

## 8. Selection, measurement and missingness QA — PASS

### Selection

The guide varies selection at:

- recruitment;
- eligibility restriction;
- retention/follow-up;
- complete-case status;
- final analytical inclusion.

Learners must determine what causes selection and whether conditioning opens a non-causal path rather than using `selection bias` as a generic label.

### Measurement

The guide varies:

- exposure measurement;
- outcome measurement;
- confounder measurement;
- calibration;
- recall;
- differential awareness;
- coarse categorization/proxy measurement.

It explicitly rejects the universal claim that non-differential misclassification always biases toward the null.

### Missingness/attrition

The guide deliberately presents identical missing-data percentages under different causal mechanisms and requires different validity judgments.

It prevents:

- missing percentage = bias direction;
- equal missingness = unbiased;
- complete-case analysis = automatically neutral.

---

## 9. Target-trial boundary QA — PASS

The package uses the 2025 target-trial framework to teach:

- eligibility;
- strategies;
- assignment concept;
- time zero;
- follow-up;
- outcome;
- causal contrast;
- design/data mapping.

It repeatedly requires separation of:

1. design-induced bias preventable by better emulation;
2. measured limitations potentially addressed under assumptions;
3. unmeasured/unavailable information not guaranteed recoverable;
4. residual causal assumptions.

The package never represents target-trial emulation as retroactive randomization.

---

## 10. Formal RoB/GRADE scope-control QA — PASS

The package explicitly defers to F0.8:

- RoB 2 formal application;
- ROBINS-I/ROBINS-I V2 signaling-question algorithms;
- domain-level formal judgments;
- overall formal risk-of-bias judgments;
- GRADE certainty domains/ratings.

The ROBINS-I V2 webpage is present only as a support/boundary source showing contemporary domain separation and version status.

The current V2 is labeled **draft** everywhere in the package where status matters.

---

## 11. Answer-leakage control — PASS

Excluded from the initial NotebookLM corpus:

- F0.3 `ANSWER_KEY.md`;
- F0.3 `EXERCISES.md`;
- F0.3 production `QA_REPORT.md`;
- full `SOURCE_INDEX.md`.

`EXERCISES.md` remains the independent first-pass assessment and is completed only after source-guided study.

The guide requires NotebookLM to:

- present scenarios one at a time;
- wait for causal reasoning before grading;
- avoid naming the bias in the prompt;
- require a DAG/text structure where appropriate;
- grade only after the learner commits to an answer.

---

## 12. Pedagogical QA — PASS

The sequence progresses by conceptual dependency:

`random vs systematic error`

`→ counterfactual/exchangeability`

`→ confounding/residual confounding`

`→ confounder/mediator/collider`

`→ DAG construction and assumption challenge`

`→ selection`

`→ measurement/misclassification`

`→ missingness/attrition`

`→ reverse causation`

`→ randomized vs observational bias pathways`

`→ target trial: design vs data limitation`

`→ internal vs external validity`

`→ mixed unfamiliar causal appraisal`

The learner repeatedly:

- retrieves without answer exposure;
- creates and critiques causal structures;
- compares near-neighbor mechanisms;
- revises decisions after an assumed arrow changes;
- separates what analysis can mitigate from information that is not present;
- calibrates conclusions to assumptions.

This supports F0.3 practice across `K1`, `K3`, `K4`, `K5`, `K6`, `K7` and `K8`, while later cumulative retesting remains necessary for `MASTERED`.

---

## 13. Scientific-boundary QA — PASS

The package does not prematurely import F0.4-F0.6 statistics.

It may state conceptually that:

- random error differs from systematic error;
- larger samples generally reduce sampling variability but not systematic bias;
- precision and causal validity are distinct.

It intentionally does **not** teach in F0.3:

- standard-error formulas;
- confidence-interval mechanics;
- p-value interpretation;
- effect-size mathematics;
- Type I/II error;
- power calculations;
- multiplicity.

Those remain for F0.4-F0.6.

---

## 14. Public-repository/copyright QA — PASS

The public GitHub package contains only:

- project-authored Markdown;
- citations;
- official/open web links;
- study instructions.

No third-party PDF or formal risk-of-bias tool document was copied into the repository.

For `Causal Inference: What If`, the guide instructs the learner to obtain the current PDF from the authors' official page for personal NotebookLM use rather than versioning it in the public project.

For ROBINS-I V2, the package links only to the official webpage; it does not redistribute the CC BY-NC-ND tool document.

No personal, clinical or sensitive learner information is persisted.

---

## 15. Learner-state integrity — PASS

Before package creation:

- F0.1: pending / no observed validation;
- F0.2: pending / no observed validation;
- F0.3: `UNSEEN` / no observed validation.

After package creation:

- no learner-state transition is authorized;
- package readiness is production metadata only;
- `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` and `MASTERED` remain unsupported without observed learner performance;
- later cumulative retesting is still required for `MASTERED`.

---

## 16. Final Study Package gate

Question:

> Can a capable learner use this small, auditable corpus to learn F0.3 causal-validity reasoning, construct/critique simple DAGs, distinguish confounders/mediators/colliders, identify selection/measurement/missingness mechanisms, understand what randomization and target-trial design do and do not solve, separate repairable from unavailable information, and communicate a calibrated causal conclusion—without leaking the assessment or prematurely applying formal RoB/GRADE tools?

**Decision:** yes.

**Package state:** `READY_FOR_STUDY`.
