# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-08
**Canonical branch:** `main`
**Project state:** `F0_2_INSTRUCTIONAL_UNIT_APPROVED`

## Completed

- public repository initialized;
- canonical agent/startup protocol created;
- project mission and scope defined;
- public-repository/privacy policy defined;
- evidence policy and research protocol defined;
- pedagogical standard and QA gates defined;
- mastery protocol defined;
- NotebookLM protocol and manifest template created;
- macro curriculum created;
- source registry and claim ledger initialized;
- learner, mastery, error and study-history artifacts initialized;
- F0 Scientific Literacy scaffold created;
- `F0-A01` completed: evidence-backed instructional architecture for F0.1–F0.10 created;
- F0 competency/course map created in `foundations/F0-scientific-literacy/COURSE_MAP.md`;
- P0/P1/P2 dependency graph and conditional quantitative bridge created in `PREREQUISITE_GRAPH.md`;
- authoritative methodological source index created in `SOURCE_INDEX.md`, researched/checked on 2026-09-08;
- F0 exit-assessment architecture, scoring gates, critical-fail conditions and retest rules created in `ASSESSMENT_BLUEPRINT.md`;
- `F0-A02` completed: full instructional unit `F0.1 — Scientific questions, hypotheses and operationalization` created and QA-approved;
- F0.1 self-contained lesson created in `foundations/F0-scientific-literacy/F0.1-scientific-questions/LESSON.md`;
- F0.1 active-recall/application assessment created in `EXERCISES.md`;
- F0.1 commented answer key and local progression rubric created in `ANSWER_KEY.md`;
- F0.1 production QA recorded in `QA_REPORT.md` with CONTENT, EVIDENCE, PEDAGOGICAL and MASTERY gates passed;
- sports-nutrition transfer exemplar `F0-S21` (Areta et al. 2013) registered in the local `SOURCE_INDEX.md` and explicitly restricted to inferential-boundary/operationalization teaching;
- `F0-A03` completed: NotebookLM study package for F0.1 created and Study Package QA passed;
- F0.1 NotebookLM manifest v1 created in `notebooklm/F0.1-scientific-questions/MANIFEST.md` with a six-source auditable corpus and `CORE`/`SUPPORT`/`CONTRAST` roles;
- practical NotebookLM setup/study sequence created in `notebooklm/F0.1-scientific-questions/STUDY_GUIDE.md`;
- package source/file/link verification and copyright/answer-leakage controls recorded in `notebooklm/F0.1-scientific-questions/QA_REPORT.md`;
- external study links verified on 2026-09-08 for Cochrane Handbook v6.5 Chapter 2, EMA ICH E9/E9(R1), GRADE Book, CONSORT 2025 and Areta et al. full text via PMC;
- `F0-A04` completed: full instructional unit `F0.2 — Study designs and what they can answer` created and QA-approved;
- F0.2 self-contained lesson created in `foundations/F0-scientific-literacy/F0.2-study-designs/LESSON.md`;
- F0.2 active-recall/application assessment created in `EXERCISES.md`, including eight study-classification scenarios and mandatory strongest-defensible/tempting-invalid inference statements;
- F0.2 commented answer key and local progression rubric created in `ANSWER_KEY.md`;
- F0.2 production QA recorded in `QA_REPORT.md` with CONTENT, EVIDENCE, PEDAGOGICAL and MASTERY gates passed;
- F0.2 design-specific methodological sources `F0-S22`–`F0-S25` registered in `SOURCE_INDEX.md`: Cochrane Chapter 23 plus crossover, cluster-randomized and factorial CONSORT extensions;
- target-trial source `F0-S17` expanded to F0.2 use after 2026-09-08 recheck;
- source-version caveat recorded: CONSORT 2025 is the current general standard; older design-specific extensions are used only for their still-relevant architecture until updated replacements exist.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

Production position: `F0.2 APPROVED`; F0.1 remains `STUDY_PACKAGE_READY`; F0.2 NotebookLM packaging is the next production step.

Learning position: `UNSEEN`

No module has been marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`. Production approval and NotebookLM package readiness must not be interpreted as learner mastery.

## F0 architecture decisions now canonical

- F0.1–F0.10 are organized by conceptual dependency rather than simple terminology sequence;
- reporting guidelines (CONSORT/STROBE/PRISMA) must not be taught or scored as study-quality/risk-of-bias instruments;
- a quantitative entry diagnostic precedes F0.4; isolated numeracy gaps are P1 repairs, structural gaps become conditional `P2-QB` before inferential statistics;
- F0 exit requires integrated appraisal of a complete exercise/nutrition paper plus quantitative and evidence-synthesis interpretation;
- passing the first exit assessment can support `APPLIED/INTEGRATED`, but does not automatically establish `MASTERED`; later cumulative retesting is required;
- current methodological backbone includes CONSORT 2025, Cochrane Handbook v6.5 (2024), current risk-of-bias resources, ASA statistical-inference statements, causal-inference references and the living GRADE Book current through 2026;
- exercise/nutrition primary studies used for transfer must be labeled as exemplars and must not be treated as general methodological authorities.

## F0.1 canonical production decisions

- F0.1 teaches `question → target population → contrast → outcome → time → estimand` before study-design choice;
- PICO(T) is taught as a decomposition aid, not as a mechanical quality checklist;
- construct, operational definition, variable, outcome/endpoint and estimand are explicitly separated;
- exploratory analysis is treated as legitimate hypothesis generation when transparently labeled; post hoc findings must not be rewritten as prespecified confirmation;
- primary, secondary and exploratory outcomes are distinguished without prematurely teaching full multiplicity mathematics;
- the estimand framework is introduced conceptually using population, conditions compared, variable/outcome, intercurrent-event handling and population-level summary, while estimator/statistical-design detail is deferred;
- acute mechanistic outcomes are explicitly prevented from being silently converted into chronic hypertrophy, performance or health conclusions;
- the local F0.1 exercise gate is `>=80/100` with critical-fail conditions, but it affects learning state only after actual observed learner performance.

## F0.1 NotebookLM package decisions

- initial corpus is intentionally limited to six sources: canonical F0.1 lesson, Cochrane Chapter 2, ICH E9/E9(R1), GRADE Book answerable-question material, CONSORT 2025 and Areta et al. 2013;
- `ANSWER_KEY.md` is excluded from the initial NotebookLM corpus to prevent answer leakage;
- `EXERCISES.md` remains outside the initial corpus and is completed independently after source-guided study;
- CONSORT remains `SUPPORT` reporting guidance, never a risk-of-bias score;
- Areta et al. is `CONTRAST`/transfer evidence for inferential-boundary practice, not a universal nutrition recommendation;
- the GRADE Book is a living JavaScript resource; if NotebookLM ingestion fails, the official page remains a manual reference rather than being replaced with an unofficial copy;
- package generation changed no learner state.

## F0.2 canonical production decisions

- F0.2 teaches study design as architecture relative to a scientific question, not as a universal evidence pyramid;
- every major design requires two outputs: the strongest defensible inference and at least one tempting inference not established by the design;
- randomization is taught as an allocation mechanism that strengthens causal comparability in expectation, not as a guarantee of perfect baseline balance, flawless execution or universal generalizability;
- parallel randomized trials are separated from crossover by between-subject versus within-subject comparison structure;
- crossover suitability requires a sufficiently stable setting, reversible/transient effects and explicit washout/carryover/period-effect reasoning;
- cluster trials distinguish unit of allocation from unit of observation/analysis; individual observations inside one randomized cluster must not be treated as independent randomizations;
- factorial trials introduce multiple randomized factors and interaction intuition without prematurely teaching interaction-testing/multiplicity mathematics;
- non-randomized intervention studies are neither treated as automatically causal nor dismissed as intrinsically useless; formal confounding/identification is deferred to F0.3;
- retrospective cohort versus case-control is distinguished by where sampling starts, not by whether historical data are used;
- cross-sectional designs are limited to prevalence/association unless temporal/causal information comes from additional structure;
- acute mechanistic studies and chronic adaptation/outcome studies are explicitly separated;
- diagnostic, prognostic and intervention questions are treated as distinct design problems rather than forced into an RCT hierarchy;
- target-trial emulation is introduced as a way to specify the hypothetical randomized causal design before using observational data; it does not create randomization or repair inadequate data;
- the local F0.2 exercise gate is `>=80/100` with critical-fail conditions, but it affects learning state only after actual observed learner performance.

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner.
- F0.2 has not yet been studied or assessed by the learner.
- The approved F0.1 NotebookLM study sequence remains available in `notebooklm/F0.1-scientific-questions/STUDY_GUIDE.md`.
- F0.2 has an approved instructional unit but no NotebookLM study package yet.
- No mastery-state change is authorized from curriculum/package production alone.

## Operational constraints

- repository is public;
- never persist sensitive personal/health data;
- do not publish copyrighted PDFs without redistribution permission;
- current scientific claims must be researched and sourced, not generated from memory alone;
- NotebookLM is a study layer; GitHub remains canonical;
- F0 source versions must be rechecked if a living methodological resource materially changes before its dependent lesson is authored;
- legacy CONSORT design extensions must be clearly distinguished from the current general CONSORT 2025 statement;
- lesson exemplars must not be promoted into practical recommendations beyond the evidence they directly provide;
- answer keys must not contaminate first-pass retrieval/application assessments.

## NEXT_ACTION

`F0-A05` — Create the complete NotebookLM study package for `F0.2 — Study designs and what they can answer`. Build `notebooklm/F0.2-study-designs/MANIFEST.md`, `STUDY_GUIDE.md` and package `QA_REPORT.md`. Use the canonical F0.2 lesson as `CORE`; select a deliberately small auditable corpus from the sources actually used in F0.2, prioritizing current/general CONSORT 2025 plus the most instructionally necessary cluster/crossover/factorial/Cochrane/target-trial resources rather than loading every registered methodology source. Assign explicit `CORE`/`SUPPORT`/`CONTRAST` roles and explain exactly what each source should teach. Exclude `ANSWER_KEY.md` and keep `EXERCISES.md` outside the initial NotebookLM corpus to prevent answer leakage. The study sequence must force classification of unfamiliar study descriptions, between- versus within-subject reasoning, washout/carryover, unit-of-allocation logic, cohort/case-control/cross-sectional discrimination, acute-versus-chronic inferential boundaries and target-trial limits; it must repeatedly require “strongest defensible inference” plus “tempting unsupported inference.” Verify every source/file/link and current version, preserve F0.1/F0.2 learning state as pending, run Study Package QA, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.
