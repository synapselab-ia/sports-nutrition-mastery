# F0.8 — Production QA Report

**Module:** `F0.8 — Risk of bias, certainty of evidence and applicability`

**Reviewed:** `2026-09-09`

**Decision:** `APPROVED`

**Learner-state change:** none.

**F0.4 quantitative diagnostic:** unchanged; remains `UNOBSERVED`.

This QA covers the instructional unit only. It does not indicate that the learner studied or mastered F0.8.

---

# 1. Required artifact gate — PASS

Canonical unit path:

`foundations/F0-scientific-literacy/F0.8-risk-of-bias-certainty-applicability/`

Required files created:

- `LESSON.md`;
- `EXERCISES.md`;
- `ANSWER_KEY.md`;
- `QA_REPORT.md`.

Assessment total: `100 points`.

Local assessment gate: `>=80/100 + no critical fail`, applicable only after actual observed learner performance.

---

# 2. Scope/prerequisite gate — PASS

F0.8 uses the required P2 dependencies:

- F0.2 — study design/inference boundaries;
- F0.3 — causal bias mechanisms/internal versus external validity;
- F0.5 — magnitude, CI, practical thresholds;
- F0.7 — heterogeneity, synthesis and missing-evidence reasoning.

The lesson does not treat formal RoB/certainty/applicability as if they were already mastered from production activity.

P0/P1 support is taught locally:

- result-specific RoB;
- domain-based judgment;
- certainty categories;
- evidence-versus-target PICO comparison;
- threshold/range reasoning;
- applicability dimensions.

---

# 3. External source/version verification — PASS

Verification date: `2026-09-09`.

Only already-registered sources were used; no new source ID was required in `SOURCE_INDEX.md`.

## `F0-S07` — riskofbias.info / RoB 2 / ROBINS-I

Rechecked official riskofbias.info pages.

Verified:

- current RoB 2 version for individually randomized parallel-group trials remains `22 August 2019`;
- RoB 2 remains result-specific and domain-based;
- current ROBINS-I V2 revised draft is posted `20 November 2025`;
- the official page explicitly states that ROBINS-I V2 remains a **draft subject to change**;
- current Nov-2025 V2 draft lists six main domains:
  1. confounding;
  2. classification of intervention;
  3. selection into the study;
  4. missing data;
  5. measurement of outcome;
  6. selection of reported result;
- current V2 also includes triage for `Critical risk of bias`;
- the Nov-2025 draft removed the separate deviations-from-intended-intervention domain present in the Nov-2024 draft.

Use is restricted to conceptual/applied domain reasoning; official tool completion/training is not simulated by a simple score.

## `F0-S05` — Cochrane Handbook

Current Handbook landing page remains Version 6.5 (2024).

Chapter 8 was rechecked and continues to state that:

- RoB 2 is the recommended randomized-trial risk-of-bias tool for Cochrane Reviews;
- assessment targets a specific result;
- five bias domains are used;
- signalling questions feed domain judgments;
- judgments require written justification.

No protected chapter PDF was copied into the repository.

## `F0-S18` — GRADE overview

Current official GRADE Book chapter rechecked:

- last modified `12 May 2026`;
- four certainty categories remain `high`, `moderate`, `low`, `very low`;
- five principal domains can lower certainty: risk of bias, inconsistency, indirectness, imprecision and dissemination/publication bias;
- certainty assessment and recommendation development remain distinct processes.

## `F0-S19` — GRADE certainty principles

Current official chapter rechecked:

- last modified `21 August 2025`;
- certainty is assessed across a body of evidence for an outcome/question;
- current framing is threshold/range aware;
- absolute-effect reasoning is emphasized for decision-relevant certainty;
- RCT bodies generally start high for intervention questions;
- NRSI can follow the traditional low-start approach or, for advanced users applying structured ROBINS-I assessment, may start high and then be rated down according to identified limitations.

The lesson presents this nuance and explicitly rejects `observational = unusable`.

## `F0-S20` — GRADE indirectness

Current official chapter rechecked:

- last modified `12 May 2026`;
- indirectness is assessed through PICO alignment and indirect comparisons;
- differences should matter when they plausibly produce meaningful systematic changes in relative or absolute effects;
- applicability/generalizability/transferability are not binary labels.

## Reporting contrast — `F0-S01`, `F0-S02`, `F0-S03`

Rechecked current reporting resources as needed for the conceptual contrast.

- STROBE explicitly states that its recommendations concern reporting and that its checklist is **not** an instrument for evaluating methodological quality.
- PRISMA 2020 remains the main PRISMA reporting guideline and exposes a 27-item checklist plus expanded/abstract checklists and flow diagrams.
- CONSORT remains used only as randomized-trial reporting transparency, not as risk-of-bias certification.

No source-version change required a new source ID.

---

# 4. CONTENT_QA — PASS

## Required distinction: reporting vs appraisal vs RoB vs certainty vs applicability

Explicitly taught and repeatedly tested.

The lesson prevents:

`reporting complete → low bias → high certainty → broadly applicable → strong recommendation`

as an invalid automatic chain.

## Result-specific risk of bias

Explicitly taught:

- a study can have different RoB judgments for different results;
- quality-total scoring is rejected;
- bias and imprecision are separated;
- overall reasoning is not a numerical average of domains.

## RoB 2

All five current main domains for individually randomized parallel-group trials are taught at conceptual/applied level.

Critical protection:

`randomized ≠ automatically low risk of bias`.

## ROBINS-I

Target-trial logic is taught as a causal benchmark rather than retroactive randomization.

Current Nov-2025 V2 draft status is explicit.

Critical protection:

`observational ≠ automatically unusable`.

## GRADE certainty

Four categories and five downgrading domains are taught.

Certainty is explicitly:

- outcome/question/body specific;
- threshold/range aware;
- not effect magnitude;
- not statistical significance;
- not a paper prestige label.

## Inconsistency

Preserves F0.7:

- I² is not certainty;
- decision-relevant effect pattern matters;
- plausible prespecified explanations matter;
- heterogeneity statistics alone do not determine certainty.

## Indirectness/applicability

Structured comparison covers:

- population;
- intervention/exposure;
- comparator;
- outcome;
- time horizon;
- setting;
- decision context.

The lesson distinguishes internal validity from transportability/applicability.

## Imprecision

Preserves F0.5 magnitude/CI/practical-threshold reasoning.

The worked contrast with equal point estimates but CIs `[1.2,1.8]` versus `[-0.4,3.4]` correctly demonstrates decision-relevant precision rather than p-value thresholding.

## Missing/dissemination evidence

Preserves F0.7:

- small-study/funnel signals are non-diagnostic;
- absence of a signal is not proof of complete evidence.

## Recommendation boundary

The lesson explicitly separates outcome certainty from recommendation strength and lists additional decision criteria without attempting a full guideline panel workflow.

---

# 5. EVIDENCE_QA — PASS

- Claims about RoB 2 are sourced to official riskofbias.info/Cochrane material.
- ROBINS-I V2 is labeled with its current **draft** status rather than silently treated as final.
- GRADE categories/domain/indirectness claims use current official GRADE Book material.
- The unit does not cherry-pick a single design hierarchy as universal truth.
- Reporting guidelines are used only for their reporting function.
- Effect magnitude and precision remain separate from certainty.
- Synthetic exercise/nutrition scenarios do not become substantive recommendations.
- No third-party full text was copied into GitHub.

---

# 6. PEDAGOGICAL_QA — PASS

Progression:

`objects to separate → reporting contrast → result-specific bias → RoB 2 → ROBINS-I → body-level certainty → GRADE domains → applicability → recommendation boundary → integrated evidence-body audit`

This sequence prevents premature memorization of GRADE labels before the learner can distinguish the underlying objects.

Pedagogical safeguards include:

- counterexamples;
- explicit critical fails;
- two studies with same estimate but different precision;
- randomized trial with material missing-data bias;
- non-randomized evidence that must be appraised rather than dismissed;
- high-certainty trivial-effect example;
- direct-but-biased distinction;
- integrated target/evidence applicability matrix.

---

# 7. MASTERY_QA — PASS

The 100-point assessment covers:

- conceptual discrimination;
- misconception repair;
- result-specific RoB 2 application;
- target-trial/ROBINS-I reasoning;
- version literacy;
- GRADE categories/domains;
- threshold-aware imprecision;
- I²/inconsistency repair;
- structured applicability;
- integrated comparison of two evidence bodies.

The performance task requires all 13 fields:

`Target question/outcome → Reporting visibility → Design/effect of interest → Result-level RoB mechanisms → RoB judgment/rationale → Body estimate + threshold → Inconsistency → Indirectness → Imprecision → Missing/dissemination evidence → Overall certainty → Applicability → Recommendation-strength boundary`.

A learner cannot pass by terminology recall alone.

---

# 8. Critical-fail QA — PASS

The assessment explicitly fails these errors:

- reporting checklist completion = low RoB/high quality;
- total quality score replaces domain reasoning;
- randomized = automatically low RoB;
- observational = automatically high/unusable;
- low certainty = no effect;
- high certainty = large/important effect;
- significance = high certainty;
- direct evidence = unbiased evidence;
- representative sample repairs internal bias;
- certainty = paper score;
- certainty = recommendation strength;
- ROBINS-I V2 Nov 2025 mislabeled as finalized.

This meets and extends the F0-A16 critical-fail requirements without changing scope.

---

# 9. Integrated performance-task QA — PASS

Both synthetic bodies have similar point estimates:

- A: `+1.5 [1.2,1.8]`;
- B: `+1.6 [-0.2,3.4]`.

They differ materially in:

- randomization/confounding;
- missingness;
- measurement;
- consistency;
- precision;
- population directness;
- follow-up directness;
- reporting/prespecification visibility.

The learner must judge separately:

1. result-level RoB;
2. body certainty;
3. applicability;
4. recommendation boundary.

This directly tests the target competency.

---

# 10. Scope-boundary QA — PASS

Deferred beyond F0.8 depth:

- full signalling-question-by-question official tool certification;
- advanced ROB-ME implementation;
- exhaustive GRADE Evidence Profiles;
- guideline Evidence-to-Decision panel process;
- formal transportability estimators;
- network-meta-analysis certainty;
- recommendation authoring.

F0.9 remains the full-paper practicum that integrates F0.1–F0.8.

---

# 11. Copyright/public-repository QA — PASS

- no protected RoB/Handbook/GRADE PDF copied into GitHub;
- repository contains project-authored Markdown plus citations/links only;
- no personal, clinical or sensitive user data;
- all athlete/intervention examples are synthetic methodological examples.

---

# 12. Production/learning-state separation — PASS

After F0-A16 production:

- F0.1–F0.7 learner states remain pending/unvalidated;
- F0.8 learner state remains `UNSEEN`/unvalidated;
- F0.4 quantitative diagnostic remains `UNOBSERVED`;
- no `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` transition is authorized.

---

# 13. Final gate

> Can a learner with F0.2/F0.3/F0.5/F0.7 prerequisites distinguish reporting from bias, apply domain-level RoB reasoning to randomized/non-randomized results, compare certainty of two evidence bodies using GRADE-style domains, and separately judge applicability without collapsing any of those objects into recommendation strength?

**Decision:** yes.

**Production decision:** `APPROVED`.
