# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-09
**Canonical branch:** `main`
**Project state:** `F0_6_UNIT_APPROVED`

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
- design reasoning remains architecture-first and target-trial emulation remains a design benchmark rather than retroactive randomization;
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

- `F0-A08` completed: approved instructional unit plus quantitative entry diagnostic;
- `F0-A09` completed: approved NotebookLM package;
- canonical distinctions remain variable meaning before summary; sample versus population; parameter versus statistic; sample distribution versus sampling distribution; SD versus SE; larger n can reduce SE without automatically reducing individual SD or systematic bias;
- F0.4 quantitative diagnostic remains `UNOBSERVED` because no learner response has been observed.

### F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance

- `F0-A10` completed: approved instructional unit, independent assessment, answer key and production QA;
- `F0-A11` completed: approved NotebookLM package;
- canonical interpretation sequence remains `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`;
- frequentist CI is not posterior probability; p-value is not `P(H0|data)` and does not measure importance;
- MD/SMD and RD/RR/OR remain distinct; relative effects require baseline absolute context;
- smallest-effect/decision thresholds remain contextual;
- formal power/multiplicity/analytical-flexibility machinery is now taught in F0.6 rather than retrofitted into F0.5;
- learner state remains unvalidated.

### F0.6 — Power, Type I/II error, multiplicity and analytical flexibility

#### `F0-A12` — instructional unit

- `F0-A12` completed: complete sixth instructional unit created and production QA passed;
- approved unit path: `foundations/F0-scientific-literacy/F0.6-power-multiplicity-analytical-flexibility/`;
- verified canonical files on `main`:
  - `LESSON.md` — `APPROVED`;
  - `EXERCISES.md` — 100-point active-recall/application assessment;
  - `ANSWER_KEY.md` — commented scoring key;
  - `QA_REPORT.md` — CONTENT, EVIDENCE, PEDAGOGICAL and MASTERY gates passed;
- F0.6 defines Type I error/alpha and Type II error/beta in repeated-use/decision-rule terms rather than as posterior probabilities;
- power is defined as `1−beta` for a specified true effect/design/model and is explicitly a pre-study conditional rejection probability, not probability that H1 is true;
- a power statement is incomplete without the effect size and assumptions for which it was calculated;
- simple power-curve intuition is taught: power varies with the assumed effect, n, variability, alpha and design efficiency;
- power and precision are explicitly separated: prospective power describes behavior of a planned procedure under assumed effects, while post-study informativeness is read primarily from estimate + CI + practical threshold;
- post hoc/observed power calculated by substituting the observed effect is explicitly rejected as a completed-study interpretation tool;
- `1−power` is explicitly not the posterior probability that a specific nonsignificant result is a false negative;
- sample-size justification is tied to inferential goal and can use a-priori power, desired precision/accuracy, near-census/population constraints, resource constraints or another transparent rationale rather than a universal magic N;
- smallest effect of interest/planning effect is treated as a quantity that requires independent justification rather than being inferred from the observed p-value;
- multiplicity is taught across endpoints, time points, subgroups, alternative models/analytical paths and stopping/data-dependent choices;
- `family of hypotheses` is defined relative to scientific claims/decision strategy rather than mechanically as every p-value in a paper;
- illustrative FWER calculation `1−(1−alpha)^m` is explicitly restricted to the simplifying case of independent tests with relevant nulls true; worked values include m=5 ≈22.6% and m=20 ≈64.2%;
- conceptual multiplicity strategies include a prespecified primary endpoint, hierarchy/gatekeeping, alpha allocation/adjusted outputs and explicit exploratory classification;
- Bonferroni is used only as a simple illustration (`0.05/5=0.01`), not as a universally optimal correction;
- subgroup training explicitly rejects `significant in A + nonsignificant in B = interaction`; direct interaction estimation/testing plus CI/multiplicity/prespecification is required;
- researcher degrees of freedom / analytical flexibility includes outcome definitions, time windows, exclusions, missing-data handling, transformations, covariates, subgroups, models, analysis populations, outlier rules and stopping/reporting choices;
- trial registration, preregistration, protocol and SAP are distinguished rather than treated as synonyms;
- timing/versioning and transparent rationale for deviations are required for an audit trail;
- preregistration/prespecification improves transparency but is explicitly not a guarantee of low risk of bias, valid measurement, correct model or important effect;
- confirmatory versus exploratory outputs are separated without treating exploratory science as inherently invalid;
- integrated audit framework is `Target claims → Decision rules → Power/sample-size assumptions → Effective hypothesis family → Analytical paths → Prespecification evidence → Multiplicity control → Estimate/CI interpretation → Confirmatory vs exploratory → Transparent conclusion`;
- performance assessment audits a synthetic trial with 20 outcomes × 4 time points, multiple subgroup definitions and covariate models, selected favorable p-values, incomplete reporting and observed-power misuse;
- local assessment gate is `>=80/100 + no critical fail`, applicable only after observed learner performance;
- critical fails include `power=P(H1 true)`, `1−power=P(this result is false negative)`, observed-power rescue, many nominal unadjusted tests treated as independent confirmation, subgroup p-value comparison as interaction proof, preregistration as low-bias guarantee and ignoring estimate/CI in completed-study interpretation;
- full meta-analysis, heterogeneity/I², publication-bias methods and meta-regression remain deferred to F0.7.

#### F0.6 source/version decisions

- `F0-S01` CONSORT 2025 rechecked on 2026-09-09; current 30-item general statement remains current and is used for trial registration, protocol/SAP access, prespecified versus post hoc transparency, timing/versioning and deviations; it remains a reporting guideline rather than a risk-of-bias score;
- `F0-S08` ASA 2016 rechecked on 2026-09-09; the six principles remain the p-value/transparency boundary;
- `F0-S09` ASA Task Force 2021 rechecked on 2026-09-09; used for uncertainty, variability, multiplicity, replicability and the balanced position that correctly used p-values remain statistical tools;
- `F0-S10` FDA *Multiple Endpoints in Clinical Trials* rechecked on 2026-09-09 and remains Final Guidance (October 2022); used conceptually for multiple-endpoint false-conclusion risk, grouping/ordering and multiplicity control without universalizing regulatory requirements to sports science;
- `F0-S13` Lakens 2022 rechecked on 2026-09-09 and now used for F0.6 sample-size justification, a-priori power, precision/accuracy and smallest-effect planning;
- `F0-S28` Greenland et al. 2016 remains the probability-reversal safeguard for p-values/CIs/power;
- new `F0-S29` added: Heinsberg LW, Weeks DE. *Post hoc Power is Not Informative*. Genetic Epidemiology. 2022;46(7):390-394. doi:10.1002/gepi.22464; used specifically to block observed/post hoc power as an interpretation of completed-study results;
- `SOURCE_INDEX.md` updated on 2026-09-09 with the F0.6 source rechecks and F0-S29;
- no third-party full text was copied into the public repository.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.6 APPROVED`.

F0.1–F0.5 each have an approved instructional unit and approved NotebookLM package.

F0.6 now has:

- approved self-contained lesson;
- 100-point active-recall/application assessment;
- commented answer key;
- approved production QA.

The F0.6 NotebookLM study package is the next production artifact.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from production activity.

## F0.6 canonical production decisions

- `alpha` and `beta/power` are repeated-use properties conditional on the statistical procedure and assumptions, not posterior probabilities about one study;
- power must always be tied to an assumed effect and design;
- prospective power is a planning concept; observed precision/CI is the primary post-study uncertainty object;
- observed/post hoc power based on the observed effect is not an independent explanation of nonsignificance;
- sample-size justification must follow the inferential goal rather than a universal power convention;
- multiplicity is about families/claims and selection opportunities, not merely the raw number of p-values printed;
- alternative models may represent analytical paths rather than independent scientific hypotheses, but data-driven path selection still threatens error control/interpretability;
- subgroup conclusions require direct interaction reasoning rather than comparing two significance labels;
- prespecification creates auditability, not guaranteed validity;
- exploratory findings are legitimate when labeled and interpreted as exploratory;
- F0.5 magnitude/CI/practical-threshold reasoning remains mandatory for completed-study interpretation;
- full systematic-review/meta-analysis/heterogeneity machinery remains F0.7.

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner;
- F0.2 has not yet been studied or assessed by the learner;
- F0.3 has not yet been studied or assessed by the learner;
- F0.4 has not yet been studied or assessed by the learner;
- F0.4 quantitative diagnostic = `UNOBSERVED`;
- F0.5 has not yet been studied or assessed by the learner;
- F0.6 has not yet been studied or assessed by the learner;
- approved NotebookLM guides exist for F0.1–F0.5;
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
- production can proceed while learner validation remains pending, but F0.6 learner validation requires F0.4 + F0.5 as P2;
- F0.4 diagnostic remains `UNOBSERVED` until actual learner responses are produced.

## NEXT_ACTION

`F0-A13` — Produce the complete NotebookLM study package for `F0.6 — Power, Type I/II error, multiplicity and analytical flexibility`. Create `notebooklm/F0.6-power-multiplicity-analytical-flexibility/MANIFEST.md`, `STUDY_GUIDE.md` and package `QA_REPORT.md` using the approved F0.6 lesson and a deliberately limited, auditable source corpus drawn only from sources needed for the learning objectives. Assign `CORE`/`SUPPORT`/`CONTRAST` roles and explain the instructional function and limitation of every source. The package must repeatedly require correct Type I/alpha versus Type II/beta reasoning; define power only relative to a specified effect/design and reject `power=P(H1 true)` or `1−power=P(this nonsignificant result is a false negative)`; distinguish prospective power from observed precision/CI; explicitly train against observed/post hoc power calculated from the observed effect; compare a-priori power, precision/accuracy and other transparent sample-size justifications; reconstruct effective families of confirmatory claims across endpoints/timepoints/subgroups and distinguish hypothesis multiplicity from analytical-path multiplicity; calculate/interpret simple illustrative family-wise false-positive risk without treating independent-test formulas as universal; reason about endpoint hierarchies/alpha allocation at conceptual level; audit subgroup and secondary analyses; identify researcher degrees of freedom; distinguish trial registration, preregistration, protocol and SAP with timing/versioning/deviation checks; and separate confirmatory from exploratory outputs without treating exploration as invalid. Preserve the F0.5 requirement to interpret completed results through magnitude + CI + practical threshold rather than observed power. Include an integrated synthetic study audit with many outcomes/time points/subgroups/models and require the ten-field F0.6 audit sequence. Keep F0.6 `EXERCISES.md` and `ANSWER_KEY.md` outside the initial NotebookLM corpus so independent assessment remains uncontaminated; keep the F0.4 entry diagnostic outside and preserve it as `UNOBSERVED`. Recheck every external source/link/version actually used in the manifest, apply STUDY PACKAGE QA plus copyright/public-repository controls, preserve F0.1–F0.6 learner states as pending, keep full meta-analysis/heterogeneity machinery deferred to F0.7, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.