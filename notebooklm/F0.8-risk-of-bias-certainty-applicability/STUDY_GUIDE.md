# F0.8 — NotebookLM Study Guide

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Use with:** the six-source corpus defined in `MANIFEST.md`

This guide is designed for active learning. Do not read the sources passively from beginning to end and then assume mastery. For each pass:

1. answer from memory first;
2. use NotebookLM to interrogate only the approved sources;
3. repair errors in your own words;
4. repeat the concept without consulting the sources;
5. only then advance.

The fixed audit sequence for this module is:

`1. Target question/outcome → 2. Reporting visibility → 3. Design/effect of interest → 4. Result-level RoB mechanisms → 5. RoB judgment/rationale → 6. Body estimate + threshold → 7. Inconsistency → 8. Indirectness → 9. Imprecision → 10. Missing/dissemination evidence → 11. Overall certainty → 12. Applicability to target → 13. Recommendation-strength boundary`

Do not substitute a global word such as “quality” for these thirteen fields.

---

## Pass 1 — Separate the six objects

Before asking NotebookLM anything, define from memory:

- reporting completeness;
- critical appraisal;
- result-level risk of bias;
- certainty of evidence;
- applicability/transportability;
- recommendation strength.

Then ask NotebookLM to compare your definitions against the canonical lesson and GRADE/STROBE sources.

### Required distinction

You must be able to say:

- reporting asks whether the process is visible;
- RoB asks whether a specific result may be systematically distorted;
- certainty asks how confident we are in the body/outcome effect range relative to decision thresholds;
- applicability asks whether that inference transfers to the target;
- recommendation strength is a broader decision output.

### Critical trap

`well reported = low risk = high certainty = applicable = strong recommendation`

This chain is invalid.

### Recall check

Without sources, give one example where:

1. reporting is excellent but RoB is high;
2. RoB is low but applicability is narrow;
3. certainty is high but the effect is trivial;
4. one outcome has high certainty but a strong recommendation still cannot be inferred.

---

## Pass 2 — Reporting versus methodological validity

Use the STROBE contrast source plus the canonical lesson.

Ask:

- What does STROBE say its checklist is for?
- What does it explicitly say the checklist is **not** for?
- Why can missing reporting create uncertainty without proving a method was poor?

### Repair exercise

Repair each statement:

- “The paper is STROBE-complete, so confounding is controlled.”
- “Allocation concealment was not reported, so concealment was definitely inadequate.”
- “PRISMA-complete means the review is high certainty.”

The repaired answer must separate **visibility** from **validity**.

---

## Pass 3 — Risk of bias is result-specific

Use the canonical lesson and riskofbias.info.

Construct one randomized trial with:

- automated performance outcome;
- subjective recovery outcome;
- different missingness patterns;
- several eligible analysis choices for only one outcome.

Then ask NotebookLM to help you produce separate RoB judgments for the two results.

### Required principle

A study is not a single indivisible object with “quality 8/10”.

Use:

`result/effect of interest → bias mechanism → domain → direction/impact plausibility → judgment + rationale`

### Critical trap

Do not average domains numerically.

---

## Pass 4 — RoB 2 architecture

Before consulting sources, state:

- current individually randomized parallel-group RoB 2 version;
- five core domains;
- usual judgment categories.

Then verify against riskofbias.info.

### Current version to retain

`22 August 2019`

### Five domains

1. bias arising from the randomization process;
2. bias due to deviations from intended interventions;
3. bias due to missing outcome data;
4. bias in measurement of the outcome;
5. bias in selection of the reported result.

### Applied drill

Use this synthetic result:

- 180 athletes randomized X vs control;
- adequate randomization/concealment;
- automated 12-week performance outcome;
- 22% missing in X vs 6% control;
- losses in X occur mainly after symptoms/worse training tolerance;
- completers-only primary analysis;
- registered outcome/timepoint matches report.

Answer:

1. What did randomization protect?
2. Which domain remains most concerning?
3. Why does “randomized” not settle the overall result-level judgment?
4. What additional information would change your confidence?

---

## Pass 5 — Bias versus imprecision

Use F0.5 reasoning from the canonical lesson.

Create two results:

- Result A: very narrow CI but strong measurement bias;
- Result B: wide CI but little evidence of systematic bias.

Explain why:

- Result A may be precise but wrong;
- Result B may be unbiased in expectation but too uncertain to support a narrow conclusion.

### Required sentence

> Precision and validity are different axes.

### Critical trap

Never use larger `n`, smaller p-value or narrower CI as proof that systematic bias is absent.

---

## Pass 6 — ROBINS-I and target-trial logic

Before any V2-specific discussion, state:

> `ROBINS-I V2 revised draft posted 20 November 2025; still draft and subject to change.`

Verify this wording using riskofbias.info.

Then construct the target trial for a non-randomized intervention study:

- eligibility;
- strategies/interventions;
- time zero;
- assignment benchmark;
- follow-up;
- outcome;
- causal contrast/effect of interest;
- analysis concept.

### Mechanism drill

Given self-selection into Intervention X, identify:

- likely confounders;
- selection processes;
- exposure/classification issues;
- missing-data pathways;
- measurement issues;
- result-selection opportunities.

### Critical traps

Reject both:

- `observational = useless`;
- `large adjusted observational study = randomized enough`.

Target-trial specification clarifies the benchmark; it does not create exchangeability or missing variables.

---

## Pass 7 — Design label is not a final verdict

Generate four cases:

1. low-risk randomized result;
2. high-risk randomized result;
3. weak non-randomized result;
4. unusually strong non-randomized result with rich confounding measurement and target-trial alignment.

For each, state:

- what the design gives you;
- what bias threats remain;
- what precision tells you;
- what applicability tells you.

### Required conclusion

`design → informs appraisal`

not

`design label → final certainty/applicability verdict`.

---

## Pass 8 — What GRADE certainty is

Use GRADE overview and certainty-principles sources.

From memory, state the four categories:

- High;
- Moderate;
- Low;
- Very low.

Then define certainty without using “paper quality”.

### Required idea

Certainty concerns confidence that the true effect lies within a decision-relevant range or on the relevant side of a threshold for an **outcome/body/question**.

### Repair exercise

Repair:

- “High certainty means the intervention works a lot.”
- “Low certainty means no effect.”
- “p<0.001 means high certainty.”
- “This RCT is high-certainty evidence.”

The last statement is incomplete because certainty is not simply a label for one paper.

---

## Pass 9 — Starting points are not final judgments

Ask NotebookLM to explain the two GRADE approaches to non-randomized intervention evidence.

You must understand:

- standard/basic framing: RCT body starts High; NRSI body usually starts Low;
- structured ROBINS-I framing: NRSI may start High and then be explicitly rated down for confounding/selection/other concerns.

### Required nuance

Do not memorize:

`RCT = high certainty forever`

or

`NRSI = low certainty forever`.

Starting level is only the beginning of the certainty assessment.

---

## Pass 10 — Body-level risk-of-bias domain

Return to a body of several studies.

Ask:

- Which results contribute most to the estimate?
- Which are at higher risk of bias?
- Do higher- and lower-risk results fall in different decision-relevant ranges?
- Would removing the most concerning results move the interpretation across the threshold?

### Required principle

There is no automatic rule:

`one high-risk study = downgrade one level`.

The question is whether the bias concern creates reasonable doubt about the effect range that matters.

---

## Pass 11 — Inconsistency preserves F0.7

Use the F0.7 concepts already embedded in the lesson.

Generate two meta-analytic bodies:

### Case A

- high I²;
- effects vary numerically but all remain above the same practical-benefit threshold.

### Case B

- low/moderate I²;
- effects cluster near a threshold so small between-study differences change the decision category.

Ask which case raises more decision-relevant inconsistency concern and why.

### Required rule

`I² alone ≠ inconsistency judgment`.

Use:

- direction;
- magnitude;
- decision ranges;
- clinical/methodological diversity;
- plausible effect modifiers;
- prespecified explanations;
- residual unexplained variability.

---

## Pass 12 — Indirectness and applicability

Use GRADE indirectness.

For every target, compare:

1. population;
2. intervention/exposure;
3. comparator;
4. outcome;
5. time horizon;
6. setting;
7. decision context.

### Mechanism rule

Do not downgrade or reject applicability just because a difference exists.

Ask:

> Is there a plausible reason this difference would materially change the relative effect, the absolute effect, or the decision-relevant interpretation?

### Drill

Target:

- trained adult endurance athletes;
- 12-week intervention;
- standardized performance score.

Evidence:

- mostly untrained participants;
- 2-week exposure;
- surrogate physiological marker.

Explain separately how population, time and outcome indirectness could matter.

### Critical distinction

`direct evidence ≠ unbiased evidence`.

---

## Pass 13 — Imprecision preserves F0.5

Use the practical-benefit threshold `+1.0`.

Compare:

- `MD +1.5 [1.2, 1.8]`;
- `MD +1.6 [-0.2, 3.4]`.

Do not discuss p-values first.

For each interval, ask:

- Is meaningful benefit compatible?
- Is trivial effect compatible?
- Is harm/negative effect compatible?
- Does the interval cross decision-relevant categories?

### Required conclusion

Imprecision is threshold/range dependent.

A statistically significant result can still be too imprecise for the decision, and a nonsignificant result can sometimes be informative if the CI rules out important effects.

---

## Pass 14 — Dissemination/non-reporting bias preserves F0.7

Review:

- selective non-publication;
- selective outcome/result reporting;
- small-study effects;
- funnel-plot limitations.

Generate one asymmetric and one symmetric funnel scenario.

For each, list at least three alternative explanations.

### Critical traps

Reject:

- `asymmetry = publication bias proven`;
- `symmetry = no publication bias`.

Use wording such as:

> missing/dissemination bias remains plausible/unresolved because...

not

> the funnel plot diagnosed publication bias.

---

## Pass 15 — Certainty is not effect magnitude

Generate four combinations:

1. high certainty, trivial effect;
2. high certainty, meaningful effect;
3. low certainty, apparently large point estimate;
4. very low certainty, near-null point estimate.

For each, separately state:

- best estimate;
- uncertainty/range;
- certainty;
- practical meaning.

### Required rule

`effect estimate` and `confidence in that estimate` are different objects.

---

## Pass 16 — Internal validity versus applicability

Create a 2×2 conceptual grid:

| | High applicability | Low applicability |
|---|---|---|
| Lower RoB | ? | ? |
| Higher RoB | ? | ? |

Fill each cell with a synthetic example.

### Required conclusions

- representative/direct target population does not repair internal bias;
- low-bias result can remain narrow for a different target;
- applicability is not a consolation prize for weak validity;
- validity does not guarantee transport.

---

## Pass 17 — Certainty versus recommendation strength

Use GRADE overview.

Suppose one outcome has high certainty of moderate benefit.

Before making a recommendation, list what is still missing:

- harms/undesirable outcomes;
- net effect across critical outcomes;
- values/preferences;
- resource use/costs when relevant;
- equity;
- acceptability;
- feasibility;
- target implementation context.

### Required rule

`certainty of one outcome ≠ recommendation strength`.

A strong recommendation is a broader decision judgment, not a direct mathematical transformation of one certainty rating.

---

# Pass 18 — Integrated two-body audit

## Target question

> In trained adult endurance athletes, does Intervention X versus control improve a standardized performance score after about 12 weeks? Higher is better. Practical-benefit threshold = `+1.0` point.

Everything below is synthetic.

## Evidence Body A

Four randomized parallel trials:

- predominantly trained adults;
- intervention/dose/duration close to target;
- adequate randomization/concealment;
- automated/blinded primary performance assessment;
- low differential missingness;
- primary analyses consistent with registrations;
- pooled `MD +1.5 [1.2, 1.8]`;
- study effects `+1.2`, `+1.4`, `+1.6`, `+1.7`;
- no material unexplained heterogeneity.

## Evidence Body B

Five non-randomized cohort studies:

- mostly recreational/untrained adults;
- Intervention X self-selected;
- higher baseline motivation/training volume strongly predicts X use;
- training volume measured crudely;
- completers-only analysis after differential dropout;
- subjective performance proxy in three studies;
- pooled transformed MD-equivalent `+1.6 [-0.2, 3.4]`;
- study effects range `-0.3` to `+3.8`;
- larger estimates concentrated in short-duration studies;
- no prespecified moderator analysis;
- most follow-up is 2–4 weeks rather than 12 weeks.

## Required 13-field audit

Complete in order, with no skipped field:

### 1. Target question/outcome

State the population, contrast, outcome, time horizon and `+1.0` practical-benefit threshold.

### 2. Reporting visibility

State what is visible for each body and what reporting information remains unknown. Do not infer methods from silence.

### 3. Design/effect of interest

State randomized versus non-randomized architecture and the causal effect/contrast being approximated.

### 4. Result-level RoB mechanisms

For Body A, identify residual possible mechanisms despite randomization.

For Body B, prioritize confounding, selection/missingness, measurement and result-selection mechanisms.

### 5. RoB judgment/rationale

Give a calibrated relative judgment. Do not use a total numerical quality score.

### 6. Body estimate + threshold

Compare both point estimates and CIs against `+1.0`.

### 7. Inconsistency

Use study-effect pattern and context, not I² alone.

### 8. Indirectness

Compare evidence and target population, intervention, comparator, outcome, time and setting/context.

### 9. Imprecision

State which decision ranges remain compatible with each CI.

### 10. Missing/dissemination evidence

State what is known versus unresolved. Do not invent funnel-plot evidence.

### 11. Overall certainty

Give a relative or categorical certainty judgment with explicit reasons. Exact category credit requires enough supplied information; otherwise state the uncertainty rather than inventing a rating.

### 12. Applicability to target

Judge Body A and Body B separately for trained endurance athletes at about 12 weeks.

### 13. Recommendation-strength boundary

State why these certainty/applicability judgments do not by themselves establish a strong/conditional recommendation.

---

## Expected high-level synthesis

A defensible answer should recognize that the point estimates are superficially similar but the evidence bodies are not epistemically equivalent.

Body A is more compatible with a confident meaningful-benefit interpretation because:

- result-level bias concerns appear smaller from the supplied information;
- effects are consistent in magnitude;
- the CI stays above the +1.0 threshold;
- target population/intervention/time/outcome are comparatively direct.

Body B is materially less secure because:

- self-selection plus crudely measured training/motivation creates confounding concerns;
- completers-only differential dropout raises selection/missingness concerns;
- subjective proxy outcomes create measurement/directness concerns;
- effects range from negative to large positive;
- the pooled CI spans below zero through large benefit;
- the target differs in training status and follow-up duration;
- no prespecified moderator analysis resolves the pattern.

Do **not** convert this high-level synthesis into a recommendation about a real intervention; the scenario is methodological and synthetic.

---

# Final closed-book check

Without NotebookLM or notes, answer all of the following in one sitting:

1. What six objects does F0.8 keep separate?
2. Why is a reporting checklist not a RoB tool?
3. Why is RoB result-specific?
4. What is the current RoB 2 version for individually randomized parallel-group trials?
5. Name the five RoB 2 domains.
6. Why can a randomized result still be high risk?
7. What is the current status of ROBINS-I V2?
8. What does target-trial thinking add to non-randomized appraisal?
9. Why is observational evidence not automatically unusable?
10. What are the four GRADE certainty categories?
11. What five domains can reduce certainty in F0.8?
12. Why does high certainty not imply a large effect?
13. Why does low certainty not imply no effect?
14. Why does statistical significance not determine certainty?
15. How does F0.5 enter imprecision?
16. How does F0.7 enter inconsistency?
17. How does F0.7 enter dissemination/missing-evidence reasoning?
18. How do you audit indirectness/applicability?
19. Why is internal validity different from applicability?
20. Why is certainty of one outcome different from recommendation strength?
21. Compare Bodies A and B without using the words “better study design” as a complete explanation.
22. Execute all thirteen F0.8 fields from memory.

If you cannot answer these without retrieval, continue study; do not mark mastery.

---

# What not to add to the first-pass notebook

Do not add:

- `EXERCISES.md`;
- `ANSWER_KEY.md`;
- production `QA_REPORT.md`;
- F0.4 `ENTRY_DIAGNOSTIC.md`;
- full `SOURCE_INDEX.md`;
- F0.9 full-paper materials;
- extra reporting checklists that only duplicate the reporting-versus-validity lesson;
- substantive sports-nutrition intervention papers.

The purpose is to train the methodological architecture, not to maximize source count.
