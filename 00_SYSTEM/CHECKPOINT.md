# CHECKPOINT — Sports Nutrition Mastery

**Updated:** 2026-09-08
**Canonical branch:** `main`
**Project state:** `F0_1_STUDY_PACKAGE_READY`

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
- external study links verified on 2026-09-08 for Cochrane Handbook v6.5 Chapter 2, EMA ICH E9/E9(R1), GRADE Book, CONSORT 2025 and Areta et al. full text via PMC.

## Current curriculum position

`F0 — Scientific Literacy and Quantitative Reasoning`

Production position: `F0.1 STUDY_PACKAGE_READY`; F0.2 is the next unproduced instructional unit.

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

## Pending learning validations

- F0.1 has not yet been studied or assessed by the learner.
- The approved NotebookLM study sequence is available in `notebooklm/F0.1-scientific-questions/STUDY_GUIDE.md`.
- No mastery-state change is authorized from curriculum/package production alone.

## Operational constraints

- repository is public;
- never persist sensitive personal/health data;
- do not publish copyrighted PDFs without redistribution permission;
- current scientific claims must be researched and sourced, not generated from memory alone;
- NotebookLM is a study layer; GitHub remains canonical;
- F0 source versions must be rechecked if a living methodological resource materially changes before its dependent lesson is authored;
- lesson exemplars must not be promoted into practical recommendations beyond the evidence they directly provide;
- answer keys must not contaminate first-pass retrieval/application assessments.

## NEXT_ACTION

`F0-A04` — Produce the complete second instructional unit `F0.2 — Study designs and what they can answer` using `COURSE_MAP.md`, `PREREQUISITE_GRAPH.md` and the mapped methodological sources. Create a self-contained `LESSON.md`, active-recall/application `EXERCISES.md`, commented `ANSWER_KEY.md` and production `QA_REPORT.md`. Explicitly teach randomized parallel, crossover, cluster and factorial trials; non-randomized intervention studies; cohort, case-control and cross-sectional designs; acute mechanistic versus chronic outcome studies; temporal ordering; within-subject versus between-subject comparisons; washout/carryover intuition; unit of allocation versus unit of analysis; and the introductory target-trial concept where useful. For every design, require the learner to state the strongest defensible inference and at least one tempting inference the design does not establish. Do **not** prematurely teach the full bias/confounding/causal-identification content reserved for F0.3. Research/recheck current authoritative design/reporting sources as required, add only new sources actually used to `SOURCE_INDEX.md`, apply CONTENT/EVIDENCE/PEDAGOGICAL/MASTERY QA, preserve F0.1 learning state as pending, then update this checkpoint and leave exactly one subsequent `NEXT_ACTION`.
