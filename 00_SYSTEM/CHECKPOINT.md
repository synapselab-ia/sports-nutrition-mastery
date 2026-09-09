# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-09
**Canonical branch:** `main`
**Project state:** `F0_8_STUDY_PACKAGE_READY`

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
- verified canonical files on `main`:
  - `MANIFEST.md`;
  - `STUDY_GUIDE.md`;
  - `QA_REPORT.md`;
- package decision: `PASS — READY_FOR_STUDY`;
- first-pass corpus is intentionally limited to exactly six sources:
  1. canonical F0.8 lesson — `CORE`;
  2. riskofbias.info official RoB 2/ROBINS-I resource — `CORE`;
  3. GRADE Book overview — `CORE`;
  4. GRADE intervention-certainty principles — `SUPPORT`;
  5. GRADE indirectness — `SUPPORT`;
  6. STROBE — `CONTRAST`;
- source roles are deliberately non-redundant: riskofbias.info anchors current result-level tool/version status; GRADE overview anchors body/outcome certainty and recommendation separation; certainty principles anchor threshold/range and NRSI starting approaches; indirectness anchors evidence-versus-target transfer; STROBE provides the explicit reporting-versus-quality contrast;
- external verification on 2026-09-09 confirmed:
  - RoB 2 current individually randomized parallel-group version = `22 August 2019`;
  - ROBINS-I V2 = revised `20 November 2025` **draft**, subject to change;
  - GRADE overview last modified `12 May 2026`;
  - GRADE intervention-certainty principles last modified `21 August 2025`;
  - GRADE indirectness last modified `12 May 2026`;
  - STROBE continues to state its checklist is for reporting and not an observational-study quality instrument;
- no source-version change required revision of the approved F0.8 lesson;
- the Study Guide uses 18 ordered passes from object separation through reporting contrast, result-level RoB, RoB 2, bias-versus-precision, ROBINS-I/target-trial reasoning, GRADE domains, applicability, recommendation boundary and integrated audit;
- package repeatedly blocks reporting-checklist certification, total quality scores, randomized=low-risk, observational=unusable, low-certainty=no-effect, high-certainty=large-effect, significance=high-certainty, direct=unbiased, I²-only certainty judgments and funnel-based publication-bias diagnoses;
- integrated study task reproduces the synthetic two-body comparison:
  - Body A: four randomized trials, pooled `MD +1.5 [1.2, 1.8]`, consistent effects and close target alignment;
  - Body B: five non-randomized cohorts, pooled transformed `MD-equivalent +1.6 [-0.2, 3.4]`, confounding/selection/measurement/directness concerns and wide effect variation;
  - practical-benefit threshold `+1.0`;
- all thirteen F0.8 audit fields are required before final synthesis;
- F0.8 `EXERCISES.md`, `ANSWER_KEY.md`, production QA, full `SOURCE_INDEX.md` and F0.4 `ENTRY_DIAGNOSTIC.md` remain outside the initial NotebookLM corpus;
- no RoB tool PDF/template, GRADE source file or third-party full text was committed; only project-authored Markdown, citations, official links and synthetic cases were persisted;
- package creation changed no learner state and did not change the F0.4 quantitative diagnostic.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.8 STUDY_PACKAGE_READY`.

F0.1–F0.8 now have approved instructional units and approved NotebookLM study packages. F0.4 additionally has the quantitative entry diagnostic, still `UNOBSERVED`.

`F0.9 — Critical reading of a complete paper` is the next unproduced instructional unit.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from production activity.

## F0.8 canonical production/package decisions

- never collapse reporting, RoB, certainty, applicability or recommendation strength;
- RoB is result-specific/domain-based, not a total quality score;
- randomized/non-randomized labels inform but do not complete appraisal;
- ROBINS-I V2 Nov-2025 remains draft until official status changes;
- GRADE certainty is outcome/body/question specific and threshold/range aware;
- certainty describes confidence in an effect range, not effect magnitude itself;
- F0.5 estimate/CI/threshold reasoning remains mandatory for imprecision;
- F0.7 heterogeneity/missing-evidence reasoning remains mandatory for inconsistency/dissemination bias;
- applicability requires mechanism-based comparison of evidence versus target context;
- internal validity and applicability are separate axes;
- certainty of one outcome does not determine recommendation strength;
- first-pass F0.8 NotebookLM manifest v1 uses exactly six sources with roles recorded above;
- F0.8 exercises and answer key remain outside the initial notebook;
- full-paper integration across F0.1–F0.8 remains F0.9.

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
- approved NotebookLM guides exist for F0.1–F0.8;
- no mastery-state change is authorized from curriculum/package production alone.

## Operational constraints

- repository is public;
- never persist sensitive personal/health data;
- do not publish copyrighted PDFs/chapters/articles without redistribution permission;
- current methodological claims must be researched and sourced;
- NotebookLM is a study layer; GitHub remains canonical;
- living/versioned sources must be rechecked when materially relevant;
- answer keys and prerequisite diagnostics must not contaminate first-pass retrieval/assessment;
- synthetic sports/nutrition numerical examples must not become substantive nutrition recommendations;
- production can proceed while learner validation remains pending;
- F0.9 learner validation requires F0.1–F0.8 as P2;
- F0.4 diagnostic remains `UNOBSERVED` until actual learner responses are produced.

## NEXT_ACTION

`F0-A18` — Produce the complete ninth instructional unit `F0.9 — Critical reading of a complete paper`. Use `COURSE_MAP.md`, `PREREQUISITE_GRAPH.md`, `ASSESSMENT_BLUEPRINT.md`, all approved F0.1–F0.8 units and current mapped reporting/appraisal sources. Create `foundations/F0-scientific-literacy/F0.9-critical-reading-complete-paper/LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md` and production `QA_REPORT.md`. Teach a fixed full-paper appraisal sequence: `1. question/estimand → 2. design/sampling → 3. intervention/exposure/comparator → 4. outcome measurement → 5. bias/confounding/missingness → 6. sample size/analysis plan → 7. effect estimate/uncertainty → 8. multiplicity/exploration → 9. result robustness → 10. applicability → 11. consistency with authors’ conclusion → 12. what the paper does not establish`. Explicitly integrate F0.1 operationalization, F0.2 design limits, F0.3 bias/causal mechanisms, F0.4 descriptive/sampling reasoning, F0.5 magnitude/CI/practical thresholds, F0.6 power/multiplicity/prespecification, F0.7 synthesis context when relevant and F0.8 result-level RoB/certainty/applicability distinctions. Teach article anatomy and supplementary-material navigation at P0/P1 level; require extraction of a compact PICO/estimand table and result table before interpretation; distinguish primary, secondary, exploratory and post hoc findings using registration/protocol/SAP/timestamps where available; use reporting guidelines only to locate information and never as validity scores. The performance task must be a blind critical appraisal of one legally accessible full human exercise/nutrition paper with enough quantitative uncertainty and methodological detail for meaningful appraisal, preferably with registration/protocol/supplement access, followed by a structured answer key. The task must require explicit statements of the strongest defensible inference, the most material limitations, applicability, whether the authors’ conclusion is proportional, and what the paper does not prove. Critical fails must include abstract-only appraisal, design-label-only appraisal, checklist completion as a substitute for reasoning, `p<0.05 = important/true`, `p>0.05 = no effect`, observed-power rescue, ignoring prespecification/multiplicity, treating reporting completeness as low RoB, treating one RoB/certainty label as a substitute for result-specific reasoning, extrapolating acute/mechanistic outcomes to chronic performance/body-composition outcomes without support, and rewriting the authors’ conclusion without independently reconstructing the measured estimand/results. Recheck the current status of every reporting/appraisal source actually used and verify that the chosen assessment paper is legally accessible before authoring; add only sources actually used to `SOURCE_INDEX.md`; apply CONTENT/EVIDENCE/PEDAGOGICAL/MASTERY QA; preserve F0.1–F0.8 learner states and F0.4 diagnostic `UNOBSERVED`; then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.