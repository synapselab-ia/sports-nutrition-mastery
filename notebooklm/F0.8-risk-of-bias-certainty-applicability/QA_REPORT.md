# F0.8 — NotebookLM Package QA Report

**Package:** `notebooklm/F0.8-risk-of-bias-certainty-applicability/`
**Manifest version:** `1`
**QA date:** `2026-09-09`
**Decision:** `PASS — READY_FOR_STUDY`
**Learner-state change authorized:** no
**F0.4 quantitative diagnostic:** unchanged; `UNOBSERVED`

## 1. Scope checked

This QA applies only to the F0.8 NotebookLM study package:

- `MANIFEST.md`;
- `STUDY_GUIDE.md`;
- this `QA_REPORT.md`.

The approved instructional unit remains canonical at:

`foundations/F0-scientific-literacy/F0.8-risk-of-bias-certainty-applicability/`

The package does not modify the approved lesson, assessment or answer key.

---

## 2. Package-content gate

### Required files

- `MANIFEST.md` — present;
- `STUDY_GUIDE.md` — present;
- package `QA_REPORT.md` — present after this commit.

### Corpus size

First-pass corpus is deliberately limited to exactly **six sources**:

1. canonical F0.8 lesson — `CORE`;
2. riskofbias.info official RoB 2/ROBINS-I resource — `CORE`;
3. GRADE Book overview — `CORE`;
4. GRADE intervention-certainty principles — `SUPPORT`;
5. GRADE indirectness — `SUPPORT`;
6. STROBE — `CONTRAST`.

**Result:** PASS.

The corpus is small enough for auditability while still covering every F0-A17 objective with non-redundant functions.

---

## 3. Source-role QA

### Canonical F0.8 lesson — CORE

Function:

- exact project vocabulary;
- six-object separation;
- RoB 2/ROBINS-I/GRADE/applicability integration;
- synthetic cases;
- critical fails;
- thirteen-field audit;
- F0.9 boundary.

Limitation explicitly recorded:

- project-authored instructional synthesis, not independent methodological authority.

### F0-S07 riskofbias.info — CORE

Function:

- official current RoB 2 version/status;
- official current ROBINS-I V2 status;
- result-specific/domain-based tool framing;
- target-trial-linked non-randomized appraisal context.

Limitation explicitly recorded:

- tools structure judgment rather than create a total quality score;
- ROBINS-I V2 remains draft;
- protected tool documents are not republished.

### F0-S18 GRADE overview — CORE

Function:

- certainty purpose;
- four categories;
- five core downgrading domains;
- body/outcome framing;
- certainty-versus-recommendation distinction.

Limitation explicitly recorded:

- framework requires judgment and does not replace detailed appraisal/domain guidance.

### F0-S19 GRADE certainty principles — SUPPORT

Function:

- threshold/range-aware certainty;
- absolute-effect orientation;
- outcome/body-level assessment;
- basic versus structured-ROBINS-I NRSI starting approaches.

Limitation explicitly recorded:

- first-pass package does not reproduce advanced GRADE implementation as a rote algorithm.

### F0-S20 GRADE indirectness — SUPPORT

Function:

- evidence-versus-target PICO comparison;
- applicability/generalizability/transferability;
- baseline-risk implications;
- mechanism-based rather than automatic downgrade logic.

Limitation explicitly recorded:

- final applicability still requires a defined target and domain knowledge.

### F0-S02 STROBE — CONTRAST

Function:

- explicit reporting-versus-quality contrast;
- demonstrates that visibility/reporting guidance is not a validity instrument.

Limitation explicitly recorded:

- does not perform RoB, GRADE or causal appraisal.

**Result:** PASS.

No source is included merely to increase count. CONSORT and PRISMA are not duplicated into the first-pass corpus because the canonical lesson already teaches their analogous reporting role and STROBE provides the cleanest explicit external contrast statement.

---

## 4. External source/link/version verification

All external sources actually used in manifest v1 were rechecked on `2026-09-09`.

### RoB 2

Official riskofbias.info page confirms:

- current version for individually randomized parallel-group trials = `22 August 2019`;
- cluster/crossover variants are separate and not silently treated as the same instrument.

Package wording matches this status.

### ROBINS-I V2

Official riskofbias.info page confirms:

- revised V2 posted `20 November 2025`;
- still a **draft**;
- explicitly subject to change/refinement.

Package never labels V2 as finalized.

### GRADE overview

Current GRADE Book page confirms:

- last modified `12 May 2026`;
- four certainty categories;
- core risk-of-bias, inconsistency, indirectness, imprecision and dissemination-bias reasoning;
- separation of certainty and recommendation strength.

### GRADE principles for intervention certainty

Current GRADE Book page confirms:

- last modified `21 August 2025`;
- certainty is confidence that the effect lies in a decision-relevant range or relative to a threshold;
- certainty is assessed across the body/outcome rather than as a paper label;
- both conventional low-start and structured-ROBINS-I high-start approaches for NRSI are described.

### GRADE indirectness

Current GRADE Book page confirms:

- last modified `12 May 2026`;
- PICO alignment is central;
- applicability/generalizability/transferability are explicitly connected to indirectness;
- differences should matter plausibly for effect transfer or absolute impact rather than trigger automatic downgrading.

### STROBE

Official STROBE site continues to state:

- recommendations concern reporting observational research;
- recommendations are not prescriptions for study design/conduct;
- checklist is not an instrument for evaluating observational-study quality.

**Result:** PASS.

No recheck identified a source-version change requiring revision of the approved F0.8 lesson or source registry.

---

## 5. F0-A17 requirement coverage

### Separate reporting, appraisal, RoB, certainty, applicability and recommendation strength

Covered repeatedly in:

- manifest objectives/claims;
- Study Guide Passes 1–3 and 16–17;
- integrated audit fields 2, 4–5, 11–13.

**PASS.**

### Result-specific/domain-based RoB 2 without total score

Covered in:

- manifest critical fails;
- Study Guide Passes 3–4;
- integrated field 4–5;
- explicit prohibition on domain summation/quality scoring.

**PASS.**

### Current RoB 2 and ROBINS-I V2 status preserved

RoB 2 `22 August 2019` and ROBINS-I V2 `20 November 2025 draft` are both required recall items and source-verification fields.

**PASS.**

### Target-trial reasoning without observational dismissal

Covered in:

- manifest objectives/claims;
- Study Guide Pass 6;
- Body B integrated audit.

The package blocks both `observational=useless` and `large adjusted study=randomized enough`.

**PASS.**

### Four GRADE categories and five core downgrade domains

Both are explicit closed-book recall requirements.

**PASS.**

### Preserve F0.5 imprecision reasoning

Study Guide Pass 13 requires estimate + CI + `+1.0` threshold reasoning before p-values and distinguishes meaningful/trivial/harm-compatible ranges.

**PASS.**

### Preserve F0.7 inconsistency/missing-evidence reasoning

Study Guide Passes 11 and 14 prohibit I2-only certainty judgments and funnel symmetry/asymmetry diagnoses.

**PASS.**

### Evidence-versus-target applicability comparison

Study Guide Pass 12 requires population, intervention/exposure, comparator, outcome, time horizon, setting and decision context.

**PASS.**

### Internal validity versus applicability

Study Guide Pass 16 uses an explicit two-axis grid.

**PASS.**

### Certainty versus recommendation strength

Study Guide Pass 17 requires additional decision information before recommendation judgment.

**PASS.**

### Integrated two-body comparison

The canonical synthetic scenario is reproduced with:

- Body A: four randomized trials, `MD +1.5 [1.2, 1.8]`, consistent effects and close target alignment;
- Body B: five non-randomized cohorts, `MD-equivalent +1.6 [-0.2, 3.4]`, confounding/selection/measurement/directness concerns and wide variation;
- practical-benefit threshold = `+1.0`.

The learner must complete all thirteen fields before synthesis.

**PASS.**

---

## 6. Scientific-boundary QA

The package explicitly rejects:

- `CONSORT/STROBE/PRISMA complete = low risk/high quality`;
- total quality scores as substitutes for bias mechanisms;
- `randomized = automatically low risk`;
- `observational = automatically unusable`;
- `low certainty = no effect`;
- `high certainty = large/important effect`;
- `statistical significance = high certainty`;
- `direct evidence = unbiased evidence`;
- representative sampling as a repair for internal bias;
- certainty as a paper-level prestige score;
- certainty of one outcome as recommendation strength;
- ROBINS-I V2 as finalized;
- I2-only inconsistency judgments;
- funnel symmetry/asymmetry as a dissemination-bias diagnosis;
- p-value-only imprecision judgments.

**Result:** PASS.

---

## 7. Pedagogical QA

### Progression

The 18-pass sequence progresses from:

`object separation → reporting contrast → result-specific RoB → RoB 2 → bias vs precision → ROBINS-I/target trial → design-label limits → GRADE certainty → starting approaches → five certainty-domain applications → validity/applicability → recommendation boundary → integrated audit`

This respects the project progression from accessible distinction to applied integration.

### Active retrieval

Every major concept is first recalled without sources and then checked against the approved corpus.

### Misconception repair

The guide contains explicit repair tasks for all critical fails named in F0-A17/F0-A16.

### Transfer

The integrated task forces comparison of two superficially similar pooled estimates and requires causal/statistical/applicability reasoning rather than memorized vocabulary.

### Prerequisite preservation

The package actively reuses:

- F0.3 bias mechanisms;
- F0.5 magnitude/CI/threshold reasoning;
- F0.7 heterogeneity/missing-evidence reasoning.

It does not pretend F0.8 can be mastered while those structural dependencies remain broken.

**Result:** PASS.

---

## 8. Mastery/assessment-contamination QA

Initial corpus excludes:

- `foundations/F0-scientific-literacy/F0.8-risk-of-bias-certainty-applicability/EXERCISES.md`;
- `foundations/F0-scientific-literacy/F0.8-risk-of-bias-certainty-applicability/ANSWER_KEY.md`;
- production `QA_REPORT.md`;
- F0.4 `ENTRY_DIAGNOSTIC.md`;
- F0.9 full-paper practicum materials.

The Study Guide includes analogous practice but does not reproduce the independent assessment answer key.

No learner performance was observed during package construction.

Therefore:

- F0.8 learner state remains pending/`UNSEEN`;
- no `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` state is authorized;
- F0.4 diagnostic remains `UNOBSERVED`.

**Result:** PASS.

---

## 9. Copyright/public-repository QA

Committed files contain only:

- project-authored Markdown;
- bibliographic citations;
- official URLs;
- synthetic educational cases.

No RoB 2/ROBINS-I tool PDF/template, GRADE protected content file, journal PDF or other third-party full text was copied into the repository.

The riskofbias.info tools currently state a CC BY-NC-ND license; the package therefore links to official pages and does not redistribute/modify tool documents.

No personal, clinical or sensitive user data are present.

**Result:** PASS.

---

## 10. Authority/noise QA

First-pass NotebookLM corpus excludes:

- full `SOURCE_INDEX.md`;
- redundant reporting guidelines beyond the single STROBE contrast source;
- exhaustive RoB tool documents;
- full ROB-ME implementation;
- exhaustive GRADE chapters;
- Evidence-to-Decision panel procedures;
- F0.9 full-paper content;
- substantive nutrition efficacy literature.

This reduces retrieval noise and prevents later-course material from displacing the F0.8 competency.

**Result:** PASS.

---

## 11. Final gate

Question:

> Can a capable learner use this package to understand what reporting reveals, judge result-level bias mechanisms, reason about body/outcome certainty, assess target applicability, preserve uncertainty and recognize the recommendation boundary without hidden prerequisites or answer-key leakage?

**Decision:** YES.

## Final decision

`PASS — READY_FOR_STUDY`

The package is ready for controlled first-pass NotebookLM study. Production completion does not imply learner study or mastery.
