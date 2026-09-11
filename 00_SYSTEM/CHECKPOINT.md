# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-11
**Canonical branch:** `main`
**Project state:** `F0_STUDY_RUNBOOK_READY`

## Canonical project state

- repository is public;
- GitHub remains canonical; NotebookLM is a controlled study layer;
- production and learner validation are separate;
- no private health data, secrets or non-redistributable third-party full text may be persisted;
- living/versioned scientific claims are rechecked when materially relevant;
- learner-state changes require observed evidence, never production inference.

## F0 production status

`F0 — Scientific Literacy and Quantitative Reasoning`

All ten instructional units are approved and all ten NotebookLM packages are `READY_FOR_STUDY`:

| Module | Unit | NotebookLM |
|---|---|---|
| F0.1 Scientific questions/hypotheses/operationalization | APPROVED | READY_FOR_STUDY |
| F0.2 Study designs and inference boundaries | APPROVED | READY_FOR_STUDY |
| F0.3 Bias/confounding/causal reasoning/validity | APPROVED | READY_FOR_STUDY |
| F0.4 Descriptive statistics/distributions/sampling variation | APPROVED | READY_FOR_STUDY |
| F0.5 Estimates/CIs/p-values/effect sizes/practical relevance | APPROVED | READY_FOR_STUDY |
| F0.6 Power/Type I-II/multiplicity/analytical flexibility | APPROVED | READY_FOR_STUDY |
| F0.7 Systematic reviews/meta-analysis/heterogeneity | APPROVED | READY_FOR_STUDY |
| F0.8 Risk of bias/certainty/applicability | APPROVED | READY_FOR_STUDY |
| F0.9 Critical reading of a complete paper | APPROVED | READY_FOR_STUDY |
| F0.10 Synthesis/communication of uncertainty | APPROVED | READY_FOR_STUDY |

F0.4 additionally has `ENTRY_DIAGNOSTIC.md`; state remains `UNOBSERVED`.

Persistent reasoning safeguards remain:

- association ≠ causation;
- randomized ≠ automatically low risk of bias;
- reporting completeness ≠ validity/certainty;
- risk of bias is result-specific/domain-based, not a total score;
- `p<0.05` ≠ truth/importance;
- `p>0.05` ≠ no effect/equivalence;
- frequentist CI ≠ posterior probability interval;
- completed-study interpretation uses estimate + CI + practical threshold + design/bias, not observed power;
- multiplicity includes outcomes, timepoints, subgroups, models and data-dependent paths;
- prespecification improves auditability without guaranteeing validity;
- systematic review ≠ meta-analysis; pooling is compatibility-dependent;
- inverse-variance weight is precision, not quality/certainty;
- I² is not a quality/sameness score;
- certainty is body/outcome/question specific and not effect magnitude;
- internal validity and applicability are separate;
- one-paper appraisal ≠ body-level certainty;
- certainty of one outcome ≠ recommendation strength;
- simplifying language cannot increase certainty or broaden scope.

## F0 cumulative Exit Assessment

`F0-A22` is complete.

Approved packet:

`foundations/F0-scientific-literacy/F0-exit-assessment/`

Verified artifacts:

- `ASSESSMENT.md` — 100 points;
- `ANSWER_KEY.md` — scoring/alternatives/critical fails/remediation mapping;
- `QA_REPORT.md` — `PASS — READY_FOR_ADMINISTRATION`.

Exit structure:

- A question/design/causal structure = 20;
- B quantitative interpretation = 25;
- C systematic review/certainty = 20;
- D full-paper critical appraisal = 25;
- E communication of uncertainty = 10.

Exit gate:

- `>=85/100` total;
- every section `>=70%`;
- no `CRITICAL_FAIL`;
- defensible integrated Section D chain;
- no increase in certainty during Section E simplification.

`75–84` with no critical fail = `NEAR_PASS / TARGETED_REMEDIATION`.
Below 75 = broader remediation mapped to earliest broken dependency.
A first strong pass may support `APPLIED`/`INTEGRATED`; it never automatically authorizes `MASTERED`.

Section D uses alternate transfer source `F0-S32` with registry companion `F0-S33`; these remain quarantined from first-pass study so the exit paper is not memorized in advance.

## F0-A23 — Study-to-Exit Runbook

`F0-A23` is complete.

Canonical learner-facing runbook:

`study/F0_STUDY_RUNBOOK.md`

State: `READY_FOR_USE`.

The runbook defines the full learner path from current `UNSEEN` state to legitimate exit readiness.

### Canonical first-pass route

`F0.1 → F0.2 → F0.3 → F0.4 quantitative entry diagnostic → F0.4 → F0.5 → F0.6 → F0.7 → F0.8 → F0.9 → F0.10 → cumulative retrieval → Exit Assessment`

The prerequisite graph remains authoritative; this linear route is a preferred operational route, not permission to bypass P2 dependencies.

### NotebookLM setup rule

For every module:

1. create a separate NotebookLM notebook;
2. use that module's `MANIFEST.md` as the exact initial corpus specification;
3. preserve `CORE`/`SUPPORT`/`CONTRAST` roles;
4. use the ordered `STUDY_GUIDE.md` passes;
5. keep `EXERCISES.md`, `ANSWER_KEY.md`, production QA, full `SOURCE_INDEX.md`, diagnostics and exit materials outside the initial corpus;
6. do not substitute AI summaries or random NotebookLM-discovered sources for approved sources.

### Standard learner cycle

`source-guided study → closed-book recall → fresh micro-transfer → independent module EXERCISES → correction/error routing → canonical study-record update`

All current module assessments use local progression gate:

`>=80/100 + no critical fail`

- 70–79 → targeted remediation + equivalent fresh retest;
- <70 → broader module review + equivalent reassessment;
- any critical fail → mandatory repair/retest regardless of numerical score.

A local pass may support `APPLIED` only when observed work demonstrates application. `INTEGRATED` requires cross-module performance. `MASTERED` requires robust repeated performance over time.

### F0.4 quantitative gate

`ENTRY_DIAGNOSTIC.md` must be independently administered before F0.4 quantitative readiness is treated as demonstrated.

Routing remains:

- `READY_FOR_F0.4` = 14–16/16 and no 0/2 domain;
- `P1_REPAIR` = localized gaps under canonical diagnostic criteria;
- `P2-QB_REQUIRED` = <=9/16, >=3 zeroed domains, or fewer than six domains with any demonstrated competence.

If `P2-QB_REQUIRED`, the quantitative bridge becomes a structural prerequisite and F0.4/downstream quantitative validation pauses until an equivalent retest demonstrates readiness.

### Retrieval/spacing

Runbook defines:

- R0 same-cycle closed-book recall + fresh micro-transfer;
- R1 short-delay retrieval at 1–3 days;
- R2 mixed retrieval at ~7 ± 2 days;
- R3 cumulative integration at ~14–21 days and again after F0.10;
- at least one delayed cumulative retrieval before the Exit Assessment even if study is accelerated.

### Persistent learner records

Observed study events update only when evidence exists:

- `study/STUDY_HISTORY.md` — concrete activity/performance/strength/gap/next action;
- `study/ERROR_LEDGER.md` — material observed conceptual/statistical/application/integration errors with remediation/retest status;
- `study/MASTERY_MATRIX.md` — state transitions supported by observed evidence only.

Errors route to the earliest broken dependency rather than the module where they were first noticed.

### Exit readiness

Before administration of the cumulative Exit Assessment:

- all F0.1–F0.10 have observed first-pass study;
- F0.4 diagnostic/bridge is resolved;
- all ten independent module assessments have passed their local gate or been repaired by equivalent retest;
- no unresolved structural prerequisite error remains;
- at least one delayed cumulative retrieval has occurred after F0.10;
- an integrated chain has already been demonstrated outside the exit packet;
- exit answer key and F0-S32/F0-S33 remain uncontaminated.

If the exit answer key is exposed before independent administration, v1 is not treated as clean validation and an alternate form is required.

## Current learner position

**Learning position:** `UNSEEN`.

Repository learner artifacts still confirm:

- initial domain = `UNKNOWN` and must be measured rather than inferred;
- `study/MASTERY_MATRIX.md` aggregate F0 = `UNSEEN`;
- F0.4 diagnostic = `UNOBSERVED`;
- no F0.1–F0.10 module has observed evidence for `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`;
- `study/STUDY_HISTORY.md` contains no completed learner event yet;
- `study/ERROR_LEDGER.md` contains no observed learner error yet.

Creating the runbook changed **no learner state**.

## Operational constraints for the next phase

- next work is learner validation, not additional F0 curriculum production;
- initial F0.1 corpus must exclude its `EXERCISES.md` and `ANSWER_KEY.md`;
- correction occurs only after an unaided response;
- only actual learner performance may be persisted;
- personal/health information stays out of the public repository;
- F0 Exit Assessment remains quarantined until runbook readiness criteria are met.

## NEXT_ACTION

`F0-A24` — Begin the **first observed F0.1 learner study session** using `study/F0_STUDY_RUNBOOK.md`, `notebooklm/F0.1-scientific-questions/MANIFEST.md` and `STUDY_GUIDE.md`. Do not produce new curriculum. First verify/guide creation of the approved six-source F0.1 NotebookLM corpus without adding `EXERCISES.md`, `ANSWER_KEY.md`, QA metadata or future-module sources. Then begin the F0.1 study sequence with the conceptual skeleton and an unaided learner response before correction; use one-question-at-a-time Socratic retrieval rather than revealing answers. Persist only study/performance that actually occurs in the session: append `study/STUDY_HISTORY.md` when there is meaningful observed activity, add `ERROR_LEDGER.md` entries only for material demonstrated errors, and update `MASTERY_MATRIX.md` only if the observed evidence justifies a state transition. Do not administer the F0.4 diagnostic, later-module assessments or the F0 Exit Assessment in this action unless the canonical runbook is subsequently updated by a real learner event that makes such progression legitimate.