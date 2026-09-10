# F0.10 — Production QA Report

**Action:** `F0-A20`

**Module:** `F0.10 — Synthesis and communication of uncertainty`

**QA date:** `2026-09-10`

**Files reviewed:**

- `LESSON.md`
- `EXERCISES.md`
- `ANSWER_KEY.md`
- `foundations/F0-scientific-literacy/SOURCE_INDEX.md`

**Production decision:** `PASS — APPROVED`, subject only to final GitHub readback/checkpoint bookkeeping.

---

# 1. Scope QA — PASS

The unit implements the exact F0.10 target from `COURSE_MAP.md`:

- calibrated evidence language;
- point estimate + interval + practical/decision threshold kept together;
- `did not detect` separated from `no meaningful effect` and formal equivalence;
- conflicting evidence synthesized by inferential weight rather than source counting;
- directness separated from bias;
- uncertainty sources separated into bias, imprecision, inconsistency, indirectness and missing/dissemination evidence;
- body certainty separated from recommendation strength;
- explicit applicability/target scope;
- explicit conclusion-changing evidence/assumption conditions;
- one fixed evidence package translated into technical, practitioner-facing and lay-facing outputs;
- explicit language-drift audit.

No later-domain nutrition prescription or guideline-development curriculum is pulled forward.

---

# 2. Prerequisite integration QA — PASS

F0.10 learner validation requires F0.5 + F0.7 + F0.8 + F0.9.

The lesson preserves these dependencies:

- F0.5 → `Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`;
- F0.7 → heterogeneous/conflicting evidence is interpreted by compatibility, design, weighting, heterogeneity and missing-evidence context, not paper vote counting;
- F0.8 → RoB, body certainty, directness/applicability and recommendation strength remain separate objects;
- F0.9 → communication starts from a reconstructed appraisal/estimand rather than title/abstract framing.

The unit does not redefine these prerequisites inconsistently.

---

# 3. Current external-source recheck — PASS

Only external methodological sources actually used were rechecked on `2026-09-10`.

## `F0-S08` — ASA Statement on p-values

Official ASA resource remains accessible.

Verified for F0.10:

- the 2016 statement still presents six principles for proper p-value use;
- scientific conclusions should not be based only on whether a p-value crosses a threshold;
- p-values do not measure effect size or practical importance;
- reporting/interpretation requires broader scientific/statistical reasoning.

F0.10 uses this only to block binary truth/absence language from p-values.

## `F0-S09` — ASA President's Task Force statement

Official ASA/Amstat News page remains accessible and continues to emphasize:

- uncertainty and variability;
- multiplicity and replicability;
- selective reporting as a distortion risk;
- p-values/significance tests as potentially useful when properly interpreted rather than universal truth metrics;
- practical significance as distinct from statistical significance.

No version/status change requires curriculum revision.

## `F0-S18` — GRADE Book overview

Rechecked living official page.

Verified:

- last modified `12 May 2026`;
- certainty remains categorized `High / Moderate / Low / Very low`;
- certainty applies to bodies of evidence/key questions rather than individual-study prestige labels;
- certainty is framed relative to ranges/decision thresholds;
- certainty of evidence remains explicitly separate from strength of recommendation.

## `F0-S19` — GRADE intervention-certainty principles

Rechecked living official page.

Verified:

- last modified `21 August 2025`;
- certainty remains tied to whether the true effect lies in a target range or on a side of a decision threshold;
- point estimate remains the best available estimate while certainty describes confidence around the target range;
- domain overlap/double counting remains a caution;
- standardized communication formats are intended to improve transparent communication, not erase uncertainty.

## `F0-S20` — GRADE indirectness

Rechecked living official page.

Verified:

- last modified `12 May 2026`;
- indirectness remains a certainty domain concerning applicability/generalizability/transferability;
- PICO mismatch remains the core structured comparison;
- setting/time issues can enter through PICO components;
- directness does not imply absence of study-level bias.

No new source ID was necessary: all sources actually used were already registered in `SOURCE_INDEX.md`, whose repository-level `Last researched` date is already `2026-09-10`.

---

# 4. CONTENT_QA — PASS

Checked:

- `invariant core` is consistently defined as target, direction, magnitude, precision, threshold, certainty, applicability and inferential boundaries/update conditions;
- technical/practitioner/lay translation changes wording but not epistemic content;
- point estimates are never allowed to travel without relevant uncertainty/threshold context when material;
- `p<0.05` is not treated as true/important;
- `p>0.05` is not treated as no effect/equivalence;
- formal equivalence is distinguished from a nonsignificant superiority test;
- high certainty is separated from large effect;
- low certainty is separated from no effect;
- uncertainty mechanisms are named rather than collapsed into generic “uncertainty”;
- directness and internal validity are distinct;
- evidence statements and recommendation statements are distinct;
- update conditions are concrete rather than generic “more research needed” language.

Synthetic numerical examples were checked for direction/threshold consistency.

---

# 5. EVIDENCE_QA — PASS

Source-to-claim fit:

- `F0-S08` → p-value interpretation boundary;
- `F0-S09` → uncertainty/multiplicity/replicability/context and significance-language boundary;
- `F0-S18` → certainty categories, body-level certainty and recommendation separation;
- `F0-S19` → range/threshold-oriented certainty reasoning;
- `F0-S20` → indirectness/applicability structure;
- approved F0.5/F0.7/F0.8/F0.9 units → internal canonical integration.

No external sports-nutrition efficacy claim is taught in F0.10. The fixed performance package uses intentionally fictional `Intervention X`, preventing accidental conversion into a real recommendation.

Anti-false-balance safeguards require weighting by claim fit, design/bias, magnitude/precision, directness and synthesis context rather than counting papers.

---

# 6. Fixed performance-package quantitative QA — PASS

Target:

- trained adult endurance athletes;
- Intervention X daily for 8–12 weeks;
- 20-km time-trial seconds, lower better;
- important-benefit threshold = `-30 s`.

Direct evidence supplied:

- meta-analysis: `MD -20 s [-42,+2]` → crosses both null and `-30 s` threshold;
- large low-risk RCT: `MD -12 s [-27,+3]` → excludes a >=30-s benefit under the supplied interval while permitting small benefit/no difference;
- small high-risk RCT: `MD -75 s [-140,-10]` → large point estimate but wide interval plus serious attrition/selective-analysis concerns.

Contextual evidence:

- observational cohort: larger favorable association but residual confounding plus population/outcome indirectness;
- acute mechanistic crossover: biomarker effect but no chronic performance outcome.

Supplied body-level certainty = `MODERATE`.

The expected synthesis therefore supports:

- small benefit remains plausible;
- large benefit is less well supported;
- the evidence does not justify “works”, “does not work” or formal equivalence language;
- no recommendation is justified because recommendation criteria were intentionally not evaluated.

No internal numerical contradiction found.

---

# 7. PEDAGOGICAL_QA — PASS

The progression is:

`reconstructed evidence → invariant core → calibrated claim → audience translation → drift audit → update conditions`.

Pedagogical safeguards:

- local P0 vocabulary is defined;
- P1 translation skill is taught through worked examples;
- the lesson includes positive and negative examples;
- conflict synthesis is taught without mechanical evidence-pyramid scoring;
- the same fixed evidence package is used for all audience outputs;
- a drift audit makes hidden certainty inflation observable;
- learner must explain what evidence would change the conclusion.

The unit is self-contained given its declared P2 prerequisites.

---

# 8. MASTERY_QA — PASS

Assessment total = `100 points`:

- Section A — calibrated language/claim scope: 20;
- Section B — estimate + interval + threshold: 20;
- Section C — conflict/false balance/uncertainty source: 20;
- Section D — fixed evidence package across audiences: 40.

The performance task requires three distinct audience outputs from one invariant evidence core.

Scoring explicitly tests:

- quantitative preservation;
- epistemic calibration;
- correct weighting of discordant sources;
- body certainty;
- applicability;
- recommendation boundary;
- drift detection and correction.

Local gate remains:

`>=80/100 + no critical fail`.

This gate changes no learner state until actual performance is observed.

---

# 9. Critical-fail coverage — PASS

The assessment explicitly blocks all F0-A20 critical fails:

- `p<0.05 = true/important`;
- `p>0.05 = no effect/equivalence`;
- hiding materially important CI/threshold information;
- low certainty → no effect;
- high certainty → large/important effect;
- direct evidence → unbiased;
- equal rhetorical weight solely for balance;
- body certainty → recommendation strength;
- unsupported target expansion;
- causal-language strengthening beyond design;
- practitioner/lay version more certain than technical version.

Additional safeguards block:

- acute biomarker → chronic performance proof;
- observational association → co-equal randomized causal estimate without qualification;
- paper vote counting;
- issuing advice from an evidence package that explicitly lacks recommendation assessment.

---

# 10. Public-repository/privacy QA — PASS

- no personal user data persisted;
- no private health data persisted;
- no credentials/secrets persisted;
- no third-party full text copied;
- all performance-package studies are synthetic;
- no individual nutrition prescription is created;
- only citations/links to methodological sources already registered in the public project are used.

---

# 11. Production versus learning-state QA — PASS

F0-A20 is curriculum production only.

Therefore:

- F0.1–F0.9 learner states remain pending/unvalidated;
- F0.10 learner state remains `UNSEEN` until actual study/performance;
- no F0 module is marked `STUDIED`, `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED` from production activity;
- F0.4 quantitative diagnostic remains `UNOBSERVED`.

---

# 12. Final production decision

`PASS — APPROVE F0.10 UNIT`.

After final file/readback bookkeeping, the next canonical production action should be the F0.10 NotebookLM study package. The cumulative F0 exit assessment remains subsequent to completion of the F0.10 study package; it must not be inferred complete from curriculum production.
