# F0.9 — Production QA Report

**Action:** `F0-A18`

**Module:** `F0.9 — Critical reading of a complete paper`

**QA date:** `2026-09-10`

**Files reviewed:**

- `LESSON.md`
- `EXERCISES.md`
- `ANSWER_KEY.md`
- `foundations/F0-scientific-literacy/SOURCE_INDEX.md` source plan/readback required before checkpoint close

**Production decision:** `PASS`, conditional only on final source-index/readback bookkeeping before checkpoint advancement.

---

# 1. Scope QA — PASS

The unit implements the exact F0.9 target from `COURSE_MAP.md`:

- complete-paper rather than abstract-only reading;
- article/supplement/registry/protocol/SAP navigation;
- compact PICO/estimand extraction before interpretation;
- result-table extraction before narrative;
- fixed twelve-step appraisal sequence;
- explicit integration of F0.1–F0.8;
- blind full-paper performance task;
- strongest-defensible-inference and what-is-not-established outputs.

The unit does not pull F0.10 calibrated public communication forward beyond the minimum concluding appraisal statement.

---

# 2. Prerequisite integration QA — PASS

F0.9 is intentionally integrative and learner validation requires F0.1–F0.8.

The lesson maps prior competencies explicitly:

- F0.1 → question, construct, outcome, time, estimand;
- F0.2 → design architecture, allocation/observation, sampling and inference limits;
- F0.3 → causal bias mechanisms, confounding, selection, measurement and missingness;
- F0.4 → descriptive data, sampling variability and SD/SE separation;
- F0.5 → direction, magnitude, effect measure, CI/precision and practical threshold;
- F0.6 → prospective power, multiplicity, registry/protocol/SAP and analytical flexibility;
- F0.7 → single-paper versus evidence-body distinction and synthesis context;
- F0.8 → result-specific RoB, certainty/body distinction and applicability.

No prior module is treated as a vocabulary checklist.

---

# 3. External source/currentness recheck — PASS

Only living/current methodological sources materially used in F0.9 were rechecked.

## `F0-S01` — CONSORT 2025

Rechecked 2026-09-10 at the BMJ current statement/explanation resources.

Verified:

- CONSORT 2025 remains the current general CONSORT statement;
- the statement was published in 2025 and uses a 30-item checklist;
- current explanation/elaboration emphasizes transparent reporting of design, conduct and analysis and access/timing of registration/protocol/SAP/open-science materials;
- its pedagogical role in F0.9 remains **reporting visibility/navigation**, not a validity score.

No source-version change requires lesson revision.

## `F0-S07` — RoB 2

Rechecked 2026-09-10 at `riskofbias.info`.

Verified:

- the current individually randomized parallel-group RoB 2 version remains `22 August 2019`;
- the official site continues to frame it as a risk-of-bias tool for randomized trials;
- the site states RoB 2/ROBINS-I/ROBINS-E/ROB ME materials are licensed CC BY-NC-ND 4.0.

F0.9 does not copy the protected operational tool documents into the repository. It uses only project-authored domain-level reasoning and links.

## `F0-S18` — GRADE Book overview

Rechecked 2026-09-10.

Verified:

- living chapter remains last modified `12 May 2026`;
- certainty applies to a body of evidence/key question rather than being a prestige score for an individual study;
- GRADE explicitly separates certainty of evidence from recommendation strength.

F0.9 uses this source only to preserve the boundary `single-paper appraisal ≠ body-level certainty rating`.

## `F0-S19` — GRADE intervention-certainty principles

Rechecked 2026-09-10.

Verified:

- living chapter remains last modified `21 August 2025`;
- certainty is tied to ranges/decision thresholds and applies across a body of evidence for an outcome;
- it is not a single-paper quality score.

No source-version change requires lesson revision.

---

# 4. Performance-paper eligibility and legal-access QA — PASS

Selected assessment paper:

**Klemp AO, Ormsbee MJ, Yeh M, et al. Neither pre-sleep nor post-exercise protein consumption influences resistance exercise training adaptations in older adults. Journal of the International Society of Sports Nutrition. 2025;22(1):2519511. doi:10.1080/15502783.2025.2519511.**

Why it satisfies `ASSESSMENT_BLUEPRINT.md`:

- human participants;
- directly exercise/nutrition relevant;
- chronic 12-week intervention rather than only an acute mechanistic experiment;
- randomized parallel-group architecture;
- full text legally accessible;
- quantitative outcomes with reported 95% CIs for key time contrasts;
- enough methods/statistical detail for genuine appraisal;
- registry identifier available;
- public data repository named;
- multiple outcomes/timepoints and a post-study sensitivity-power calculation provide real multiplicity/precision questions;
- nontrivial but not absurd appraisal issues exist.

## Copyright/access status

The PMC copy states that the article is Open Access under **CC BY 4.0**.

No article full text, figure, table or third-party PDF has been copied into the GitHub repository. The repository contains only citation, legal links and original educational synthesis/questions.

---

# 5. Performance-paper factual readback — PASS

The paper/record were checked against the following facts used in the answer key.

## Population/design

- randomized 12-week trial in older men, approximately ages 60–75;
- 32 enrolled/randomized and 30 completed/analyzed;
- three groups: post-exercise protein (`PRP`), pre-sleep protein (`PSP`) and resistance-training-only (`RETO`);
- supervised full-body resistance training two times per week.

## Intervention/comparator

- PRP and PSP receive the same 40 g mixed protein product under different timing schedules;
- the product contains energy and other macronutrients in addition to protein;
- RETO receives no supplemental protein and is reported as not blinded to group assignment;
- therefore PRP-vs-PSP is more directly a timing contrast, while supplemented-vs-RETO is not a pure nutrient-timing contrast.

## Analysis

The paper reports:

- linear mixed-effects models using REML;
- fixed factors time and group;
- participant random intercept;
- Kenward–Roger df/p-values;
- p<0.05 threshold;
- Sidak-adjusted pairwise comparisons/CIs for significant effects;
- a post-study `sensitivity power analysis` using N=30 and observed-model residual variability.

F0.9 correctly prevents that sensitivity-power analysis from being used as posterior evidence or as a substitute for the observed treatment-effect uncertainty.

## Results

The paper reports increases over time in muscle-thickness and strength outcomes, including 95% CIs for several week-0-to-week-12 changes, while reporting no statistically significant group-related differences.

The answer key explicitly distinguishes these time effects from a between-group treatment effect and does **not** invent an unreported treatment-effect CI.

## Registration/prespecification

- paper identifies `NCT05922475` and explicitly says the trial was retrospectively registered;
- public trial-record data place study start in September 2017 and completion in May 2019;
- registry first submission/posting occurred in 2023, after study completion;
- therefore the registry improves retrospective transparency but cannot prove prospective outcome/analysis prespecification for the completed trial;
- the paper also states that the presented data are a subset of a larger project with additional outcomes.

The educational material treats this as a selection/prespecification **uncertainty/opportunity**, not proof that selective reporting occurred.

---

# 6. CONTENT_QA — PASS

Checked:

- the 12-step sequence matches the canonical F0.9 architecture;
- `within-group change ≠ between-group effect` is explicit;
- `nonsignificant ≠ equivalence` is explicit;
- observed/post hoc power is not used for completed-study inference;
- reporting completeness is separated from validity;
- missing reporting is not converted into demonstrated misconduct/method failure;
- result-specific bias reasoning is preserved;
- single-paper appraisal is separated from GRADE body certainty;
- applicability is separated from internal validity;
- terminology is defined at point of use;
- synthetic examples do not present nutrition recommendations.

No material internal contradiction found.

---

# 7. EVIDENCE_QA — PASS

Evidence-source fit:

- CONSORT 2025 → reporting/navigation only;
- riskofbias.info/RoB 2 → result-specific bias architecture;
- GRADE Book → body-level certainty boundary only;
- Klemp et al. → real performance appraisal object;
- ClinicalTrials.gov `NCT05922475` → external timeline/outcome-record comparison.

Anti-cherry-picking protections:

- the answer key identifies both strengths and limitations;
- absence of group differences is not dismissed simply because the paper has limitations;
- retrospective registration is not treated as automatic invalidity;
- low attrition is acknowledged rather than exaggerated;
- high adherence/supervision are acknowledged;
- the paper's narrow population/context is separated from its internal estimate.

No claim depends on journal prestige, citation count or author reputation.

---

# 8. PEDAGOGICAL_QA — PASS

The unit follows:

`article map → extraction → prior-module audit → quantitative result → prespecification/robustness → applicability → conclusion audit`.

Pedagogical safeguards:

- P0 article anatomy is taught locally;
- P1 PICO/estimand and result tables are modeled locally;
- learner is instructed to mark unavailable information `UNCLEAR / NOT REPORTED`;
- performance paper appraisal is not solved in `LESSON.md`;
- answer key remains a separate file;
- real paper is accompanied by a neutral context box rather than substantive nutrition coaching;
- assessment routes errors back to F0.1–F0.8 dependencies.

---

# 9. MASTERY_QA — PASS

Assessment total = 100 points.

Sections test:

- article anatomy/extraction;
- temporal prespecification reasoning;
- result-specific bias;
- within-versus-between group inference;
- CI/equivalence reasoning;
- observed-power misuse;
- multiplicity/exploration;
- a complete blind appraisal of a real full paper.

The real-paper task requires:

- provenance;
- PICO/estimand extraction;
- design/sampling;
- intervention/comparator fidelity;
- outcomes;
- bias/missingness;
- model/sample-size/prespecification;
- result estimates/uncertainty;
- multiplicity/robustness;
- applicability;
- strongest defensible inference;
- audit of authors' conclusion;
- explicit what-is-not-proven boundaries.

A checklist-only response is capped at 60/100.

Local pass gate remains:

`>=80/100 + no critical fail`.

This gate changes no learner state until actual performance is observed.

---

# 10. Critical-fail coverage — PASS

The assessment explicitly blocks:

- abstract-only appraisal;
- design-label-only appraisal;
- reporting checklist as validity score;
- `p<0.05 = true/important`;
- `p>0.05 = no effect/equivalence`;
- observed-power rescue;
- ignoring retrospective/prospective prespecification;
- ignoring material multiplicity;
- reporting completeness = low RoB;
- one paper-level RoB/certainty score replacing result-specific reasoning;
- within-group significance as treatment effect;
- unsupported acute/mechanistic → chronic performance/body-composition extrapolation;
- repeating authors' conclusion without reconstruction;
- inventing missing methodological information;
- assigning one paper a body-of-evidence GRADE rating.

---

# 11. Public-repository/privacy QA — PASS

- no personal user data persisted;
- no private health data persisted;
- no credentials/secrets persisted;
- no third-party full text copied;
- paper URLs/DOI/registry/data links are references only;
- exercise/nutrition scenarios are educational/synthetic except the explicitly cited published appraisal paper;
- no individual nutrition prescription/recommendation is created.

---

# 12. Production versus learning-state QA — PASS

F0-A18 is curriculum production only.

Therefore:

- F0.1–F0.8 learner states remain pending/unvalidated;
- F0.9 learner state remains `UNSEEN` until actual study/performance occurs;
- no module is marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from this production activity;
- F0.4 quantitative diagnostic remains `UNOBSERVED`.

---

# 13. Final production decision

`PASS — APPROVE F0.9 UNIT` once the source-index additions `F0-S30`/`F0-S31` and final file/readback checks are persisted.

After that bookkeeping, the canonical next production action should be the F0.9 NotebookLM study package, not F0.10 yet.
