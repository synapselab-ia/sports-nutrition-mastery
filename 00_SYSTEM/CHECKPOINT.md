# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-09
**Canonical branch:** `main`
**Project state:** `F0_6_STUDY_PACKAGE_READY`

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
- learner state remains unvalidated.

### F0.6 — Power, Type I/II error, multiplicity and analytical flexibility

#### `F0-A12` — instructional unit

- `F0-A12` completed: approved lesson, 100-point active-recall/application assessment, commented answer key and production QA;
- approved unit path: `foundations/F0-scientific-literacy/F0.6-power-multiplicity-analytical-flexibility/`;
- Type I/alpha and Type II/beta are taught in repeated-use/decision-rule terms rather than as posterior probabilities;
- power is defined as `1−beta` for a specified true effect/design/model and is explicitly not `P(H1 true)`;
- `1−power` is explicitly not the posterior probability that one nonsignificant result is a false negative;
- power is effect/design/assumption dependent and remains a prospective planning quantity;
- completed-study interpretation remains estimate + CI + practical threshold rather than observed-power rescue;
- observed/post hoc power calculated from the observed effect is explicitly rejected as an interpretation tool;
- sample-size justification follows inferential goal and can use a-priori power, desired precision/accuracy, near-census/population constraints, resource constraints or another transparent rationale;
- multiplicity is taught across endpoints, time points, subgroups, alternative models/analytical paths and stopping/data-dependent choices;
- family of hypotheses is claim/decision dependent rather than mechanically equal to every p-value in a paper;
- independent-test FWER arithmetic is used only as a simplified illustration and is not generalized to correlated outcomes;
- hierarchy/gatekeeping, alpha allocation/adjusted outputs and exploratory classification are taught conceptually without an exhaustive correction-method catalog;
- subgroup training rejects `significant in A + nonsignificant in B = interaction`;
- trial registration, preregistration, protocol and SAP are distinguished with timing/versioning/deviation checks;
- prespecification improves auditability but does not guarantee low bias or correct design;
- confirmatory versus exploratory outputs are separated without treating exploratory science as invalid;
- integrated audit sequence is `Target claims → Decision rules → Power/sample-size assumptions → Effective hypothesis family → Analytical paths → Prespecification evidence → Multiplicity control → Estimate/CI interpretation → Confirmatory vs exploratory → Transparent conclusion`;
- full systematic-review/meta-analysis/heterogeneity machinery remains deferred to F0.7.

#### `F0-A13` — NotebookLM study package

- `F0-A13` completed: complete F0.6 NotebookLM package created at `notebooklm/F0.6-power-multiplicity-analytical-flexibility/`;
- verified canonical files on `main`:
  - `MANIFEST.md`;
  - `STUDY_GUIDE.md`;
  - `QA_REPORT.md`;
- package decision: `PASS — READY_FOR_STUDY`;
- first-pass corpus intentionally limited to exactly eight sources:
  1. canonical F0.6 lesson — `CORE`;
  2. ASA Statement on p-values 2016 — `CORE`;
  3. FDA *Multiple Endpoints in Clinical Trials* 2022 — `CORE`;
  4. Lakens 2022 *Sample Size Justification* — `CORE`;
  5. Greenland et al. 2016 — `SUPPORT`;
  6. Heinsberg & Weeks 2022 — `SUPPORT`;
  7. CONSORT 2025 — `SUPPORT`;
  8. ASA Task Force 2021 — `CONTRAST`;
- source roles are intentionally non-redundant: ASA 2016 anchors threshold/transparency safeguards; FDA anchors multiple-endpoint/family architecture; Lakens anchors sample-size justification; Greenland anchors probability-reversal/error-rate safeguards; Heinsberg & Weeks anchors observed-power misuse; CONSORT anchors registration/protocol/SAP/deviation auditability; ASA 2021 prevents categorical p-value abolition;
- external verification on 2026-09-09 confirmed:
  - ASA official six-principle statement remains accessible;
  - FDA multiple-endpoints guidance remains Final Guidance dated October 2022;
  - Lakens 2022 remains accessible at University of California Press;
  - Greenland et al. 2016 and Heinsberg & Weeks 2022 remain accessible in PMC;
  - CONSORT 2025 remains the current general CONSORT statement, superseding CONSORT 2010, with 30 items and explicit registration/protocol/SAP/change-reporting provisions;
  - ASA Task Force 2021 remains accessible and continues to emphasize uncertainty, variability, multiplicity, replicability, model choice and selective reporting while retaining properly used p-values/significance tests as statistical tools;
- no source-version/access change required modification of the approved F0.6 lesson;
- study sequence uses 17 ordered passes from alpha/beta/power definitions through observed-power traps, sample-size goals, FWER/family reconstruction, analytical paths, subgroup interaction, degrees of freedom, registration/protocol/SAP, confirmatory/exploratory classification and integrated auditing;
- package repeatedly rejects `power=P(H1 true)`, `1−power=P(this nonsignificant result is false negative)`, observed-power rescue, nominal-p-value cherry-picking across many analyses, subgroup significance comparison as interaction proof and preregistration as low-bias certification;
- simple `1−.95^m` FWER exercises always require independent-test/all-null assumptions and a warning against universal application to correlated outcomes;
- sample-size practice contrasts a-priori power, desired precision, near-census, resource constraints and other transparent justifications instead of enforcing a universal target-power convention;
- analytical-flexibility practice separates hypothesis multiplicity from alternative model/outlier/covariate/time-window paths while preserving selection-risk reasoning;
- document-audit practice distinguishes trial registration, preregistration, protocol and SAP and requires timestamp/version/deviation checks;
- integrated study task reproduces the F0.6 synthetic many-outcome/timepoint/subgroup/model audit and requires all ten audit fields;
- F0.5 magnitude/CI/practical-threshold interpretation remains mandatory in every completed-study audit;
- F0.6 `EXERCISES.md`, `ANSWER_KEY.md`, production QA, full `SOURCE_INDEX.md` and F0.4 `ENTRY_DIAGNOSTIC.md` remain outside the initial NotebookLM corpus;
- full meta-analysis, heterogeneity/I², publication-bias methods and meta-regression remain deferred to F0.7;
- no third-party full text was committed to the public repository; package files contain only project-authored Markdown, citations and links;
- package creation changed no learner state and did not change the F0.4 quantitative diagnostic.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.6 STUDY_PACKAGE_READY`.

F0.1–F0.6 each now have:

- approved instructional unit;
- independent active-recall/application assessment;
- commented answer key;
- production QA;
- approved NotebookLM study package.

F0.4 additionally has the quantitative entry diagnostic, which remains `UNOBSERVED`.

`F0.7 — Systematic reviews, meta-analyses and heterogeneity` is the next unproduced instructional unit.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from production activity.

## F0.6 canonical production/package decisions

- alpha and beta/power are repeated-use properties conditional on procedure/effect/design/model assumptions, not posterior probabilities about one study;
- power must always be tied to an assumed effect and design;
- prospective power is a planning concept; observed precision/CI is the primary post-study uncertainty object;
- observed/post hoc power based on the observed effect is not an independent explanation of nonsignificance;
- sample-size justification follows inferential goal rather than a universal power convention;
- multiplicity is about confirmatory families/claims and data-dependent selection opportunities, not merely the count of printed p-values;
- alternative models may be analytical paths rather than independent scientific hypotheses, but data-driven path selection still threatens interpretation/error control;
- subgroup conclusions require direct interaction reasoning rather than comparison of significance labels;
- registration/preregistration/protocol/SAP are distinct evidence about prespecification and require timing/versioning/deviation audit;
- prespecification creates auditability, not guaranteed validity;
- exploratory findings are legitimate when transparently labeled;
- F0.5 magnitude/CI/practical-threshold reasoning remains mandatory for completed-study interpretation;
- first-pass NotebookLM manifest v1 uses exactly eight sources with `CORE`/`SUPPORT`/`CONTRAST` roles recorded above;
- F0.6 exercises and answer key remain outside the initial notebook to preserve independent assessment;
- full systematic-review/meta-analysis/heterogeneity machinery remains F0.7.

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner;
- F0.2 has not yet been studied or assessed by the learner;
- F0.3 has not yet been studied or assessed by the learner;
- F0.4 has not yet been studied or assessed by the learner;
- F0.4 quantitative diagnostic = `UNOBSERVED`;
- F0.5 has not yet been studied or assessed by the learner;
- F0.6 has not yet been studied or assessed by the learner;
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

`F0-A14` — Produce the complete seventh instructional unit `F0.7 — Systematic reviews, meta-analyses and heterogeneity`. Use `COURSE_MAP.md`, `PREREQUISITE_GRAPH.md`, `ASSESSMENT_BLUEPRINT.md`, the approved F0.2/F0.5/F0.6 units and current mapped evidence-synthesis sources. Create `foundations/F0-scientific-literacy/F0.7-systematic-reviews-meta-analysis-heterogeneity/LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md` and production `QA_REPORT.md`. Explicitly teach the systematic-review workflow from protocol/question/eligibility/search/screening/extraction to synthesis; distinguish systematic review from meta-analysis; teach effect-measure compatibility before pooling; fixed-effect versus random-effects conceptual models without presenting either as automatically superior; inverse-variance weighting intuition at P1 level; forest-plot anatomy and interpretation; statistical versus clinical/methodological heterogeneity; cautious interpretation of I² without treating it as a study-quality score or proof of homogeneity/heterogeneity by itself; when pooling is inappropriate; sensitivity analyses, subgroup analyses and meta-regression at conceptual level; small-study effects/publication bias at introductory level; and the role/limits of PRISMA as a reporting guideline rather than a risk-of-bias score. Preserve F0.5 magnitude/CI reasoning and F0.6 multiplicity/prespecification reasoning when interpreting review results. The performance task must require interpretation of a heterogeneous forest plot/evidence-synthesis summary, identification of effect scale and weighting logic, at least two plausible clinical/methodological explanations for heterogeneity before accepting a subgroup story, and a defensible judgment about whether/what should be pooled. Critical fails must include `pooled estimate = automatically true/superior`, `low I² = studies are clinically/methodologically identical`, `high I² = meta-analysis is automatically invalid`, `PRISMA-complete = low risk of bias/high study quality`, ignoring incompatible effect measures/scales before pooling, and treating a post hoc subgroup/meta-regression pattern as proven explanation of heterogeneity. Recheck current Cochrane Handbook/PRISMA and other mapped synthesis-method sources before authoring; add only sources actually used to `SOURCE_INDEX.md`; apply CONTENT/EVIDENCE/PEDAGOGICAL/MASTERY QA; preserve F0.1–F0.6 learner states and F0.4 diagnostic `UNOBSERVED`; then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.