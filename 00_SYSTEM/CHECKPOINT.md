# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-09
**Canonical branch:** `main`
**Project state:** `F0_5_STUDY_PACKAGE_READY`

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
- canonical distinctions remain: variable meaning before summary; sample versus population; parameter versus statistic; sample distribution versus sampling distribution; SD versus SE; larger n can reduce SE without automatically reducing individual SD or systematic bias;
- first-pass NotebookLM corpus uses canonical lesson, NIST EDA, Altman/Bland SD-SE note and ICH E9/E9(R1);
- `ENTRY_DIAGNOSTIC.md`, independent exercises and answer key remain outside the initial NotebookLM corpus;
- F0.4 quantitative diagnostic remains `UNOBSERVED` because no learner response has been observed.

### F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance

#### `F0-A10` — instructional unit

- complete approved unit exists at `foundations/F0-scientific-literacy/F0.5-estimates-confidence-pvalues-effect-sizes/` with `LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md` and production `QA_REPORT.md`;
- production QA passed CONTENT, EVIDENCE, PEDAGOGICAL and MASTERY gates;
- F0.5 separates parameter, estimator and estimate; point and interval estimates; SD versus SE; frequentist CI coverage; p-value interpretation; effect magnitude; practical thresholds and unsupported claims;
- frequentist 95% CI is a repeated-sampling procedure property under assumptions, not posterior probability that a fixed parameter lies inside one observed interval;
- all six ASA p-value principles are taught explicitly;
- `p<0.05` is not truth/importance and `p>0.05` is not proof of no effect;
- MD/SMD and RD/RR/OR remain distinct; RR and OR are not interchangeable;
- relative-effect interpretation requires baseline absolute context for practical meaning;
- smallest effect of interest / decision threshold is contextual and justified rather than generated from the observed p-value;
- narrow near-null intervals can be informative when they exclude meaningful effects; wide intervals can remain compatible with important benefit/harm;
- canonical interpretation sequence is `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`;
- formal Type I/II-error, power, multiplicity, FWER/FDR and analytical-flexibility machinery remain deferred to F0.6;
- `F0-S28` Greenland et al. 2016 was added for CI/p-value misinterpretation safeguards;
- all F0.5 methodological sources were rechecked on 2026-09-09.

#### `F0-A11` — NotebookLM study package

- complete package created at `notebooklm/F0.5-estimates-confidence-pvalues-effect-sizes/`;
- verified canonical files:
  - `MANIFEST.md`;
  - `STUDY_GUIDE.md`;
  - `QA_REPORT.md`;
- package decision: `PASS — READY_FOR_STUDY`;
- first-pass corpus intentionally limited to exactly six sources:
  1. canonical F0.5 lesson — `CORE`;
  2. Cochrane Handbook Chapter 6 — `CORE`;
  3. ASA Statement on p-values (2016) — `CORE`;
  4. Greenland et al. 2016 — `SUPPORT`;
  5. Lakens 2022 — `SUPPORT`;
  6. ASA Task Force 2021 — `CONTRAST`;
- source roles are intentionally non-redundant: Cochrane anchors effect-measure scales; ASA 2016 anchors six p-value principles; Greenland targets CI/p-value misinterpretations; Lakens anchors smallest-effect/informativeness reasoning; ASA 2021 prevents the overcorrection that p-values are intrinsically useless;
- NIST and Altman/Bland remain registered methodological references but are not needed in the first-pass corpus because the canonical lesson carries the SD/SE bridge and Greenland supplies the CI safeguard;
- external verification on 2026-09-09 confirmed Cochrane Chapter 6 in Handbook v6.5 (chapter last updated August 2023), the official ASA p-value statement, Greenland open-access PMC article, Lakens 2022 UCP article and ASA Task Force 2021 page;
- no source-version change required modification of the approved F0.5 lesson;
- study sequence repeatedly enforces the six-block interpretation format and requires correct null values before interpretation;
- frequentist CI training explicitly blocks posterior-probability language;
- p-value training requires all six ASA principles plus explicit repair of false statements rather than simple true/false labeling;
- practice includes p-small/practically-trivial, p-large/imprecise, and precise-near-null scenarios so threshold categories cannot substitute for magnitude/precision reasoning;
- MD/SMD practice rejects universal Cohen-label importance conclusions;
- RD/RR/OR practice requires baseline risk, absolute difference and explicit RR-versus-OR separation;
- practical-threshold practice distinguishes intervals entirely meaningful, entirely trivial, spanning multiple practical zones and precise exclusion of meaningful effects;
- ratio-scale practice preserves null `1` and reciprocal/log-scale intuition without pulling advanced meta-analysis forward;
- forest-plot-row and synthetic trial-table passes require the complete six-block interpretation;
- ASA 2016 versus ASA Task Force 2021 contrast explicitly rejects both `p<0.05 decides truth` and `p-values should always be banned`;
- F0.5 `EXERCISES.md`, `ANSWER_KEY.md`, production QA, full source registry and F0.4 `ENTRY_DIAGNOSTIC.md` are excluded from the initial NotebookLM corpus;
- formal Type I/II error, power, multiplicity, FWER/FDR and analytical-flexibility machinery remains deferred to F0.6;
- no third-party full text was committed to GitHub; only project-authored Markdown, citations and links were added;
- package creation changed no learner state and did not change the F0.4 quantitative diagnostic.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.5 STUDY_PACKAGE_READY`.

F0.1–F0.5 each now have:

- approved instructional unit;
- independent active-recall/application assessment;
- commented answer key;
- production QA;
- approved NotebookLM study package.

F0.4 additionally has the quantitative entry diagnostic, which remains `UNOBSERVED`.

`F0.6 — Power, Type I/II error, multiplicity and analytical flexibility` is the next unproduced instructional unit.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from production activity.

## F0.5 canonical production/package decisions

- interpretation sequence is `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`;
- point estimate is not interpreted without scale/context and interval uncertainty when available;
- CI precision is not causal validity;
- frequentist confidence is repeated-sampling procedure coverage, not posterior probability of the fixed parameter;
- p-values are model-conditional outputs and never probability statements about H0;
- binary significance categories are insufficient summaries;
- p-value does not measure magnitude or practical importance;
- MD preserves original units; SMD standardizes by dispersion and has no universal practical-importance threshold;
- RD is absolute; RR and OR are relative ratio measures with null `1`; RR and OR remain distinct;
- relative effects require baseline absolute context for practical interpretation;
- smallest-effect/decision thresholds are contextual and justified independently of observed p-values;
- precise near-zero estimates may exclude effects considered important; wide intervals may leave meaningful benefit/harm unresolved;
- systematic bias, design validity and applicability remain separate from statistical precision;
- first-pass NotebookLM manifest v1 uses exactly six sources with `CORE`/`SUPPORT`/`CONTRAST` roles recorded above;
- F0.5 exercises and answer key remain outside the initial notebook to preserve independent assessment;
- formal power/multiplicity/analytical-flexibility machinery remains F0.6.

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner;
- F0.2 has not yet been studied or assessed by the learner;
- F0.3 has not yet been studied or assessed by the learner;
- F0.4 has not yet been studied or assessed by the learner;
- F0.4 quantitative diagnostic = `UNOBSERVED`;
- F0.5 has not yet been studied or assessed by the learner;
- approved NotebookLM guides exist for F0.1–F0.5;
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
- production can proceed while learner validation remains pending, but F0.5 learner validation requires F0.4 as P2 and F0.6 learner validation requires F0.4 + F0.5;
- F0.4 diagnostic remains `UNOBSERVED` until actual learner responses are produced.

## NEXT_ACTION

`F0-A12` — Produce the complete sixth instructional unit `F0.6 — Power, Type I/II error, multiplicity and analytical flexibility`. Use `COURSE_MAP.md`, `PREREQUISITE_GRAPH.md`, `ASSESSMENT_BLUEPRINT.md`, the approved F0.4/F0.5 units and current mapped quantitative/methodological sources. Create `foundations/F0-scientific-literacy/F0.6-power-multiplicity-analytical-flexibility/LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md` and production `QA_REPORT.md`. Explicitly teach Type I and Type II errors in repeated-use/decision-rule terms; alpha and beta; statistical power as a design- and assumed-effect-dependent pre-study probability rather than a posterior probability about one completed study; why post hoc/observed power is generally uninformative for interpreting an observed estimate; power versus precision; sample-size justification tied to inferential goal and smallest effect of interest; multiplicity from endpoints, time points, subgroups, models and stopping/analysis choices; family-wise false-positive risk at conceptual/applied level; endpoint hierarchies and multiplicity-adjustment concepts without turning the module into an exhaustive correction-method catalog; subgroup/secondary/exploratory analyses; researcher degrees of freedom / analytical flexibility; preregistration, trial registration, protocol and statistical analysis plan; and confirmatory versus exploratory outputs. Preserve F0.5 magnitude/CI interpretation and teach that an observed nonsignificant result cannot be rescued/interpreted by computed observed power. The performance task must audit a synthetic study with many outcomes/time points/subgroups/models, reconstruct the effective family of hypotheses, identify planned versus data-driven analyses, explain false-positive/informativeness consequences and propose a transparent prespecification/reporting strategy. Critical fails must include `power = probability H1 is true`, `1-power = probability this nonsignificant result is a false negative`, post hoc observed power as evidence for absence/presence of effect, treating many unadjusted tests as independent confirmatory proof, and treating preregistration as a guarantee of low bias. Keep full meta-analysis/heterogeneity machinery deferred to F0.7. Recheck current sources including CONSORT 2025, ASA 2016/2021, FDA multiple-endpoints guidance and Lakens 2022; add only sources actually used to `SOURCE_INDEX.md`; apply CONTENT/EVIDENCE/PEDAGOGICAL/MASTERY QA; preserve F0.1–F0.5 learner states and F0.4 diagnostic `UNOBSERVED`; then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.