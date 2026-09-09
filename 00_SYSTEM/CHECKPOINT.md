# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-09
**Canonical branch:** `main`
**Project state:** `F0_8_UNIT_APPROVED`

## Completed

### Project foundation

- public repository initialized;
- canonical `AGENTS.md` / `START_HERE.md` resume protocol established;
- project mission/scope, privacy/public-repository policy, evidence policy, research protocol, pedagogical standard, QA gates and mastery protocol created;
- NotebookLM protocol/manifest pattern created;
- macro curriculum, source registry/claim ledger and learner/mastery/error/study-history artifacts initialized;
- `F0-A01` completed: F0.1–F0.10 architecture, prerequisite graph and exit-assessment blueprint created.

### F0.1 — Scientific questions, hypotheses and operationalization

- `F0-A02` completed: approved instructional unit;
- `F0-A03` completed: approved NotebookLM package;
- canonical reasoning begins with `question → target population → contrast → outcome → time → estimand`;
- learner state remains unvalidated.

### F0.2 — Study designs and what they can answer

- `F0-A04` completed: approved instructional unit;
- `F0-A05` completed: approved NotebookLM package;
- design reasoning remains architecture-first; target-trial emulation remains a design benchmark rather than retroactive randomization;
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
- canonical distinctions remain sample/population, parameter/statistic, sample distribution/sampling distribution and SD/SE;
- larger n may reduce SE without reducing individual SD or systematic bias;
- F0.4 quantitative diagnostic remains `UNOBSERVED`.

### F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance

- `F0-A10` completed: approved instructional unit, independent assessment, answer key and production QA;
- `F0-A11` completed: approved NotebookLM package;
- canonical interpretation remains `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`;
- frequentist CI is not posterior probability; p-value is not `P(H0|data)` and does not measure importance;
- MD/SMD and RD/RR/OR remain distinct; relative effects require baseline absolute context;
- learner state remains unvalidated.

### F0.6 — Power, Type I/II error, multiplicity and analytical flexibility

- `F0-A12` completed: approved lesson, 100-point assessment, answer key and production QA;
- `F0-A13` completed: approved NotebookLM study package;
- power remains a prospective effect/design/assumption-dependent repeated-use quantity, not probability that H1 is true;
- `1−power` is not posterior false-negative probability for one observed result;
- observed/post hoc power calculated from the observed effect is not an interpretation tool;
- completed-study interpretation remains estimate + CI + practical threshold;
- multiplicity includes endpoints, time points, subgroups, models/analytical paths and stopping/data-dependent choices;
- prespecification improves auditability but does not guarantee low bias/correct design;
- learner state remains unvalidated.

### F0.7 — Systematic reviews, meta-analyses and heterogeneity

#### `F0-A14` — instructional unit

- `F0-A14` completed: approved F0.7 lesson, 100-point independent assessment, commented answer key and production QA;
- systematic review and meta-analysis are distinct; pooling is optional and requires defensible compatibility;
- inverse-variance weighting is precision weighting, not study quality/certainty;
- fixed-effect and random-effects models target different model-dependent quantities;
- random effects does not erase, explain or repair heterogeneity;
- pooled-mean CI is not the same object as between-study spread/prediction interval;
- clinical, methodological and statistical heterogeneity remain distinct;
- I² is not a quality/sameness/automatic-invalidity score;
- subgroup/meta-regression/sensitivity analyses preserve F0.6 prespecification/multiplicity/direct-comparison safeguards;
- small-study/funnel signals are non-diagnostic for publication/non-reporting bias;
- PRISMA is reporting guidance, not risk-of-bias/certainty certification.

#### `F0-A15` — NotebookLM study package

- `F0-A15` completed: approved F0.7 NotebookLM package at `notebooklm/F0.7-systematic-reviews-meta-analysis-heterogeneity/`;
- package decision: `PASS — READY_FOR_STUDY`;
- first-pass corpus uses exactly five sources: canonical lesson, Cochrane Chapters 10/6/13 and PRISMA 2020;
- integrated study task requires the canonical 12-field F0.7 audit;
- F0.7 exercises/answer key and F0.4 diagnostic remain outside the initial notebook;
- learner state remains unvalidated.

### F0.8 — Risk of bias, certainty of evidence and applicability

#### `F0-A16` — instructional unit

- `F0-A16` completed: complete eighth instructional unit created and production QA passed;
- approved unit path: `foundations/F0-scientific-literacy/F0.8-risk-of-bias-certainty-applicability/`;
- verified canonical files on `main`:
  - `LESSON.md` — `APPROVED`;
  - `EXERCISES.md` — 100-point independent assessment;
  - `ANSWER_KEY.md` — commented scoring key;
  - `QA_REPORT.md` — CONTENT, EVIDENCE, PEDAGOGICAL and MASTERY gates passed;
- F0.8 explicitly separates reporting completeness, broad critical appraisal, result-level risk of bias, certainty of a body of evidence, applicability/transportability and recommendation strength;
- CONSORT/STROBE/PRISMA are used only as reporting-transparency resources and never as low-risk/high-quality certification;
- risk of bias is result-specific and domain-based rather than a single study-quality score;
- bias and imprecision remain distinct: a precise estimate can be systematically biased;
- RoB 2 is taught at conceptual/applied domain level for individually randomized parallel-group trials with the five domains randomization process, deviations from intended interventions, missing outcome data, outcome measurement and selection of reported result;
- randomized design is explicitly not treated as automatically low risk of bias;
- current RoB 2 version rechecked on 2026-09-09 remains `22 August 2019` for individually randomized parallel-group trials;
- ROBINS-I target-trial logic is taught as a benchmark for non-randomized intervention-effect studies, not retroactive randomization;
- current `ROBINS-I V2` was rechecked on 2026-09-09 and remains the revised **draft posted 20 November 2025**, explicitly subject to change;
- current Nov-2025 ROBINS-I V2 draft is represented with six main domains: confounding, classification of intervention, selection into the study, missing data, outcome measurement and selection of reported result, plus triage to Critical risk when appropriate;
- observational/non-randomized evidence is explicitly not treated as automatically unusable;
- GRADE certainty is taught at body-of-evidence + outcome/question level rather than as a prestige label for a paper;
- current four certainty categories are `High`, `Moderate`, `Low`, `Very low`;
- core downgrading domains taught are risk of bias, inconsistency, indirectness, imprecision and dissemination/publication/non-reporting bias;
- current GRADE principles are taught as threshold/range aware, preserving F0.5 magnitude + CI + practical/decision-threshold reasoning;
- high certainty is explicitly compatible with a trivial/near-null effect; low certainty is explicitly not evidence of no effect;
- statistical significance is explicitly not a certainty rating;
- intervention-effect RCT bodies generally start high in basic GRADE reasoning; NRSI generally start low, while the advanced structured-ROBINS-I approach allowing NRSI to start high and then be rated down is explicitly acknowledged rather than hidden;
- F0.7 heterogeneity reasoning is preserved in the inconsistency domain: I² alone does not determine a certainty downgrade;
- current GRADE indirectness/applicability reasoning compares evidence PICO to target PICO and extends operationally to time horizon, setting and decision context;
- internal validity and applicability remain separate: direct evidence can still be biased and low-bias evidence can remain narrowly applicable;
- dissemination/missing-evidence reasoning preserves F0.7 funnel/small-study safeguards and does not diagnose publication bias from symmetry/asymmetry alone;
- certainty of one outcome is kept distinct from recommendation strength, which may additionally depend on net effects, other outcomes, values, resources, equity, acceptability and feasibility;
- integrated evidence-body task compares two synthetic bodies with similar point estimates but materially different bias, consistency, directness, precision and applicability;
- required 13-field F0.8 audit is `Target question/outcome → Reporting visibility → Design/effect of interest → Result-level RoB mechanisms → RoB judgment/rationale → Body estimate + threshold → Inconsistency → Indirectness → Imprecision → Missing/dissemination evidence → Overall certainty → Applicability to target → Recommendation-strength boundary`;
- local assessment gate is `>=80/100 + no critical fail`, applicable only after observed learner performance;
- critical fails include reporting-checklist certification, total quality-score substitution, randomized=low-risk, observational=unusable, low-certainty=no-effect, high-certainty=large-effect, significance=high-certainty, direct=unbiased, representative-sample-as-internal-bias-repair, certainty=paper-score, certainty=recommendation strength and ROBINS-I V2 mislabeled as finalized;
- formal full-paper integrated appraisal remains F0.9.

#### F0.8 source/version decisions

- only already-registered `F0-S01`, `F0-S02`, `F0-S03`, `F0-S05`, `F0-S07`, `F0-S18`, `F0-S19`, `F0-S20` were used; no duplicate/new source ID was needed in `SOURCE_INDEX.md`;
- riskofbias.info rechecked on 2026-09-09: RoB 2 current individually randomized version remains 22 August 2019; ROBINS-I V2 remains draft 20 November 2025 and subject to change;
- Cochrane Handbook landing page remains Version 6.5 (2024); Chapter 8 continues to describe RoB 2 as result-specific/domain-based for randomized trials;
- GRADE overview rechecked on 2026-09-09: current living chapter last modified 12 May 2026, with four certainty categories and the five principal downgrading domains;
- GRADE intervention-certainty principles rechecked: current chapter last modified 21 August 2025 and uses body/outcome, threshold/range-aware reasoning including nuanced RCT/NRSI starting approaches;
- GRADE indirectness rechecked: current chapter last modified 12 May 2026 and links PICO mismatch to material effect/absolute-impact transfer concerns rather than automatic downgrade for every difference;
- STROBE official site continues to state that its checklist is for reporting and is not an instrument to evaluate study quality;
- PRISMA 2020 remains the main PRISMA reporting guideline with a 27-item checklist and supporting expanded/abstract/flow materials;
- no third-party full text was copied into the public repository;
- all athlete/intervention examples are synthetic methodological examples and not substantive nutrition recommendations.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.8 APPROVED`.

F0.1–F0.7 have approved instructional units and approved NotebookLM study packages.

F0.8 now has:

- approved self-contained lesson;
- 100-point independent assessment;
- commented answer key;
- approved production QA.

The F0.8 NotebookLM study package is the next production artifact.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from production activity.

## F0.8 canonical production decisions

- reporting completeness, risk of bias, certainty, applicability and recommendation strength must remain separate objects;
- RoB judgments are result-specific/domain-based, not total study-quality scores;
- randomized design prevents some bias mechanisms but does not certify a result;
- non-randomized evidence requires explicit confounding/selection reasoning but is not dismissed by label;
- ROBINS-I V2 Nov-2025 must be labeled as a draft until its official status changes;
- GRADE certainty is body/outcome/question specific and threshold/range aware;
- certainty describes confidence in the effect range, not effect magnitude itself;
- F0.5 magnitude/CI/threshold reasoning remains mandatory for imprecision;
- F0.7 heterogeneity/missing-evidence reasoning remains mandatory for inconsistency/dissemination-bias judgments;
- applicability requires a mechanism-based comparison of evidence versus target population/intervention/comparator/outcome/time/setting/context;
- internal validity and applicability are not interchangeable;
- certainty of one outcome does not determine recommendation strength;
- full F0.1–F0.8 integration on an actual complete paper remains F0.9.

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
- approved NotebookLM guides exist for F0.1–F0.7;
- no mastery-state change is authorized from curriculum production alone.

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
- F0.8 learner validation requires F0.2 + F0.3 + F0.5 + F0.7 as P2;
- F0.9 learner validation requires F0.1–F0.8;
- F0.4 diagnostic remains `UNOBSERVED` until actual learner responses are produced.

## NEXT_ACTION

`F0-A17` — Produce the complete NotebookLM study package for `F0.8 — Risk of bias, certainty of evidence and applicability`. Create `notebooklm/F0.8-risk-of-bias-certainty-applicability/MANIFEST.md`, `STUDY_GUIDE.md` and package `QA_REPORT.md` using the approved F0.8 lesson and a deliberately limited, auditable corpus drawn only from sources needed for the learning objectives. Assign `CORE`/`SUPPORT`/`CONTRAST` roles and explain each source’s instructional function and limitation. The package must repeatedly separate reporting completeness, broad critical appraisal, result-level risk of bias, body/outcome certainty, applicability/transportability and recommendation strength; require result-specific/domain-based RoB 2 reasoning without total quality scores; preserve the current RoB 2 version and ROBINS-I V2 Nov-2025 **draft** status; train target-trial reasoning for non-randomized intervention studies without treating observational evidence as automatically unusable; require the four GRADE certainty categories and the core risk-of-bias/inconsistency/indirectness/imprecision/dissemination-bias reasoning; preserve F0.5 magnitude + CI + decision-threshold reasoning for imprecision and F0.7 heterogeneity/missing-evidence reasoning for inconsistency/dissemination bias; compare evidence versus target population, intervention/exposure, comparator, outcome, time horizon, setting and decision context; distinguish internal validity from applicability; and keep certainty of one outcome distinct from recommendation strength. Include the integrated synthetic two-evidence-body comparison and require the 13-field F0.8 audit sequence. Keep F0.8 `EXERCISES.md` and `ANSWER_KEY.md` outside the initial NotebookLM corpus so independent assessment remains uncontaminated; keep F0.4 `ENTRY_DIAGNOSTIC.md` outside and preserve it as `UNOBSERVED`. Recheck every external source/link/version actually used in the manifest, apply STUDY PACKAGE QA plus copyright/public-repository controls, preserve F0.1–F0.8 learner states as pending, keep full-paper practicum/integration deferred to F0.9, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.