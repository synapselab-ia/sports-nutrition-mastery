# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-09
**Canonical branch:** `main`
**Project state:** `F0_4_UNIT_APPROVED`

## Completed

### Project foundation

- public repository initialized;
- canonical agent/startup protocol created;
- project mission/scope, public-repository policy, evidence policy, research protocol, pedagogical standard, QA gates and mastery protocol created;
- NotebookLM protocol/manifest pattern created;
- macro curriculum, source registry/claim ledger and learner/mastery/error/study-history artifacts initialized;
- `F0-A01` completed: F0.1–F0.10 architecture, prerequisite graph and exit-assessment blueprint created.

### F0.1 — Scientific questions, hypotheses and operationalization

- `F0-A02` completed: approved instructional unit with `LESSON.md`, `EXERCISES.md`, `ANSWER_KEY.md` and `QA_REPORT.md`;
- `F0-A03` completed: approved NotebookLM package;
- acute sports-nutrition exemplars remain explicitly constrained to their measured outcomes/time horizons.

### F0.2 — Study designs and what they can answer

- `F0-A04` completed: approved instructional unit;
- `F0-A05` completed: approved NotebookLM package;
- design reasoning remains architecture-first: allocation, temporal direction, comparison structure, unit logic, strongest defensible inference and tempting unsupported inference;
- crossover/cluster/factorial source-version caveats remain explicit relative to CONSORT 2025.

### F0.3 — Bias, confounding, causal reasoning and validity

- `F0-A06` completed: approved instructional unit;
- `F0-A07` completed: approved NotebookLM package;
- causal appraisal sequence remains `target causal question/estimand → causal structure → distortion mechanism → adjustment/conditioning → repairability/data limitation → calibrated conclusion`;
- DAGs encode causal assumptions and are not proof generators;
- target-trial emulation remains a design benchmark, not retroactive randomization;
- formal RoB 2/ROBINS-I/GRADE application remains deferred to F0.8;
- current `ROBINS-I V2` remains recorded as a draft posted 20 November 2025, subject to change.

### F0.4 — Descriptive statistics, distributions and sampling variation

- `F0-A08` completed: complete fourth instructional unit created and production QA passed;
- new unit path: `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/`;
- `ENTRY_DIAGNOSTIC.md` created with eight independently scorable quantitative bridge domains: fraction/decimal/percentage conversion, ratio/relative change, percentage versus percentage-point change, one-step algebra, scientific notation, table/basic x-y reading, mean-versus-median intuition and probability-scale conversion;
- diagnostic routing defined as `READY_FOR_F0.4`, `P1_REPAIR` or conditional `P2-QB_REQUIRED` only after observed responses;
- no diagnostic response exists; current diagnostic state remains `UNOBSERVED`;
- F0.4 `LESSON.md` created and approved;
- F0.4 explicitly teaches categorical nominal/ordinal and numerical discrete/continuous variables; nominal/ordinal/interval/ratio measurement-scale reasoning; mean, median, mode, range, sample variance, SD, quartiles/quantiles and IQR; symmetry/skew/outliers; graph selection and misleading visualizations; population/sample; parameter/statistic; sampling variation; sample distribution versus sampling distribution; SD versus SE; sample-size intuition; and transformations at conceptual level only;
- right skew is defined by tail structure rather than the non-universal shortcut `mean > median`;
- outliers are investigated rather than automatically deleted;
- histogram is explicitly distinguished from bar chart;
- descriptive scatterplots do not authorize causal inference;
- sample variance worked examples use denominator `n−1` and identify the result as sample variance;
- SD is kept in the original measurement unit while variance is in squared units;
- `SE(mean) ≈ SD/√n` is introduced only for the simple independent-observation setting;
- increasing n is taught to reduce sampling variability/SE under comparable SD, not to automatically reduce individual-level SD or systematic bias;
- sample distribution is explicitly the distribution of observed values; sampling distribution is the distribution of a statistic across hypothetical repeated samples;
- transformations are taught as scale changes rather than a method for erasing bias or forcing acceptable results;
- F0.4 `EXERCISES.md` created as a 100-point active-recall/application assessment;
- performance tasks require selecting/justifying summaries for four structurally different datasets, calculating descriptive summaries, detecting misleading graph choices and explaining what changes when n increases while underlying individual variability remains similar;
- local exercise gate is `>=80/100` plus no critical fail, applied only after observed performance;
- F0.4 `ANSWER_KEY.md` contains both the diagnostic scoring key and the commented unit answer key;
- diagnostic answers are therefore kept outside `ENTRY_DIAGNOSTIC.md` so the first attempt can remain independent;
- F0.4 production QA recorded in `QA_REPORT.md` with CONTENT, EVIDENCE, PEDAGOGICAL and MASTERY gates passed;
- `F0-S12` NIST/SEMATECH and `F0-S14` ICH E9/E9(R1) were rechecked on 2026-09-09;
- `F0-S27` added: Altman & Bland, *Standard deviations and standard errors*, BMJ 2005, used specifically for the stable distinction between individual variability (SD) and sampling variability/precision (SE);
- `SOURCE_INDEX.md` updated on 2026-09-09 with the F0.4 source checks and `F0-S27`.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

**Production position:** `F0.4 APPROVED`.

F0.1, F0.2 and F0.3 each have an approved instructional unit and approved NotebookLM study package.

F0.4 now has:

- quantitative entry diagnostic;
- approved self-contained lesson;
- active-recall/application assessment;
- commented diagnostic/unit answer key;
- approved production QA.

The F0.4 NotebookLM study package is the next production artifact.

**Learning position:** `UNSEEN`.

No F0 module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`.

## F0.4 canonical production decisions

- learner validation of F0.4 requires the quantitative entry diagnostic or equivalent evidence of the bridge;
- the diagnostic is not a hidden statistics exam; it measures only prerequisite numeracy;
- `READY_FOR_F0.4` requires 14–16/16 with no zero domain;
- localized weakness routes to `P1_REPAIR` when at least six of eight domains show some competence;
- broad/structural weakness routes to conditional `P2-QB_REQUIRED` when score is <=9/16, three or more domains are zero, or fewer than six domains show any competence;
- no P1/P2-QB learner state can be assigned without observed responses;
- variable type, scale, distribution shape and question determine descriptive choice; a universal `always report mean ± SD` rule is rejected;
- median/IQR are robust options for strong skew/extreme values but are not taught as universally superior;
- quantile conventions can differ slightly in small samples, so exercises specify conventions when material;
- visualizations are analytical objects and must expose scale/distribution rather than merely decorate tables;
- axis truncation is not automatically forbidden, but magnitude must be interpreted from numeric scale rather than visual area alone;
- larger samples improve stability/precision of statistics but do not automatically narrow the underlying individual distribution;
- range may increase in larger samples because more extreme observations may be encountered;
- systematic bias from F0.3 remains conceptually distinct from sampling variation;
- full CI/p-value/effect-size content remains deferred to F0.5;
- formal power/Type I–II error/multiplicity remains deferred to F0.6.

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner;
- F0.2 has not yet been studied or assessed by the learner;
- F0.3 has not yet been studied or assessed by the learner;
- F0.4 has not yet been studied or assessed by the learner;
- F0.4 quantitative diagnostic = `UNOBSERVED`;
- approved F0.1 NotebookLM sequence: `notebooklm/F0.1-scientific-questions/STUDY_GUIDE.md`;
- approved F0.2 NotebookLM sequence: `notebooklm/F0.2-study-designs/STUDY_GUIDE.md`;
- approved F0.3 NotebookLM sequence: `notebooklm/F0.3-bias-confounding-causal-validity/STUDY_GUIDE.md`;
- no mastery-state change is authorized from curriculum/package production alone.

## Operational constraints

- repository is public;
- never persist sensitive personal/health data;
- do not publish copyrighted PDFs without redistribution permission;
- current scientific/methodological claims must be researched and sourced;
- NotebookLM is a study layer; GitHub remains canonical;
- living/versioned sources must be rechecked when materially relevant;
- causal DAGs remain assumption maps, not proof;
- answer keys must not contaminate first-pass retrieval/application assessments;
- production can proceed in parallel with pending learner validation, but learner progression must respect prerequisite dependencies and the F0.4 quantitative diagnostic;
- exercise/nutrition-flavored numerical examples remain synthetic educational examples and must not become substantive nutrition recommendations.

## NEXT_ACTION

`F0-A09` — Produce the complete NotebookLM study package for `F0.4 — Descriptive statistics, distributions and sampling variation`. Create `notebooklm/F0.4-descriptive-statistics/MANIFEST.md`, `STUDY_GUIDE.md` and package `QA_REPORT.md` using the approved F0.4 lesson and a deliberately limited, auditable source corpus. Assign `CORE`/`SUPPORT`/`CONTRAST` roles and explain the instructional function and limitation of every source. The package must repeatedly require the learner to classify variable type; inspect distribution shape; choose and justify center + dispersion; detect outliers without automatic deletion; choose/audit visualizations; distinguish population/sample and parameter/statistic; distinguish sample distribution from sampling distribution; explain SD versus SE; and predict what changes when sample size increases while underlying individual variability remains similar. Preserve `SE(mean) ≈ SD/√n` at the simple conceptual/application level and keep confidence intervals/p-values/effect sizes deferred to F0.5 and formal power/multiplicity deferred to F0.6. Keep `ENTRY_DIAGNOSTIC.md`, `EXERCISES.md` and `ANSWER_KEY.md` outside the initial NotebookLM corpus so both diagnostic and independent assessment remain uncontaminated; the diagnostic must remain `UNOBSERVED` until the learner actually responds. Recheck all external links/version status used in the manifest, apply STUDY PACKAGE QA and copyright/public-repository controls, preserve F0.1–F0.4 learner states as pending, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.