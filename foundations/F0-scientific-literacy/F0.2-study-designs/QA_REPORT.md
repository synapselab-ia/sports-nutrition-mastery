# F0.2 — QA report

**Unit:** `F0.2 — Study designs and what they can answer`

**Reviewed:** 2026-09-08

**Production decision:** `APPROVED`

This report records production QA only. It does **not** record learner performance and does not change any mastery state.

---

## 1. Scope gate

### Required by COURSE_MAP / NEXT_ACTION

- randomized parallel trials — covered;
- randomized crossover trials — covered;
- cluster-randomized trials — covered;
- factorial randomized trials — covered;
- non-randomized intervention studies — covered;
- cohort, case-control and cross-sectional designs — covered;
- acute mechanistic versus chronic outcome studies — covered;
- temporal ordering — covered;
- within-subject versus between-subject comparisons — covered;
- washout/carryover intuition — covered;
- period effects at introductory level — covered;
- unit of allocation versus unit of observation/analysis — covered;
- diagnostic versus prognostic versus intervention questions — covered at introductory level;
- target-trial concept — covered at introductory level;
- strongest defensible inference + tempting unsupported inference for every major design — embedded throughout lesson and mandatory in exercises;
- eight-design classification performance task — covered in `EXERCISES.md` Part B.

### Intentionally deferred

The unit does **not** attempt to teach in full:

- formal confounding, exchangeability assumptions, DAGs, collider/mediator logic — F0.3;
- detailed selection/information/missing-data bias — F0.3/F0.8;
- statistical models for paired, clustered or factorial data — F0.4–F0.6;
- effect-measure mathematics — F0.5;
- power/multiplicity/interaction-testing mathematics — F0.6;
- formal systematic review/meta-analysis methods — F0.7;
- formal RoB 2/ROBINS-I judgments — F0.8;
- complete-paper appraisal — F0.9.

This keeps F0.2 focused on design architecture and inferential boundaries rather than prematurely collapsing F0.3–F0.8 into one lesson.

---

## 2. Source recheck — PASS

Authoritative/current resources were rechecked externally on 2026-09-08 before production.

### Current/general resources

- `F0-S01` — CONSORT 2025 remains the current general randomized-trial reporting statement; current CONSORT materials explicitly recognize design-specific extensions.
- `F0-S02` — the official STROBE site continues to provide separate/current checklists for cohort, case-control and cross-sectional reporting and explicitly remains reporting guidance rather than a quality score.
- `F0-S14` — ICH E9/E9(R1) retained for alignment of objective/estimand/design.
- `F0-S16` — Hernán & Robins retained as causal-inference foundation.
- `F0-S17` — Hernán et al. 2025 target-trial framework rechecked; it specifies a two-step logic of target-trial specification followed by attempted emulation and explicitly does not solve inadequate data/unmeasured confounding by itself.

### Design-specific resources added because they were actually used

- `F0-S22` — Cochrane Handbook v6.5 Chapter 23, current handbook version 6.5 (2024): cluster and crossover variants, unit-of-analysis problem, within-person comparison, carryover and period effects.
- `F0-S23` — Dwan et al. 2019 CONSORT crossover extension: randomized sequences, periods, carryover and crossover-specific reporting.
- `F0-S24` — Campbell et al. 2012 CONSORT cluster extension: cluster as allocation unit and need to report/analyse clustering explicitly.
- `F0-S25` — Kahan et al. factorial CONSORT extension (JAMA 2023) plus explanation/elaboration (BMJ 2025): 2 × 2 factorial architecture, main comparisons and interaction.

### Version caveat

The cluster, crossover and factorial design extensions were originally written against CONSORT 2010. The current CONSORT/SPIRIT extension site still lists design-specific extensions while CONSORT 2025 is the general standard. F0.2 therefore uses the **current CONSORT 2025 statement as the general reporting backbone** and the legacy-design extensions only for their still-relevant design-specific concepts. They are not represented as 2025-rewritten extensions unless/until such revisions are published.

No new source was added solely for decoration.

---

## 3. CONTENT_QA — PASS

Checked:

- randomization is described as an allocation mechanism, not a universal validity certificate;
- finite-sample baseline imbalance is not falsely treated as evidence that randomization “failed”;
- parallel versus crossover is separated by comparison architecture;
- crossover suitability requires reversibility/stability and carryover control;
- washout is not presented as a universal fixed duration;
- cluster randomization distinguishes unit of allocation from observed individuals;
- unit-of-analysis dependence is introduced without premature statistical derivations;
- factorial trials are not presented as automatically additive; interaction is explicit;
- non-randomized interventions are neither promoted to automatic causality nor dismissed as useless;
- retrospective cohort is differentiated from case-control by how sampling starts, not by whether historical records are used;
- cohort temporal ordering is not equated with causal identification;
- cross-sectional association is not presented as temporal/causal evidence;
- acute mechanistic outcomes are explicitly separated from chronic adaptation outcomes;
- diagnostic, prognostic and intervention questions are treated as distinct design problems;
- target-trial emulation is not presented as retroactive randomization;
- “RCT > observational” is rejected as a universal hierarchy while preserving design-specific inferential limits.

No material internal contradiction identified.

---

## 4. EVIDENCE_QA — PASS

Evidence safeguards:

- reporting guidelines are used to identify/report architecture, not as risk-of-bias scores;
- the current CONSORT 2025 general statement is distinguished from older design-specific extensions;
- source claims remain within source scope;
- no primary sports-nutrition study is promoted into methodological authority;
- no practical nutrition recommendation is inferred from methodological examples;
- no association is converted into causal effect without additional assumptions;
- no acute mechanism is converted into chronic benefit;
- target-trial claims preserve the source’s explicit limitation that design emulation cannot repair inadequate data.

`F0-S03` (PRISMA 2020) is used only as a boundary reminder that systematic reviews are a separate synthesis/reporting layer; F0.7 retains the substantive review/meta-analysis teaching.

---

## 5. PEDAGOGICAL_QA — PASS

### Prerequisites

`F0.1` is the sole P2 prerequisite and supplies question/estimand language.

Local P0/P1 coverage includes:

- intervention/exposure;
- allocation/follow-up;
- prospective/retrospective;
- between-subject/within-subject;
- washout/carryover/period effect;
- allocation/observation/analysis units;
- temporal ordering.

### Progression

The lesson follows:

`question → design vocabulary → comparison structure → randomized variants → non-randomized intervention → observational designs → acute/chronic → diagnostic/prognostic → target trial → anti-hierarchy reasoning → identification algorithm → active recall`

### Autossuficiência

A learner does not need external methodology material to classify the required designs or state their core inferential boundaries. External sources provide traceability and deeper technical detail rather than outsourcing essential explanation.

### Anti-memorization design

Every major design is taught with:

1. architecture;
2. comparison structure;
3. use-case;
4. strongest defensible inference;
5. tempting unsupported inference.

This directly operationalizes the module competency rather than teaching labels alone.

---

## 6. MASTERY_QA — PASS

`EXERCISES.md` tests:

- `K1` — recall of core design vocabulary;
- `K3` — compare parallel/crossover, cohort/case-control, randomized/non-randomized;
- `K4` — interpret what each design can support;
- `K5` — predict consequences of persistent effects, temporal ambiguity and clustering;
- `K6` — select/design an architecture for a concrete question;
- `K7` — integrate F0.1 question formulation with target-trial thinking;
- `K8` — state inferential limits and unsupported extrapolations.

The mandatory “strongest inference + tempting invalid inference” requirement prevents a learner from passing through terminology recognition alone.

Critical-fail conditions explicitly target structural misconceptions that would make F0.3 unsafe to learn on top of a broken design model.

Production approval alone does not mark `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`.

---

## 7. Public-repository/privacy QA — PASS

- no personal/health-identifying data;
- no learner-specific sensitive information;
- no copyrighted guideline PDF copied into repository;
- sources are cited/link-referenced only;
- examples are hypothetical educational research designs, not individualized nutrition prescriptions.

---

## 8. Final gate

> Can a capable learner who has completed F0.1 classify the principal human research designs used in nutrition/exercise science, reason from architecture to inference, reject a tempting overclaim, and enter F0.3 without hidden design prerequisites?

**Decision:** yes — `APPROVED`.

NotebookLM packaging is not part of `F0-A04`; it should be produced only under the subsequent canonical action.