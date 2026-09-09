# F0.8 — Exercícios e avaliação independente

**Unit:** `F0.8 — Risk of bias, certainty of evidence and applicability`

**Assessment state:** independent; do not consult `ANSWER_KEY.md` before first attempt.

**Total:** `100 points`

**Local gate:** `>=80/100 + no critical fail`.

Passing this assessment does not by itself authorize `MASTERED`; learner-state changes require observed scoring and the project mastery protocol.

---

# Critical-fail gate

Any response that endorses one of the following as a final principle fails the local gate even if the numeric score is >=80:

1. `CONSORT/STROBE/PRISMA complete = low risk of bias/high quality`;
2. a single summed quality score replaces domain-based RoB reasoning;
3. `randomized = automatically low risk of bias`;
4. `observational = automatically unusable/high risk`;
5. `low certainty = no effect`;
6. `high certainty = large/important effect`;
7. `statistical significance = high certainty`;
8. `direct evidence = unbiased evidence`;
9. representative sampling is used as a repair for internal bias;
10. GRADE certainty is treated as a score for one paper;
11. certainty of one outcome is treated as identical to recommendation strength;
12. ROBINS-I V2 Nov 2025 is described as finalized/stable rather than draft.

---

# Section A — Conceptual separation — 25 points

## A1. Five objects — 5 points

For each prompt, name the primary object being judged:

`reporting completeness`, `critical appraisal`, `risk of bias`, `certainty of evidence`, `applicability`, or `recommendation strength`.

1. “Were the search strategy and exclusions fully described?”
2. “Could missing outcomes systematically shift this result?”
3. “How confident are we that the true effect is above a +1.0 threshold for this outcome?”
4. “Do results from recreational adults transport to elite endurance athletes?”
5. “Should a guideline make a strong or conditional recommendation?”

## A2. Repair the reporting fallacy — 4 points

Repair both statements:

1. “This RCT followed CONSORT completely, so it is low risk of bias.”
2. “This review followed PRISMA, so the evidence is high certainty.”

Your repairs must state what the reporting guideline **does** establish and what still requires separate appraisal.

## A3. Bias versus imprecision — 4 points

Study A: `MD +1.6 [1.4, 1.8]`, but outcome measurement is systematically influenced by unblinded assessors.

Study B: `MD +1.6 [-1.0, 4.2]`, outcome measurement is objective and no major systematic-bias mechanism is supplied.

Explain separately:

- which study is more precise;
- which supplied problem is bias versus random uncertainty;
- why precision cannot repair the problem in Study A.

## A4. Result-specific RoB — 4 points

One trial measures:

- automated time-trial performance;
- self-reported perceived recovery collected by unblinded staff;
- blood biomarker analyzed by blinded laboratory staff.

Explain why “the study has one risk-of-bias rating” is inadequate.

## A5. Certainty versus magnitude — 4 points

Classify the following claims as valid/invalid and repair invalid claims:

1. High-certainty evidence must show a large effect.
2. A narrow CI around a trivial effect can support high certainty about triviality.
3. Low-certainty evidence means the true effect is zero.
4. A large point estimate can coexist with low certainty.

## A6. Certainty versus recommendation — 4 points

In <=120 words, explain why high certainty for one performance outcome does not automatically imply a strong recommendation for an intervention.

---

# Section B — RoB 2 and ROBINS-I applied reasoning — 25 points

## B1. RoB 2 domains — 5 points

From memory, list the five main RoB 2 domains for individually randomized parallel-group trials.

No credit for replacing domains with a numerical quality score.

## B2. RCT audit — 10 points

Synthetic randomized trial:

- 180 athletes randomized X versus control;
- computerized random sequence and adequate concealment;
- primary outcome is automated time-trial at week 12;
- missing primary outcome: 22% in X versus 6% in control;
- most missing data in X followed symptoms and poor training tolerance;
- final analysis includes completers only;
- registration predates enrollment and identifies the same primary outcome/timepoint;
- no evidence supplied of multiple alternative primary analyses.

For each RoB 2 domain, state:

1. the main information relevant to the domain;
2. your qualitative concern (`low concern`, `some/material concern`, or `high/material concern` is sufficient; exact official tool completion is not required);
3. a one-sentence rationale.

Then write an overall bounded interpretation of the **primary result**, without calling the whole trial “good” or “bad”.

## B3. Why randomization is not enough — 3 points

Give three post-randomization mechanisms that can create risk of bias despite correct baseline randomization.

## B4. ROBINS-I target-trial logic — 4 points

Explain the target-trial benchmark for a non-randomized intervention study and why it does **not** make observational data randomized.

## B5. Version literacy — 3 points

State the current project position for ROBINS-I V2 as rechecked on 2026-09-09:

- date/version status;
- whether finalized;
- one important structural feature/change in the current draft.

---

# Section C — GRADE certainty and applicability — 25 points

## C1. Four certainty categories — 4 points

List the four GRADE certainty categories and explain in one sentence what certainty is confidence **about**.

## C2. Five downgrading domains — 5 points

List the five core GRADE domains that can lower certainty for an intervention-effect evidence body.

## C3. Threshold-aware imprecision — 5 points

Practical benefit threshold = `+1.0`.

Body A: `MD +1.5 [1.2, 1.8]`.

Body B: `MD +1.5 [-0.4, 3.4]`.

Compare their imprecision without using a significance label as the conclusion. State which decision-relevant ranges each CI includes.

## C4. Inconsistency without I² worship — 4 points

Body C has `I² = 10%`, but all studies were conducted in one narrow laboratory population that differs greatly from the target.

Body D has `I² = 70%`, but all estimates remain on the same side of a prespecified practical-benefit threshold and the variation has a plausible prespecified explanation.

Explain why:

- low I² does not guarantee high certainty;
- high I² does not automatically invalidate synthesis or force a downgrade without contextual reasoning.

## C5. Indirectness/applicability matrix — 5 points

Target:

> trained adult endurance athletes; Intervention X at protocol dose; active control; field performance outcome; 12-week horizon; hot outdoor environment.

Evidence:

> recreational adults; half target dose; placebo; laboratory physiological surrogate; 2-week horizon; temperate indoor setting.

For each dimension below, state the mismatch and one plausible reason it might or might not materially affect transfer:

- population;
- intervention;
- comparator;
- outcome;
- time horizon;
- setting.

## C6. Directness versus bias — 2 points

Repair:

> “The study population exactly matches the target, therefore the result is unbiased.”

---

# Section D — Integrated evidence-body audit — 25 points

Target decision:

> In trained adult endurance athletes, Intervention X versus control improves synthetic performance score after approximately 12 weeks. Higher = better. Practical-benefit threshold = `+1.0` point.

Everything below is synthetic and methodological only.

## Evidence Body A

Four randomized parallel trials:

- predominantly trained adults;
- intervention/dose/duration close to target;
- automated/blinded primary performance assessment;
- adequate randomization/concealment;
- low and balanced missingness;
- primary analyses match preregistration;
- pooled `MD +1.5 [1.2, 1.8]`;
- study effects `+1.2`, `+1.4`, `+1.6`, `+1.7`;
- no material unexplained heterogeneity supplied;
- search included trial registries and attempts to locate unpublished results.

## Evidence Body B

Five non-randomized cohort studies:

- mostly recreational/untrained adults;
- Intervention X self-selected;
- baseline motivation/training volume predicts both X use and outcome;
- training volume measured crudely;
- completers-only analyses after differential dropout;
- subjective performance proxy in three studies;
- pooled transformed `MD-equivalent +1.6 [-0.2, 3.4]`;
- individual effects range `-0.3` to `+3.8`;
- larger effects occur mainly in 2–4 week studies;
- no prespecified moderator analysis;
- target application is trained athletes at ~12 weeks.

Complete all **13 fields** below in order:

1. Target question/outcome.
2. Reporting visibility — what is known and what remains unknown from the summaries.
3. Design/effect of interest.
4. Result-level RoB mechanisms for each body.
5. Comparative RoB judgment with rationale.
6. Body estimate + practical threshold interpretation.
7. Inconsistency.
8. Indirectness.
9. Imprecision.
10. Missing/dissemination-evidence concerns.
11. Relative overall certainty judgment for A versus B and why.
12. Applicability to the target.
13. Recommendation-strength boundary — state why this assessment alone cannot determine a final strong/conditional recommendation.

### Required performance-task constraints

Your answer must explicitly state all of the following:

- similar point estimates do not imply similar certainty;
- Body B's observational design does not by itself make the evidence unusable;
- Body A's randomized design does not exempt it from RoB appraisal;
- the CI in B leaves materially different decision ranges compatible with the evidence;
- certainty and applicability receive separate judgments;
- certainty of the performance outcome is not recommendation strength.

---

# Scoring summary

| Section | Points |
|---|---:|
| A — Conceptual separation | 25 |
| B — RoB 2 / ROBINS-I | 25 |
| C — GRADE / applicability | 25 |
| D — Integrated audit | 25 |
| **Total** | **100** |

A technically fluent answer that commits a critical fail does not pass the local gate.
