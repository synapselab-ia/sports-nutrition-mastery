# F0.2 — NotebookLM Study Package QA Report

**Module:** `F0.2 — Study designs and what they can answer`
**Package version:** `1`
**Reviewed:** `2026-09-08`
**Package decision:** `PASS — READY_FOR_STUDY`
**Learner-state change:** none

This report records QA of the NotebookLM package only. It does not record that the learner studied F0.2 and does not authorize any transition from `UNSEEN`.

---

## 1. Package contents — PASS

Required files exist in the intended package path:

- `notebooklm/F0.2-study-designs/MANIFEST.md`;
- `notebooklm/F0.2-study-designs/STUDY_GUIDE.md`;
- `notebooklm/F0.2-study-designs/QA_REPORT.md`.

The package is aligned to the approved instructional unit:

- `foundations/F0-scientific-literacy/F0.2-study-designs/LESSON.md`.

The package does not alter or replace the canonical instructional lesson.

---

## 2. Corpus-size and auditability gate — PASS

The initial corpus is limited to **six sources**:

1. canonical F0.2 lesson — `CORE`;
2. Cochrane Handbook Chapter 23 — `CORE`;
3. CONSORT 2025 — `SUPPORT`;
4. factorial randomized-trial explanation/elaboration — `SUPPORT`;
5. STROBE — `SUPPORT`;
6. Hernán et al. 2025 target-trial framework — `CONTRAST`.

This is intentionally smaller than the full F0.2 methodological source list.

### Redundancy decision

Separate crossover and cluster CONSORT extensions were **not** added to the initial NotebookLM corpus because:

- the canonical lesson already provides the F0.2-level translation;
- Cochrane Chapter 23 provides both crossover and cluster architecture in one authoritative source;
- adding separate legacy extensions would increase corpus size without adding enough first-pass pedagogical value to justify the redundancy.

They remain registered in `SOURCE_INDEX.md` and available for later deep dives/F0.9 appraisal.

### Scope decision

`F0-S16` (`Causal Inference: What If`) remains a teacher/reference source rather than an initial NotebookLM source because its depth substantially exceeds the F0.2 target and risks pulling the learner prematurely into F0.3 causal-identification content.

---

## 3. Source/file/link verification — PASS

Verification date: `2026-09-08`.

### Canonical lesson

`foundations/F0-scientific-literacy/F0.2-study-designs/LESSON.md` exists on canonical `main` and remains `APPROVED`.

Preferred NotebookLM URL uses the repository raw Markdown endpoint. If NotebookLM cannot ingest that URL, the guide instructs the learner to upload the same canonical Markdown file rather than substitute an AI-generated summary.

### CONSORT 2025

Verified current BMJ article:

- Hopewell S, Chan A-W, Collins GS, et al.;
- *CONSORT 2025 statement: updated guideline for reporting randomised trials*;
- BMJ 2025;389:e081123;
- DOI `10.1136/bmj-2024-081123`;
- published 14 April 2025.

The package correctly treats CONSORT 2025 as the **current general randomized-trial reporting statement** and not as a study-quality/risk-of-bias instrument.

### Cochrane Chapter 23

Verified current Cochrane Handbook page:

- Chapter 23: *Including variants on randomized trials*;
- cited under Cochrane Handbook version 6.5 (2024);
- chapter itself last updated October 2019;
- contains cluster-randomized and crossover sections, including unit-of-allocation and crossover-suitability/carryover material.

The package records both the current Handbook version and older chapter-update date rather than implying the chapter was rewritten in 2024.

### STROBE

Verified official STROBE site remains available and explicitly covers:

- cohort;
- case-control;
- cross-sectional designs.

The official site explicitly states that the recommendations concern reporting, are not prescriptions for designing/conducting studies, and the checklist is not an instrument for evaluating study quality. The package preserves this restriction.

### Factorial trial guidance

Verified:

- 2023 JAMA factorial CONSORT extension: Kahan BC, Hall SS, Beller EM, et al., JAMA 2023;330(21):2106-2114, DOI `10.1001/jama.2023.19793`;
- 2025 BMJ explanation/elaboration: Kahan BC, Juszczak E, Beller E, et al., BMJ 2025;388:e080785, DOI `10.1136/bmj-2024-080785`.

The package uses the open 2025 BMJ explanation/elaboration as the preferred NotebookLM study source because it exposes the factorial design rationale, main comparisons and interaction concepts in more pedagogically useful detail.

The package explicitly notes that this is an extension built from CONSORT 2010/SPIRIT 2013 specialized guidance while CONSORT 2025 remains the current general reporting statement.

### Target-trial framework

Verified current article/full text:

- Hernán MA, Dahabreh IJ, Dickerman BA, Swanson SA;
- *The Target Trial Framework for Causal Inference From Observational Data: Why and When Is It Helpful?*;
- Ann Intern Med. 2025;178(3):402-407;
- DOI `10.7326/ANNALS-24-01871`;
- free full text available through PMC.

The package correctly limits the framework to observational causal intervention questions where a hypothetical trial can be coherently specified and does not imply that emulation creates randomized assignment.

---

## 4. Role assignment QA — PASS

Each source has an explicit role and non-overlapping instructional function.

### `CORE`

**Canonical F0.2 lesson**

Function:

- supplies the project's exact terminology;
- integrates all design classes into one reasoning algorithm;
- defines the required inference-boundary task;
- prevents NotebookLM from replacing curriculum logic with source-by-source summaries.

**Cochrane Chapter 23**

Function:

- anchors cluster/crossover architecture in an authoritative methods source;
- supports unit-of-allocation, clustering, within-person comparison and crossover suitability.

### `SUPPORT`

**CONSORT 2025**

Function:

- teaches which randomized-trial architecture/reporting elements should be visible;
- reinforces current reporting standard status.

**Factorial guidance**

Function:

- supplies specialized factor/main-comparison/interaction architecture not efficiently taught by the general CONSORT statement alone.

**STROBE**

Function:

- anchors the three major analytical observational designs and reporting distinctions.

### `CONTRAST`

**Target-trial framework**

Function:

- contrasts an ideal randomized causal design with observational emulation;
- reinforces that better design specification is not equivalent to actual randomization.

No source is assigned a role it was not designed to fulfill.

---

## 5. Required F0-A05 learning-sequence coverage — PASS

The study guide explicitly forces all elements required by the canonical `NEXT_ACTION`.

### Unfamiliar design classification

Pass 9 requires mixed unseen study descriptions and forbids revealing the design label before learner classification.

### Between-subject versus within-subject

Pass 2 explicitly contrasts randomized parallel and crossover structures and requires the learner to justify the comparison unit.

### Washout/carryover

Pass 2 requires definitions, biological suitability judgments, chronic-counterexample construction and period-effect reasoning.

### Unit-of-allocation logic

Pass 3 requires explicit separation of allocation, observation and dependence/analysis structure in multiple cluster scenarios.

### Cohort/case-control/cross-sectional discrimination

Pass 5 deliberately mixes prospective and retrospective datasets so the learner cannot use the word `retrospective` as a shortcut.

### Acute-versus-chronic inferential boundary

Pass 6 repeatedly forces rewriting of exaggerated chronic claims to match the actual measured acute outcome/time scale.

### Target-trial limits

Pass 8 requires full introductory target-trial specification and asks what observational emulation still cannot create.

### Strongest defensible versus tempting unsupported inference

This pair is mandatory:

- in Pass 1;
- in cluster exercises;
- in observational classification;
- in mixed final classification;
- in the manifest's active-recall and NotebookLM task instructions.

The package therefore tests inferential restraint as a repeated habit rather than a single end-of-module question.

---

## 6. Answer-leakage control — PASS

Excluded from the initial NotebookLM corpus:

- F0.2 `ANSWER_KEY.md`;
- F0.2 `EXERCISES.md`;
- F0.2 production `QA_REPORT.md`;
- full `SOURCE_INDEX.md`.

`EXERCISES.md` remains the independent first-pass assessment and is opened only after NotebookLM-guided study.

The study guide explicitly instructs NotebookLM to:

- present questions one at a time;
- wait for the learner's answer;
- grade only after the attempt;
- avoid revealing design labels in unfamiliar scenarios.

---

## 7. Scientific-boundary QA — PASS

The package does **not** prematurely teach F0.3 as though it were already mastered.

It permits introductory statements such as:

- randomization strengthens causal comparability in expectation;
- temporal ordering alone is insufficient for causal attribution;
- non-randomized allocation requires additional assumptions/structure;
- target-trial emulation does not eliminate unmeasured confounding by declaration.

It intentionally defers formal treatment of:

- confounding pathways;
- selection bias;
- measurement/information bias;
- missing-data mechanisms;
- collider bias;
- causal diagrams;
- identification assumptions;
- formal risk-of-bias judgments.

This preserves the F0.2 → F0.3 prerequisite boundary.

---

## 8. Reporting-guideline misuse QA — PASS

The package repeatedly states:

- CONSORT = reporting guidance for randomized trials;
- STROBE = reporting guidance for observational designs;
- factorial CONSORT extension = specialized reporting/protocol guidance;
- checklist completeness ≠ low risk of bias;
- reporting completeness ≠ correct causal inference;
- reporting guideline ≠ universal evidence hierarchy.

This is consistent with the canonical evidence policy and F0 architecture.

---

## 9. Pedagogical QA — PASS

The package sequence progresses from:

`design-reading algorithm → randomized structures → crossover → cluster → factorial → observational discrimination → acute/chronic boundary → question-specific design choice → target-trial thinking → mixed unfamiliar classification`

This order preserves conceptual dependency and avoids drowning the learner in taxonomy.

The learner is repeatedly required to:

- retrieve without answer exposure;
- generate original examples;
- compare near-neighbor designs;
- reject keyword-based classification;
- justify design against the scientific question;
- state inferential limits.

The package is therefore appropriate for `K1`, `K3`, `K4`, `K5`, `K6` and `K8` practice, with later integration/retesting still required for higher mastery states.

---

## 10. Public-repository/copyright QA — PASS

The public GitHub package contains only:

- project-authored Markdown;
- bibliographic citations;
- official/public source links;
- study instructions.

No third-party copyrighted PDF has been copied into the repository.

The guide tells the learner to use official/open pages or upload files personally when needed rather than republish restricted third-party documents in the public project.

No personal, clinical or sensitive learner information is persisted.

---

## 11. Learner-state integrity — PASS

Before package creation:

- F0.1 learner state: pending / no observed validation;
- F0.2 learner state: `UNSEEN`.

After package creation:

- no learner-state transition is authorized;
- package readiness is production metadata only;
- `MASTERED` remains impossible without observed performance and later cumulative retesting.

---

## 12. Final Study Package gate

Question:

> Can a capable learner use this small, auditable corpus to learn F0.2 study architecture, classify unfamiliar designs, preserve time/allocation/comparison logic, distinguish acute from chronic inference, understand target-trial limits, and repeatedly state both the strongest defensible and tempting unsupported inference—without contaminating the independent assessment or importing F0.3 prematurely?

**Decision:** yes.

**Package state:** `READY_FOR_STUDY`.
