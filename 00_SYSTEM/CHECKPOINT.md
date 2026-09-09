# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-09
**Canonical branch:** `main`
**Project state:** `F0_4_STUDY_PACKAGE_READY`

## Completed

### Project foundation

- public repository initialized;
- canonical `AGENTS.md` / `START_HERE.md` resume protocol established;
- project mission/scope, public-repository/privacy policy, evidence policy, research protocol, pedagogical standard, QA gates and mastery protocol created;
- NotebookLM protocol/manifest pattern created;
- macro curriculum, source registry/claim ledger and learner/mastery/error/study-history artifacts initialized;
- `F0-A01` completed: F0.1–F0.10 architecture, prerequisite graph and exit-assessment blueprint created.

### F0.1 — Scientific questions, hypotheses and operationalization

- `F0-A02` completed: approved instructional unit;
- `F0-A03` completed: approved NotebookLM package;
- canonical reasoning begins with `question → target population → contrast → outcome → time → estimand`;
- acute/mechanistic exemplars remain constrained to their measured outcome/time horizon;
- learner state remains unvalidated.

### F0.2 — Study designs and what they can answer

- `F0-A04` completed: approved instructional unit;
- `F0-A05` completed: approved NotebookLM package;
- design reasoning remains architecture-first: allocation, temporal direction, comparison structure, unit logic, strongest defensible inference and tempting unsupported inference;
- target-trial emulation remains a design benchmark rather than retroactive randomization;
- learner state remains unvalidated.

### F0.3 — Bias, confounding, causal reasoning and validity

- `F0-A06` completed: approved instructional unit;
- `F0-A07` completed: approved NotebookLM package;
- causal appraisal sequence remains `target causal question/estimand → causal structure → distortion mechanism → adjustment/conditioning → repairability/data limitation → calibrated conclusion`;
- DAGs encode assumptions and do not prove arrows;
- larger sample size is not represented as a cure for systematic bias;
- formal RoB 2/ROBINS-I/GRADE application remains deferred to F0.8;
- current `ROBINS-I V2` remains recorded as a draft posted 20 November 2025 and subject to change;
- learner state remains unvalidated.

### F0.4 — Descriptive statistics, distributions and sampling variation

#### `F0-A08` — instructional unit

- complete approved unit exists at `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/`;
- `ENTRY_DIAGNOSTIC.md`, `LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md` and production `QA_REPORT.md` exist;
- quantitative entry diagnostic covers eight independently scorable bridge domains: fraction/decimal/percentage, ratio/relative change, percentage versus percentage points, one-step algebra, scientific notation, table/basic x-y reading, mean-versus-median intuition and probability-scale conversion;
- diagnostic routing is defined as `READY_FOR_F0.4`, `P1_REPAIR` or conditional `P2-QB_REQUIRED` only from observed responses;
- no diagnostic response exists; diagnostic state remains `UNOBSERVED`;
- F0.4 teaches variable types/scales, mean/median/mode, range/sample variance/SD, quartiles/quantiles/IQR, distributions/skew/outliers, data visualization, population/sample, parameter/statistic, sampling variability, sample distribution versus sampling distribution, SD versus SE, sample-size intuition and conceptual transformations;
- right skew is defined by tail structure rather than the non-universal shortcut `mean > median`;
- outliers are investigated rather than automatically deleted;
- histogram is distinguished from bar chart;
- descriptive scatterplots do not authorize causal inference;
- sample variance uses `n−1` in worked examples and is labeled as sample variance;
- SD remains in the original unit while variance is in squared units;
- `SE(mean) ≈ SD/√n` is taught only in the simple independent-observation setting;
- increasing n can reduce sampling variability/SE while leaving individual-level SD and systematic bias intact;
- sample distribution is the distribution of observed values; sampling distribution is the distribution of a statistic across hypothetical repeated samples;
- transformations are scale changes, not methods for erasing bias or forcing a desired result;
- F0.4 independent assessment is 100 points with gate `>=80/100` plus no critical fail, applicable only after observed performance;
- `F0-S12` NIST/SEMATECH, `F0-S14` ICH E9/E9(R1) and `F0-S27` Altman & Bland are the registered F0.4 methodological sources;
- `F0-S27` specifically anchors SD-versus-SE reasoning.

#### `F0-A09` — NotebookLM study package

- complete package created at `notebooklm/F0.4-descriptive-statistics/`;
- verified files on canonical `main`:
  - `MANIFEST.md`;
  - `STUDY_GUIDE.md`;
  - `QA_REPORT.md`;
- package decision: `PASS — READY_FOR_STUDY`;
- first-pass corpus intentionally limited to exactly four sources:
  1. canonical F0.4 lesson — `CORE`;
  2. NIST/SEMATECH Chapter 1: Exploratory Data Analysis — `CORE`;
  3. Altman & Bland, *Standard deviations and standard errors* — `SUPPORT`;
  4. ICH E9/E9(R1) official EMA page — `CONTRAST`;
- NIST direct chapter endpoint `https://www.itl.nist.gov/div898/handbook/eda/eda.htm` is the preferred NotebookLM ingestion URL because it exposes actual EDA chapter content/navigation; the NIST modern publication record remains the bibliographic verification page;
- external verification on 2026-09-09 confirmed the NIST EDA chapter, BMJ Altman/Bland article and current EMA ICH E9/E9(R1) Step 5 status;
- no source-version change required modification of the approved F0.4 lesson;
- NotebookLM sequence repeatedly requires `variable type → distribution features → center → dispersion → visualization → outlier/anomaly plan → bounded conclusion` where applicable;
- mixed practice explicitly covers population/sample, parameter/statistic, sample versus sampling distribution, SD versus SE and larger-n prediction;
- `SE(mean) ≈ SD/√n` remains limited to the simple F0.4 mean example; clustered/paired/weighted/model-based standard errors are not generalized from it;
- package requires the learner to predict that larger n can lower mean SE without automatically lowering individual SD, systematic bias, selection problems, confounding or causal uncertainty;
- outlier training alternates data-entry error, measurement failure, plausible rare observations and unresolved anomalies so deletion cannot be a keyword response;
- visualization audit includes truncated axes, hidden individual distributions, incompatible scales, selective windows and histogram-bin choices;
- ICH E9/E9(R1) is used only as a boundary/contrast source showing that descriptive summaries do not independently define a treatment-effect estimand;
- `ENTRY_DIAGNOSTIC.md`, `EXERCISES.md`, `ANSWER_KEY.md`, production QA and full source registry are excluded from the initial NotebookLM corpus;
- diagnostic integrity rule is explicit: if the diagnostic is still `UNOBSERVED`, honest learner validation requires completing it independently before F0.4 study;
- full CI/p-value/effect-size interpretation remains deferred to F0.5;
- formal power, Type I/II error and multiplicity remain deferred to F0.6;
- no third-party copyrighted PDF/chapter text was committed to the public repository;
- package creation changed no learner or diagnostic state.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.4 STUDY_PACKAGE_READY`.

F0.1–F0.4 now each have an approved instructional unit. F0.1–F0.4 also have approved NotebookLM packages, with F0.4 additionally containing the prerequisite quantitative entry diagnostic.

`F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance` is the next unproduced instructional unit.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`.

## F0 architecture decisions now canonical

- curriculum order follows conceptual dependency, not calendar order;
- production may proceed before learner validation, but learner states must respect prerequisites;
- reporting guidelines are never converted into risk-of-bias/quality scores;
- exercise/nutrition examples used for methodological transfer remain synthetic or explicitly bounded exemplars rather than recommendations;
- F0 exit requires integrated paper appraisal plus quantitative/evidence-synthesis interpretation;
- a first strong assessment can support progression evidence but not automatic `MASTERED`; later cumulative retesting is required;
- F0.4 learner validation requires the quantitative bridge evidence before progression;
- no `P1_REPAIR` or `P2-QB_REQUIRED` state can be assigned without observed diagnostic responses.

## F0.4 canonical production decisions

- variable meaning and distribution inspection precede summary selection;
- nominal/ordinal/interval/ratio scales are reasoning aids rather than a mechanical analysis selector;
- `always report mean ± SD` is rejected as a universal rule;
- median/IQR are robust options in relevant distributions but not universally superior;
- quantile conventions can differ slightly in small samples and must be specified when material;
- visualizations are analytical objects, not decoration;
- truncated axes are analyzed for their effect on perception rather than mechanically prohibited;
- sample/population and parameter/statistic remain distinct;
- sample distribution and sampling distribution remain distinct;
- SD and SE describe different objects;
- larger n can improve statistic stability/precision without automatically shrinking the underlying individual distribution;
- observed range can become wider in larger samples;
- systematic bias from F0.3 remains distinct from sampling variation;
- full confidence-interval/p-value/effect-size content remains F0.5;
- formal power/Type I–II error/multiplicity remains F0.6.

## F0.4 NotebookLM package decisions

- manifest version `1` uses exactly four initial sources;
- `CORE`: canonical lesson + NIST EDA;
- `SUPPORT`: Altman & Bland SD/SE note;
- `CONTRAST`: ICH E9/E9(R1) for question/target/analysis boundary;
- NIST direct EDA chapter is preferred over the bibliographic landing page for NotebookLM retrieval;
- initial corpus excludes diagnostic, exercises, answer key and QA metadata;
- learner must classify the statistical object before formula use;
- SD/SE tasks require object meaning before calculation;
- sample-size tasks explicitly ask what does **not** change automatically;
- CI/p-values/effect sizes/power/multiplicity must not be introduced as F0.4 solutions;
- package creation did not change learner state or diagnostic state.

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner;
- F0.2 has not yet been studied or assessed by the learner;
- F0.3 has not yet been studied or assessed by the learner;
- F0.4 has not yet been studied or assessed by the learner;
- F0.4 quantitative diagnostic = `UNOBSERVED`;
- approved NotebookLM guides exist for F0.1, F0.2, F0.3 and F0.4;
- no mastery-state change is authorized from curriculum/package production alone.

## Operational constraints

- repository is public;
- never persist sensitive personal/health data;
- do not publish copyrighted PDFs/chapters without redistribution permission;
- current methodological claims must be researched and sourced;
- NotebookLM is a study layer; GitHub remains canonical;
- living/versioned sources must be rechecked when materially relevant;
- answer keys and prerequisite diagnostics must not contaminate first-pass retrieval/assessment;
- synthetic sports/nutrition numerical examples must not become substantive nutrition recommendations;
- production can proceed to F0.5 while F0.1–F0.4 learner validation remains pending, but F0.5 learner validation requires F0.4 as P2.

## NEXT_ACTION

`F0-A10` — Produce the complete fifth instructional unit `F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance`. Use `COURSE_MAP.md`, `PREREQUISITE_GRAPH.md`, `ASSESSMENT_BLUEPRINT.md`, the approved F0.4 unit and current mapped quantitative sources. Create `foundations/F0-scientific-literacy/F0.5-estimates-confidence-pvalues-effect-sizes/LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md` and production `QA_REPORT.md`. Explicitly teach point estimates and interval estimates; the frequentist meaning and common misinterpretations of confidence intervals; p-values and all six core ASA cautions; why magnitude and precision are more informative than a binary significance label; raw versus standardized effect sizes; mean difference and standardized mean difference; risk difference, risk ratio and odds ratio at conceptual/applied level; absolute versus relative effects; smallest effect of interest/decision-threshold intuition; statistical versus practical importance; and compatibility/range-of-plausible-effect reasoning without converting CI into a Bayesian posterior statement. Preserve the F0.4 distinction between SD and SE and show how standard error participates in uncertainty without reteaching F0.4 as a formula-only prerequisite. The performance task must require interpretation of a forest-plot row and a small synthetic trial table in plain language, explicitly separating direction, magnitude, precision, statistical output, practical importance and what remains unsupported. Include critical-fail protections against `p<0.05 = important/true`, `p>0.05 = no effect`, `95% CI = 95% probability the fixed true parameter lies inside this observed interval`, relative effects without absolute baseline context, and standardized effect sizes treated as intrinsically clinically meaningful. Keep formal Type I/II-error operating characteristics, power calculations, multiplicity and analytical-flexibility machinery deferred to F0.6, while allowing only the minimum conceptual bridge needed to interpret F0.5 outputs. Research/recheck current statistical-method sources before authoring, add only sources actually used to `SOURCE_INDEX.md`, apply CONTENT/EVIDENCE/PEDAGOGICAL/MASTERY QA, preserve F0.1–F0.4 learner states and the F0.4 diagnostic as `UNOBSERVED`, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.
