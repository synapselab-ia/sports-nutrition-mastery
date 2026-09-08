# F0.1 — QA report

**Unit:** `F0.1 — Scientific questions, hypotheses and operationalization`

**Reviewed:** 2026-09-08

**Production decision:** `APPROVED`

This report records production QA only. It does **not** record learner performance and does not change any mastery state.

---

## 1. Scope gate

### Required by COURSE_MAP

- scientific question framing — covered;
- target population, contrast, outcome and time — covered;
- construct, operational definition, variable, endpoint/outcome and estimand — covered;
- directional/non-directional hypotheses — covered;
- exploratory versus confirmatory reasoning — covered;
- primary versus secondary/exploratory outcomes — covered;
- prespecification versus post hoc reasoning — covered;
- introductory estimand thinking — covered;
- performance task converting popular claims into answerable questions — covered in `EXERCISES.md`.

### Intentionally deferred

The lesson does **not** attempt to teach in full:

- randomized versus observational study designs — F0.2;
- confounding, selection bias or causal diagrams — F0.3;
- descriptive/inferential statistics — F0.4–F0.6;
- multiplicity mathematics — F0.6;
- systematic reviews/meta-analysis — F0.7;
- formal risk-of-bias/certainty frameworks — F0.8;
- complete-paper critical appraisal — F0.9.

This preserves the planned conceptual dependency structure.

---

## 2. CONTENT_QA — PASS

Checked:

- core terminology is explicitly defined;
- estimand is separated from estimator;
- population is separated from sample;
- construct is separated from operationalization;
- outcome labels are not treated as self-defining;
- acute mechanistic outcomes are not equated with long-term applied outcomes;
- exploratory analysis is not portrayed as invalid, only as requiring transparent labeling;
- prespecification is not portrayed as sufficient proof of validity;
- no statistical significance or causal-design content is prematurely taught as if mastered;
- examples are framed as hypothetical unless explicitly identified as the real transfer exemplar.

No material internal contradiction identified.

---

## 3. EVIDENCE_QA — PASS

### Methodological backbone

- `F0-S01` — CONSORT 2025: objectives, prespecified outcomes, transparent reporting and distinction between planned and non-prespecified changes.
- `F0-S05` — Cochrane Handbook v6.5: answerable question structure and role of question formulation in downstream evidence work.
- `F0-S14` — ICH E9/E9(R1): alignment of scientific question, estimand, design, analysis and interpretation.
- `F0-S15` — GRADE Book: structured answerable questions and outcome relevance.

### Transfer exemplar

- `F0-S21` — Areta et al. 2013: used only to teach reconstruction of the question and limits of extrapolating an acute myofibrillar-protein-synthesis outcome to chronic hypertrophy/performance.

### Evidence safeguards

- reporting guidelines are not presented as risk-of-bias tools;
- the primary exercise/nutrition study is not used as a methodological authority;
- no recommendation about protein distribution is inferred from the exemplar;
- no mechanistic outcome is presented as proof of long-term benefit;
- source scope/limitations are stated;
- current methodological source versions were checked on 2026-09-08.

---

## 4. PEDAGOGICAL_QA — PASS

### Prerequisites

There are no `P2` prerequisites for F0.1. All required `P0` vocabulary is defined locally. The relevant `P1` concepts — measurement specificity and time horizon — are taught with worked examples.

### Progression

The lesson follows:

`accessible claim → structured question → vocabulary → operationalization → hypotheses → exploratory/confirmatory distinction → outcome hierarchy/time → estimand → real transfer exemplar → failure modes → operational workflow → active recall`

### Autossuficiência

A learner does not need an external statistics or research-methods text to understand the core lesson. Sources provide traceability and optional depth rather than substituting for explanation.

### Examples and counterexamples

Each major abstract concept includes at least one concrete example or misuse pattern. Popular sports-nutrition claims are used as question-framing material without requiring prior knowledge of whether the claims are true.

---

## 5. MASTERY_QA — PASS

`EXERCISES.md` tests beyond recognition/definition:

- `K1`: terminology recall;
- `K3`: distinguish constructs, outcomes and reasoning modes;
- `K4`: identify what a real study actually measured;
- `K5`: predict what remains unsupported under different operationalizations;
- `K6`: formulate answerable PICO(T)/estimand-style questions;
- `K8`: state limits and uncertainty boundaries.

`ANSWER_KEY.md` includes reasoning criteria, acceptable variants and critical-fail conditions.

The local score gate can support progression after actual learner performance, but production alone does not mark `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`.

---

## 6. Public-repository/privacy QA — PASS

- no personal health data;
- no learner-identifying information;
- no copyrighted PDF copied into repository;
- external scientific work is referenced bibliographically/link-wise only;
- examples involving supplements are educational research examples, not individualized medical/nutrition prescriptions.

---

## 7. Final gate

> Can a capable learner without prior formal methodology training learn how to turn a vague sports-nutrition claim into a precise empirical question, understand what quantity is being targeted, recognize operationalization errors, and demonstrate the competence without hidden prerequisites?

**Decision:** yes — `APPROVED`.

NotebookLM packaging is not created in this action because the canonical `NEXT_ACTION` requires the instructional unit, exercises and key; packaging should follow the project protocol when a study package is explicitly scheduled.