# F0 Exit Assessment v1 — Production QA Report

**Artifact:** `foundations/F0-scientific-literacy/F0-exit-assessment/`
**QA date:** `2026-09-11`
**Decision:** `PASS — READY_FOR_ADMINISTRATION`
**Learner state changed:** no
**F0.4 diagnostic changed:** no; remains `UNOBSERVED`

## 1. Scope gate — PASS

The packet implements the approved `ASSESSMENT_BLUEPRINT.md` without changing its architecture:

| Section | Required | Implemented |
|---|---:|---:|
| A — Question/design/causal structure | 20 | 20 |
| B — Quantitative interpretation | 25 | 25 |
| C — Systematic review/certainty | 20 | 20 |
| D — Full-paper critical appraisal | 25 | 25 |
| E — Communication of uncertainty | 10 | 10 |
| **Total** | **100** | **100** |

Exit gate is preserved exactly:

- `>=85/100` total;
- every section `>=70%`;
- no `CRITICAL_FAIL`;
- integrated full-paper appraisal;
- uncertainty communication that does not overstate the evidence.

The packet is authored only. No learner response exists and no score/state is inferred.

---

## 2. CONTENT_QA — PASS

### A — question/design/causal reasoning

- A1 requires target, intervention/exposure, comparator, outcome/time, estimand and a result that counts against the claim.
- A2 spans randomized crossover, prospective cohort and cross-sectional designs and requires inference boundaries rather than labels.
- A3 uses an explicit synthetic causal graph with confounder, mediator and collider structure. The answer key explains pathways rather than bias-name memorization.

### B — quantitative reasoning

- skewed-data item supports median/IQR reasoning;
- SD and SE remain separate objects;
- truncated-axis item tests visual magnitude distortion;
- risk change correctly distinguishes `+5 percentage points` from `+50% relative`;
- B2 uses `MD=-18 s [−38,+2]`, benefit threshold `−25 s`, harm threshold `+25 s`; the CI is deliberately compatible with important benefit, trivial/near-null effects and slight worsening, but not the prespecified important-harm threshold;
- B4 correctly makes Study B more informative because `[-18,+2]` excludes the `−25 s` important-benefit threshold while Study A `[-55,+19]` does not;
- p-value and post-hoc-power items preserve F0.5/F0.6 definitions;
- multiplicity item distinguishes analytical opportunity family from one highlighted p-value.

### C — evidence synthesis/certainty

- synthetic forest package contains five studies, all on the same MD-seconds scale, with weights summing to 100%;
- pooled random-effects result and `I²=74%` are explicitly supplied as synthetic outputs rather than recomputed from hidden assumptions;
- the task tests weight/precision versus quality, pooled estimate versus heterogeneity and clinical/methodological explanations;
- review-method extract contains both demonstrated strengths/limitations and one deliberately unresolved protocol-comparison issue;
- certainty comparison uses nearly identical point estimates with sharply different RoB, precision, consistency and directness so the learner cannot equate point estimate with evidence strength.

### D — complete paper

The assigned paper is different from F0-S30 and satisfies the blueprint:

- human exercise/nutrition trial;
- randomized, double-blind, placebo-controlled, parallel design;
- trained endurance population;
- legally accessible full text;
- quantitative estimates with 95% CIs;
- multiple outcomes and explicit multiplicity adjustment;
- nontrivial sample-size/prespecification/missingness/applicability issues;
- public trial-registry companion;
- enough information to reconstruct question → design → bias → estimate → uncertainty → applicability → conclusion.

### E — communication

- one fixed synthetic result is used for technical and plain-language outputs;
- estimate, CI, practical threshold, moderate certainty, applicability and non-equivalence boundary are all explicit;
- scoring rewards invariant epistemic content rather than tone/style.

No scored item requires hidden sports-nutrition factual knowledge beyond the information supplied or the assigned full paper/registry.

---

## 3. EVIDENCE_QA — PASS

### Assigned paper verification

**F0-S32** — Jagłowska K, Folwarski M, Chroboczek M, Potrykus M, Kaczmarczyk M, Skonieczna-Żydecka K, Kaczor JJ. *Multistrain Probiotic Supplementation Combined with a Standardized Diet Did Not Significantly Affect Exercise Performance or Inflammatory Responses in Male Endurance Runners: A Randomized Controlled Trial.* Nutrients. 2026;18(15):2484. doi:10.3390/nu18152484.

Verified on 2026-09-11:

- publication date: 1 August 2026;
- PMC full text resolves at `https://pmc.ncbi.nlm.nih.gov/articles/PMC13468382/`;
- article is Open Access under CC BY;
- 30 trained male long-distance runners randomized and 27 completed/analyzed;
- four-week multistrain probiotic vs matched placebo with standardized diet;
- primary performance outcome VO2peak;
- primary estimand reported as group×phase interaction;
- VO2peak interaction approximately `−3.5 mL·kg−1·min−1 [−7.0,−0.1]`, nominal `p=.044`, adjusted `p=.707` after Benjamini–Hochberg correction;
- paper explicitly frames trial as exploratory/preliminary and reports per-protocol/complete-case analysis;
- a-priori target was 40 participants based on a large assumed effect from a different prior athletic/formulation context; target was not reached;
- paper states the public trial registration was retrospective: first submitted 31 Dec 2025 and first posted 13 Feb 2026 after participant enrolment;
- article also states primary/secondary outcomes and sample-size calculation existed in earlier bioethics/grant materials; these claims are kept distinct from what the public registry independently proves;
- article contains internally inconsistent wording in its institutional statement calling the registration prospective/prior to enrollment. The answer key resolves this by the reported timeline rather than by choosing the more favorable label;
- paper explicitly limits generalization to women and notes self-reported training monitoring, modest sample and no direct microbiome/metabolomic measurement in this reported analysis.

### Trial registry verification

**F0-S33** — ClinicalTrials.gov `NCT07411482`.

Verified public URL: `https://clinicaltrials.gov/study/NCT07411482`.

The registry is used as a provenance/timeline audit source. It is not treated as a validity certificate or as automatic evidence of prospective prespecification.

### Anti-cherry-picking / inferential balance

The paper was selected for assessment fitness, not because it supports a desired probiotic conclusion. The answer key explicitly prevents both positive and null overclaiming:

- nominal `p=.044` is not converted into confirmed harm;
- adjusted `p=.707` is not converted into proof of no effect;
- the CI, achieved information, multiplicity and practical-threshold absence remain visible;
- mechanistic claims are bounded because direct microbiome/metabolomic measurements are not part of the reported analysis.

No substantive recommendation about probiotic use is produced by the assessment.

---

## 4. PEDAGOGICAL_QA — PASS

The assessment is cumulative rather than definition-heavy:

- Section A integrates F0.1–F0.3;
- Section B integrates F0.4–F0.6;
- Section C integrates F0.7–F0.8 with F0.5/F0.6 safeguards;
- Section D requires F0.1–F0.9 in one real paper;
- Section E tests F0.10 while preserving F0.5/F0.8.

Fresh transfer is protected:

- A–C/E use new synthetic scenarios/numbers, not module assessment copies;
- D uses a different full paper from F0-S30;
- the answer key accepts calibrated alternatives but not structural misconceptions;
- missing information must be labeled rather than invented;
- checklist-only Section D is capped at 60% as required by the blueprint.

The assessment therefore tests reasoning transfer rather than answer memorization.

---

## 5. MASTERY_QA — PASS

The packet can distinguish memorized vocabulary from integrated performance because it requires:

- operationalization;
- design/inference boundaries;
- causal-path reasoning;
- quantitative interval/threshold interpretation;
- multiplicity/prespecification reasoning;
- forest-plot/heterogeneity interpretation;
- body-level certainty/applicability reasoning;
- full-paper independent reconstruction;
- calibrated cross-audience communication.

Critical fails remain conceptual safety gates, not arbitrary point deductions.

A passing first administration may support `APPLIED`/`INTEGRATED` evidence according to `MASTERY_PROTOCOL.md`; this production QA does not authorize any learner-state change and does not authorize `MASTERED` from one attempt.

---

## 6. Answer-key QA — PASS

The key includes:

- point-by-point allocation for all 100 points;
- acceptable alternative reasoning where relevant;
- explicit critical-fail triggers;
- earliest-dependency remediation mapping;
- D-section source facts sufficient for consistent scoring;
- separate rules for PASS, NEAR_PASS, BROADER_REMEDIATION and CRITICAL_FAIL;
- section minimums A 14/20, B 17.5/25, C 14/20, D 17.5/25, E 7/10.

No answer requires invented external information.

---

## 7. Public-repository / copyright QA — PASS

- no third-party PDF/full article/table/figure was copied into GitHub;
- the assessment stores citation, DOI, public links and original appraisal questions only;
- F0-S32 is CC BY, but full-text duplication is unnecessary and deliberately avoided;
- ClinicalTrials.gov is linked as a public record;
- synthetic data in Sections A–C/E are project-authored;
- no private health/personally identifying learner data are stored.

---

## 8. Production decision

`PASS — READY_FOR_ADMINISTRATION`

F0 Exit Assessment v1 is suitable for a first independent administration under the canonical gate.

This decision means the **assessment artifact** is ready. It does **not** mean the learner passed, studied or attempted F0.

Learner position remains pending/UNSEEN across F0.1–F0.10, and the F0.4 quantitative diagnostic remains `UNOBSERVED` until actual learner activity is observed.
