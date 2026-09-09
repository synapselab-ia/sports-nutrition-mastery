# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-09
**Canonical branch:** `main`
**Project state:** `F0_7_UNIT_APPROVED`

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
- formal RoB 2/ROBINS-I/GRADE application remains deferred to F0.8;
- current `ROBINS-I V2` remains recorded as a draft posted 20 November 2025 and subject to change;
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
- family of hypotheses is claim/decision dependent;
- prespecification improves auditability but does not guarantee low bias/correct design;
- subgroup inference requires direct interaction reasoning;
- learner state remains unvalidated.

### F0.7 — Systematic reviews, meta-analyses and heterogeneity

#### `F0-A14` — instructional unit

- `F0-A14` completed: complete seventh instructional unit created and production QA passed;
- approved unit path: `foundations/F0-scientific-literacy/F0.7-systematic-reviews-meta-analysis-heterogeneity/`;
- verified canonical files on `main`:
  - `LESSON.md` — `APPROVED`;
  - `EXERCISES.md` — 100-point active-recall/application assessment;
  - `ANSWER_KEY.md` — commented scoring key;
  - `QA_REPORT.md` — CONTENT, EVIDENCE, PEDAGOGICAL and MASTERY gates passed;
- systematic review and meta-analysis are explicitly distinct; a review can legitimately avoid pooling when a meaningful common synthesis is not defensible;
- canonical review workflow is `Protocol/question → Eligibility → Search → Screening → Extraction → Study/result appraisal → Effect measure → Synthesis plan → Heterogeneity → Missing evidence → Interpretation`;
- PRISMA 2020 is taught as reporting transparency, not risk-of-bias/high-quality/high-certainty certification;
- effect-measure compatibility is required before pooling; same direction does not make MD/SMD/RR/OR numerically interchangeable;
- inverse-variance weighting is taught at P1 level as precision weighting, not study quality;
- fixed-effect and random-effects models are separated by target quantity/model assumptions; neither is universally superior;
- random effects is explicitly not a heterogeneity cure or bias correction;
- between-study variance `tau²` and prediction-interval intuition are introduced conceptually without advanced estimator derivations;
- forest-plot interpretation preserves F0.5 magnitude/CI reasoning and adds compatibility, weight/model, heterogeneity and synthesis-defensibility checks;
- clinical diversity, methodological diversity and statistical heterogeneity are separate concepts;
- I² is explicitly not percent of heterogeneous studies, quality score, proof of sameness when low or automatic pooling ban when high;
- pooling may be inappropriate when questions/constructs/scales/time horizons/unit structures are not sufficiently compatible or when a single average would be misleading;
- sensitivity analyses are framed as robustness checks for defensible assumptions, not result-shopping;
- subgroup/meta-regression reasoning preserves F0.6 multiplicity/prespecification and rejects `significant in A + nonsignificant in B = interaction`;
- post hoc subgroup/meta-regression patterns are hypothesis-generating rather than proven causes of heterogeneity;
- small-study effects are separated from publication/non-reporting bias; funnel asymmetry is not diagnostic and apparent symmetry is not proof of no missing evidence;
- formal ROB-ME/RoB/certainty/GRADE application remains deferred to F0.8;
- integrated 12-field review audit is `Review question → Eligibility → Search/selection → Extraction/unit structure → Effect compatibility → Study estimates/precision → Weight/model → Clinical/methodological heterogeneity → Statistical heterogeneity → Sensitivity/subgroup/meta-regression prespecification → Missing-evidence/small-study signals → Pooling/conclusion defensibility`;
- performance task uses a synthetic five-study heterogeneous MD synthesis plus one deliberately incompatible SMD study, multiple post hoc moderators, collinearity, funnel-plot overclaim and PRISMA overclaim;
- local assessment gate is `>=80/100 + no critical fail`, applicable only after observed learner performance.

#### F0.7 source/version decisions

- only already-registered `F0-S03`, `F0-S04`, `F0-S05`, `F0-S06` were used; no duplicate/new source ID was needed in `SOURCE_INDEX.md`;
- PRISMA 2020 rechecked on 2026-09-09 and remains the current general PRISMA statement with 27-item checklist plus expanded/abstract checklists and flow diagrams;
- `F0-S04` Cochrane Chapter 10 rechecked on 2026-09-09: current page remains *Analysing data and undertaking meta-analyses*, cites Handbook v6.5 and chapter last updated November 2024;
- Cochrane `Versions and changes` records patch-level `6.5.1` changes through 2026, but no listed patch replaces the Chapter-10 citation or alters the F0.7 methods used here;
- current Handbook landing page still labels the main edition `Version 6.5, 2024`;
- `F0-S05` current Cochrane core methods/Chapter 13 rechecked for missing-evidence/small-study reasoning; Chapter 13 remains last updated August 2024 and treats funnel asymmetry as a non-diagnostic small-study signal with multiple possible causes;
- `F0-S06` Cochrane Chapter 6 rechecked and remains last updated August 2023, supporting effect/data compatibility and log-scale ratio logic;
- no third-party full text was copied into the public repository;
- all numerical performance examples are synthetic and do not constitute nutrition/performance recommendations.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.7 APPROVED`.

F0.1–F0.6 each have:

- approved instructional unit;
- independent active-recall/application assessment;
- commented answer key;
- production QA;
- approved NotebookLM study package.

F0.7 now has:

- approved self-contained lesson;
- 100-point independent assessment;
- commented answer key;
- approved production QA.

The F0.7 NotebookLM study package is the next production artifact.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from production activity.

## F0.7 canonical production decisions

- systematic review is a structured evidence process; meta-analysis is a statistical combination and is optional;
- numerical pooling requires defensible compatibility of question, construct, scale, timepoint and unit structure;
- inverse-variance weight measures statistical precision, not methodological quality/certainty;
- fixed-effect and random-effects answer different model-dependent synthesis questions;
- random-effects average does not erase between-study heterogeneity;
- pooled CI for an average is not the same object as between-study spread/prediction interval;
- forest-plot interpretation starts with effect measure/null/magnitude/CI before pooled labels;
- clinical, methodological and statistical heterogeneity remain distinct;
- I² requires context and is never a quality/sameness/automatic-invalidity score;
- pooling is a scientific decision, not an obligatory final step;
- subgroup/meta-regression/sensitivity analyses must preserve F0.6 prespecification/multiplicity logic;
- small-study/funnel patterns are signals with multiple possible explanations, not publication-bias diagnostics;
- PRISMA is reporting guidance, not review-quality/risk-of-bias certification;
- formal body-of-evidence certainty/risk-of-bias/applicability machinery remains F0.8.

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner;
- F0.2 has not yet been studied or assessed by the learner;
- F0.3 has not yet been studied or assessed by the learner;
- F0.4 has not yet been studied or assessed by the learner;
- F0.4 quantitative diagnostic = `UNOBSERVED`;
- F0.5 has not yet been studied or assessed by the learner;
- F0.6 has not yet been studied or assessed by the learner;
- F0.7 has not yet been studied or assessed by the learner;
- approved NotebookLM guides exist for F0.1–F0.6;
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
- production can proceed while learner validation remains pending, but F0.7 learner validation requires F0.2 + F0.5 + F0.6 as P2 and F0.3 before formal risk-of-bias synthesis;
- F0.4 diagnostic remains `UNOBSERVED` until actual learner responses are produced.

## NEXT_ACTION

`F0-A15` — Produce the complete NotebookLM study package for `F0.7 — Systematic reviews, meta-analyses and heterogeneity`. Create `notebooklm/F0.7-systematic-reviews-meta-analysis-heterogeneity/MANIFEST.md`, `STUDY_GUIDE.md` and package `QA_REPORT.md` using the approved F0.7 lesson and a deliberately limited, auditable corpus drawn only from sources needed for the learning objectives. Assign `CORE`/`SUPPORT`/`CONTRAST` roles and explain each source’s instructional function and limitation. The package must repeatedly distinguish systematic review from meta-analysis; reconstruct protocol/question/eligibility/search/screening/extraction/synthesis workflow; require effect-measure/construct/timepoint/unit compatibility before pooling; teach inverse-variance weight as precision rather than quality; distinguish fixed-effect from random-effects target quantities and reject `random effects solves heterogeneity`; interpret forest plots using F0.5 magnitude/CI reasoning plus compatibility/weight/model/heterogeneity/pooling-defensibility; distinguish clinical, methodological and statistical heterogeneity; train I² misconception repair including low-I² sameness and high-I² automatic-invalidity traps; compare pooled-mean CI with prediction/between-study variation at conceptual level; require justified pooling/no-pooling decisions; apply F0.6 prespecification/multiplicity safeguards to sensitivity, subgroup and meta-regression analyses; teach small-study effects/missing evidence and funnel-plot asymmetry as non-diagnostic; and preserve PRISMA as reporting guidance rather than risk-of-bias/high-quality certification. Include the integrated synthetic heterogeneous review audit with the incompatible SMD study and require the 12-field F0.7 audit sequence. Keep F0.7 `EXERCISES.md` and `ANSWER_KEY.md` outside the initial NotebookLM corpus so independent assessment remains uncontaminated; keep F0.4 `ENTRY_DIAGNOSTIC.md` outside and preserve it as `UNOBSERVED`. Recheck every external source/link/version used in the manifest, apply STUDY PACKAGE QA plus copyright/public-repository controls, preserve F0.1–F0.7 learner states as pending, keep formal RoB/GRADE/applicability machinery deferred to F0.8, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.