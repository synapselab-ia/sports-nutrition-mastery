# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-09
**Canonical branch:** `main`
**Project state:** `F0_3_STUDY_PACKAGE_READY`

## Completed

### Project foundation

- public repository initialized;
- canonical agent/startup protocol created;
- project mission and scope defined;
- public-repository/privacy policy defined;
- evidence policy and research protocol defined;
- pedagogical standard and QA gates defined;
- mastery protocol defined;
- NotebookLM protocol and manifest pattern created;
- macro curriculum created;
- source registry and claim ledger initialized;
- learner, mastery, error and study-history artifacts initialized;
- F0 Scientific Literacy scaffold created;
- `F0-A01` completed: evidence-backed architecture for F0.1–F0.10, prerequisite graph and exit-assessment blueprint created.

### F0.1 — Scientific questions, hypotheses and operationalization

- `F0-A02` completed: full instructional unit created and QA-approved;
- `LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md` and `QA_REPORT.md` exist under `foundations/F0-scientific-literacy/F0.1-scientific-questions/`;
- sports-nutrition transfer exemplar `F0-S21` registered with explicit acute/mechanistic inferential limits;
- `F0-A03` completed: NotebookLM package created and Study Package QA passed;
- F0.1 NotebookLM package contains `MANIFEST.md`, `STUDY_GUIDE.md` and `QA_REPORT.md` and excludes the answer key/independent assessment from the initial corpus.

### F0.2 — Study designs and what they can answer

- `F0-A04` completed: full instructional unit created and QA-approved;
- `LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md` and `QA_REPORT.md` exist under `foundations/F0-scientific-literacy/F0.2-study-designs/`;
- F0.2 design-specific sources `F0-S22`–`F0-S25` registered with explicit version caveats relative to CONSORT 2025;
- `F0-A05` completed: NotebookLM package created and Study Package QA passed;
- F0.2 NotebookLM first-pass corpus is intentionally limited to six sources and repeatedly requires `Strongest defensible inference` plus `Tempting unsupported inference`.

### F0.3 — Bias, confounding, causal reasoning and validity

- `F0-A06` completed: full instructional unit created and QA-approved;
- `LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md` and `QA_REPORT.md` exist under `foundations/F0-scientific-literacy/F0.3-bias-confounding-causal-validity/`;
- F0.3 teaches counterfactual intuition, exchangeability, systematic versus random error, confounding/residual confounding, DAGs, confounder/mediator/collider roles, invalid adjustment, selection, measurement/information bias, misclassification, missingness/attrition, reverse causation, target-trial thinking, randomization limits and internal versus external validity/applicability;
- F0.3 assessment requires the applied reasoning sequence `target causal question/estimand → causal structure → distortion mechanism → adjustment/conditioning → repairability/data limitation → calibrated conclusion`;
- `F0-S26` (Feeney, Hartwig & Davies, BMJ 2025 DAG guide) registered for introductory DAG/causal-adjustment reasoning;
- `F0-A07` completed: complete NotebookLM study package created and Study Package QA passed;
- F0.3 NotebookLM manifest v1 created in `notebooklm/F0.3-bias-confounding-causal-validity/MANIFEST.md`;
- practical F0.3 NotebookLM setup/study sequence created in `notebooklm/F0.3-bias-confounding-causal-validity/STUDY_GUIDE.md`;
- F0.3 package QA/source-version/copyright/answer-leakage controls recorded in `notebooklm/F0.3-bias-confounding-causal-validity/QA_REPORT.md`;
- F0.3 initial corpus is intentionally limited to six sources: canonical F0.3 lesson, Hernán & Robins `Causal Inference: What If`, BMJ 2025 DAG guide, Catalogue of Bias, official ROBINS-I V2 webpage and Hernán et al. 2025 target-trial framework;
- source roles: canonical lesson, `What If` and BMJ DAG guide are `CORE`; Catalogue of Bias and ROBINS-I V2 webpage are `SUPPORT`; target-trial framework is `CONTRAST`;
- package requires construction/critique of simple DAGs but explicitly treats arrows as causal assumptions, not empirical proof;
- package contrasts randomized and observational bias pathways stage by stage and preserves randomization as a strong treatment-assignment protection rather than a universal validity certificate;
- package separates target-trial design bias prevention from data limitations such as unmeasured confounding and never treats emulation as retroactive randomization;
- package keeps formal RoB 2/ROBINS-I/GRADE application deferred to F0.8;
- F0.3 `ANSWER_KEY.md` and `EXERCISES.md` are excluded from the initial NotebookLM corpus so assessment remains independent;
- external verification on 2026-09-09 confirmed the current authors' page for `Causal Inference: What If`, the 2025 BMJ DAG article, current Catalogue of Bias, current riskofbias.info pages and the 2025 target-trial full text;
- direct official verification corrected the ROBINS-I V2 project note: the revised V2 draft was posted **20 November 2025**, not 30 November 2025; the official page still labels it a **draft version subject to change** as of 2026-09-09;
- `SOURCE_INDEX.md` was updated on 2026-09-09 to preserve the corrected ROBINS-I V2 date/status and current checks for F0.3 package sources.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.3 STUDY_PACKAGE_READY`.

F0.1, F0.2 and F0.3 each have:

- an approved instructional unit;
- active-recall/application assessment;
- commented answer key;
- production QA;
- an approved NotebookLM study package.

`F0.4 — Descriptive statistics, distributions and sampling variation` is the next unproduced instructional unit.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`. Production approval and NotebookLM package readiness must not be interpreted as learner mastery.

## F0 architecture decisions now canonical

- F0.1–F0.10 are organized by conceptual dependency rather than a simple terminology sequence;
- reporting guidelines such as CONSORT/STROBE/PRISMA are never treated as study-quality/risk-of-bias scores;
- a quantitative entry diagnostic precedes learner validation of F0.4;
- isolated numeracy gaps are `P1` repairs; structural numeracy gaps promote the conditional `P2-QB` bridge before F0.4 learner progression;
- F0 exit requires integrated appraisal of a complete exercise/nutrition paper plus quantitative and evidence-synthesis interpretation;
- passing an initial assessment can support `APPLIED/INTEGRATED` but does not automatically establish `MASTERED`; later cumulative retesting is required;
- exercise/nutrition primary studies used for transfer are exemplars and must not be promoted into methodological authority or practical recommendations beyond their evidence;
- current methodological backbone includes CONSORT 2025, Cochrane Handbook v6.5 (2024), current risk-of-bias resources, ASA statistical-inference statements, causal-inference references, the 2025 BMJ DAG guide and the living GRADE Book current through 2026.

## F0.1 canonical production decisions

- teach `question → target population → contrast → outcome → time → estimand` before study-design choice;
- PICO(T) is a decomposition aid, not a quality checklist;
- construct, operational definition, variable, outcome/endpoint and estimand remain distinct;
- exploratory findings are legitimate hypothesis generation when transparently labeled and must not be rewritten as prespecified confirmation;
- acute mechanistic outcomes must not be silently converted into chronic hypertrophy/performance/health conclusions;
- local assessment gate is `>=80/100` plus no critical fail, applied only after observed learner performance.

## F0.1 NotebookLM package decisions

- first-pass corpus is small/auditable;
- canonical lesson is the project instructional spine;
- `ANSWER_KEY.md` and `EXERCISES.md` remain outside the initial corpus;
- package generation did not change learner state.

## F0.2 canonical production decisions

- study design is architecture relative to a scientific question, not a universal evidence pyramid;
- randomization strengthens causal comparability in expectation but does not guarantee flawless execution/generalization;
- parallel versus crossover is separated by between- versus within-subject architecture;
- crossover requires reversibility/stability and explicit washout/carryover/period reasoning;
- cluster trials distinguish allocation from observation/analysis units;
- retrospective cohort versus case-control is distinguished by sampling logic, not by age of records;
- acute mechanistic and chronic outcome studies answer different questions;
- target-trial emulation specifies a causal-design benchmark but does not create randomization;
- local assessment gate is `>=80/100` plus no critical fail, applied only after observed learner performance.

## F0.2 NotebookLM package decisions

- manifest v1 uses exactly six initial sources;
- reporting guidance remains reporting guidance, never a risk-of-bias score;
- all classification tasks preserve `design → strongest defensible inference → tempting unsupported inference`;
- answer key and independent exercises are excluded from the first-pass corpus;
- package generation did not change learner state.

## F0.3 canonical production decisions

- causal appraisal begins with the target causal question/estimand; covariate selection is downstream of that question;
- counterfactual/exchangeability reasoning is conceptual at F0.3, without requiring advanced potential-outcome mathematics;
- systematic bias is distinct from random error and larger sample size is not a universal bias cure;
- confounding is a causal/common-cause/open-path problem, not merely a statistically associated covariate;
- residual confounding includes unmeasured, poorly measured, coarsened/proxy and structurally misspecified causes;
- DAGs encode assumptions and audit causal structure; they do not prove arrows;
- confounder, mediator and collider roles are question/estimand-specific;
- mediator adjustment can change a total-effect estimand;
- collider conditioning/post-exposure selection can open non-causal paths;
- selection at entry, retention, complete-case status or analytical inclusion is analyzed by mechanism, not by representativeness slogans;
- measurement/information bias includes exposure, outcome and confounder measurement;
- non-differential misclassification is not universally assumed to bias toward the null;
- missingness/attrition is a causal process; percentages alone do not determine bias and complete-case analysis is not automatically neutral;
- reverse causation remains tied to temporal-ordering logic;
- randomization reduces baseline treatment-assignment confounding in expectation but does not eliminate post-randomization selection, missingness, measurement, adherence, analysis or reporting problems;
- target-trial thinking is a design benchmark, not a substitute for unavailable data;
- internal validity is distinct from external validity/generalizability/transportability/applicability;
- formal RoB 2/ROBINS-I/GRADE scoring and F0.4–F0.6 inferential-statistics machinery remain deliberately deferred;
- local assessment gate is `>=80/100` plus no critical fail, applied only after observed learner performance.

## F0.3 NotebookLM package decisions

- manifest version `1` uses exactly six initial sources;
- `CORE`: canonical F0.3 lesson, Hernán & Robins `Causal Inference: What If`, Feeney et al. 2025 BMJ DAG guide;
- `SUPPORT`: Catalogue of Bias and the current official ROBINS-I V2 webpage;
- `CONTRAST`: Hernán et al. 2025 target-trial framework;
- `What If` is used selectively at introductory conceptual depth; its full advanced longitudinal material is outside F0.3 scope;
- the official authors' page is preferred because the online book can be revised; the current linked PDF observed on 2026-09-09 was dated `19aug26`;
- the ROBINS-I V2 webpage is a boundary/version-literacy source only; the current November 2025 V2 remains draft and formal tool application belongs to F0.8;
- every applied NotebookLM task requires `Target causal question/estimand → Causal structure → Distortion mechanism → Adjustment/conditioning → Repairability/data limitation → Calibrated conclusion`;
- DAG prompts require explicit assumptions and at least some counterfactual/alternative-structure challenge rather than rote node labeling;
- source comparison distinguishes causal foundations, DAG reasoning, bias taxonomy, operational RoB domains and target-trial design logic;
- `ANSWER_KEY.md`, `EXERCISES.md`, production QA, full source registry and formal RoB/GRADE documents are excluded from the first-pass corpus;
- package creation changed no learner state.

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner.
- F0.2 has not yet been studied or assessed by the learner.
- F0.3 has not yet been studied or assessed by the learner.
- approved F0.1 NotebookLM sequence: `notebooklm/F0.1-scientific-questions/STUDY_GUIDE.md`;
- approved F0.2 NotebookLM sequence: `notebooklm/F0.2-study-designs/STUDY_GUIDE.md`;
- approved F0.3 NotebookLM sequence: `notebooklm/F0.3-bias-confounding-causal-validity/STUDY_GUIDE.md`;
- F0.4 quantitative entry diagnostic has not been taken by the learner;
- no mastery-state change is authorized from curriculum/package production alone.

## Operational constraints

- repository is public;
- never persist sensitive personal/health data;
- do not publish copyrighted PDFs without redistribution permission;
- current scientific claims must be researched and sourced rather than generated from memory alone;
- NotebookLM is a study layer; GitHub remains canonical;
- living/versioned methodological sources must be rechecked when materially relevant to a new production action;
- current `ROBINS-I V2` status must remain labeled as draft until official status changes;
- causal DAGs encode assumptions and must never be represented as proof that a causal structure is true;
- answer keys must not contaminate first-pass retrieval/application assessments;
- F0.4 production may proceed before F0.1–F0.3 learner validation, but F0.4 learner progression must respect prerequisite/diagnostic routing.

## NEXT_ACTION

`F0-A08` — Produce the complete fourth instructional unit `F0.4 — Descriptive statistics, distributions and sampling variation` and the quantitative entry diagnostic required before F0.4 learner validation. Use `COURSE_MAP.md`, `PREREQUISITE_GRAPH.md`, `ASSESSMENT_BLUEPRINT.md`, the approved F0.1–F0.3 units and current mapped quantitative sources. Create `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/ENTRY_DIAGNOSTIC.md` with a short independently scorable diagnostic covering fractions/ratios/percentages, percentage versus percentage-point change, one-step algebraic rearrangement, scientific notation, reading tables/basic x-y plots, mean-versus-median intuition and probability on 0–1/0–100% scales; define routing so isolated gaps remain `P1` repairs and structural failure promotes conditional `P2-QB`, but do **not** infer any learner deficit until actual responses are observed. Create the self-contained F0.4 `LESSON.md`, active-recall/application `EXERCISES.md`, commented `ANSWER_KEY.md` and production `QA_REPORT.md`. Explicitly teach variable types and measurement scales; mean, median, mode, range, variance, standard deviation, IQR and quantiles; distributions, skew and outliers; appropriate data visualization and misleading graph choices; sample versus population; sampling variability; sample distribution versus sampling distribution at an accessible conceptual level; standard deviation versus standard error; and transformations only at a conceptual level where they clarify skew/scales. Use exercise/nutrition-flavored numerical examples without turning them into substantive nutrition recommendations. The performance task must require choosing/justifying summaries for multiple datasets, detecting misleading visualizations and explaining what changes when sample size increases while underlying individual variability remains similar. Do **not** prematurely teach full confidence-interval/p-value/effect-size content reserved for F0.5 or power/multiplicity content reserved for F0.6. Research/recheck current quantitative-method sources when needed, add only sources actually used to `SOURCE_INDEX.md`, apply CONTENT/EVIDENCE/PEDAGOGICAL/MASTERY QA, preserve F0.1–F0.3 learning states and the F0.4 diagnostic state as unobserved, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.
