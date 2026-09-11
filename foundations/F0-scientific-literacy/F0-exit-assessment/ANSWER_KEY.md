# F0 Exit Assessment v1 — Answer Key and Scoring Guide

**Use:** scoring only after independent administration
**Total:** `100 points`
**Pass gate:** `>=85/100` total + every section `>=70%` + no `CRITICAL_FAIL`

This key rewards defensible reasoning. Equivalent wording earns credit when it preserves the same scientific content. Do not require one memorized phrase when multiple interpretations are genuinely defensible.

---

# Global critical-fail rules

A `CRITICAL_FAIL` blocks passage regardless of total score when the response materially demonstrates any of the following structural misconceptions:

1. observational association asserted causal solely because it is significant/adjusted;
2. `p>0.05 = no effect` when meaningful effects remain compatible with the data;
3. a frequentist 95% CI interpreted as a 95% posterior probability that the fixed true parameter lies in the observed interval;
4. statistical significance treated as practical importance;
5. CONSORT/STROBE/PRISMA completion treated as proof of low RoB/high quality;
6. low I² treated as proof of clinical/methodological identity;
7. obvious multiplicity ignored while a favorable result is declared confirmatory;
8. low/very-low certainty converted into a definitive recommendation without explicit independent justification;
9. absence of evidence confused with sufficiently precise evidence excluding a meaningful effect;
10. material information fabricated rather than marked missing/unclear.

Additional F0.9/F0.10 critical errors can trigger failure when severe: within-group change substituted for treatment effect, observed-power rescue, body-level certainty assigned from one paper, or a lay synthesis made materially more certain than the technical synthesis.

---

# Section A — 20 points

## A1 — 5 points

Full-credit answer defines a coherent target effect. One acceptable example:

> Among trained adult 10 km runners, does ingesting a specified dose/composition of CarboMax at a defined pre-race timing, versus an isoenergetic matched placebo/control, change official 10 km completion time over a standardized test/race? The target contrast is the mean between-strategy difference in completion time under the assigned strategies. A result with a sufficiently precise interval excluding any prespecified practically important benefit would count against the performance claim.

Scoring:

- 1.0 — target population;
- 1.0 — operational intervention/exposure;
- 0.75 — comparator;
- 0.75 — outcome + window;
- 0.75 — explicit contrast/estimand;
- 0.75 — plausible falsifying/counter-claim result.

Acceptable alternatives may use recreational runners, a different valid performance outcome, crossover estimand or another dose/timing, provided all components align.

**Remediation if weak:** F0.1.

## A2 — 7 points

### Study A — 2 points

- Design: randomized counterbalanced crossover trial with blinding and washout.
- Strongest inference: under valid randomization, adequate washout/no problematic carryover, adherence and measurement, it can estimate the acute within-person causal contrast between beverage X and placebo for the 20 km trial in the studied cyclists.
- Cannot establish by itself: long-term training adaptation, effects in different populations, or validity if carryover/unblinding/measurement problems are material.

### Study B — 2 points

- Design: prospective observational cohort.
- Strongest inference: prospective association between habitual caffeine exposure and subsequent injury incidence, conditional on measured data/model.
- Cannot establish causal effect solely from adjustment/significance; residual/unmeasured confounding and exposure measurement remain possible.

### Study C — 2 points

- Design: cross-sectional observational study.
- Strongest inference: contemporaneous association between reported protein intake and measured strength.
- Cannot establish temporal order or causal effect; reverse causation/confounding are plausible.

### Synthesis — 1 point

Randomization protects baseline exchangeability against confounding in principle when implemented correctly, but it does not automatically solve deviations, missingness, poor measurement, carryover, selective reporting, imprecision or external validity.

**CRITICAL_FAIL:** B or C declared causal only because adjusted/significant.

**Remediation:** F0.2; causal overreach → F0.3/F0.2.

## A3 — 8 points

Expected reasoning:

- `T` = confounder because `T→X` and `T→Y`, creating backdoor path `X←T→Y` (1.5).
- `G` = mediator on `X→G→Y`; adjusting for it blocks part of the total effect and changes the estimand toward a direct effect under further assumptions (1.5).
- `S` = collider on `X→S←U`; conditioning/stratifying on S can associate X with U and open `X↔U→Y`, generating collider/selection bias (2.0).
- adjusting for T is defensible to close the backdoor path (1.0).
- U need not be adjusted merely because it predicts Y; in the stated graph it does not cause X unless S is conditioned on (0.75).
- reasonable total-effect strategy: adjust for T, do not condition on G or S; state that this conclusion is conditional on the simplified DAG and adequate measurement/positivity/model specification (1.25).

Accept equivalent causal-path wording.

**Remediation:** F0.3; if target/estimand confusion is primary → F0.1.

---

# Section B — 25 points

## B1 — 5 points

### B1a — 1 point

Median/IQR is preferable as the primary summary because the value 46 creates strong right-skew/outlier influence. Mean/SD can be additionally reported if useful, but mean/SD alone may poorly describe the typical value/spread.

### B1b — 1 point

For the simple mean relation `SE≈SD/√n`, quadrupling n halves SE if SD is comparable. Individual-observation SD does not necessarily shrink.

### B1c — 1 point

Truncating the axis can visually exaggerate a small absolute difference. Report original-scale difference/estimate, uncertainty (CI/SE), units and a practical threshold/context before judging importance.

### B1d — 2 points

- absolute risk difference: `15%−10%=+5 percentage points` (1);
- relative increase: `(15−10)/10=50%` (1).

**Remediation:** F0.4; percentage confusion may require quantitative bridge.

## B2 — 8 points

Expected audit:

1. direction favors intervention because lower time is better (0.75);
2. point estimate = 18 s faster (0.75);
3. CI spans from 38 s faster to 2 s slower, so precision is insufficient for a narrow conclusion (1.25);
4. practically important benefit (`<=-25 s`) remains compatible because CI extends to −38 (1.25);
5. small/trivial effects including near-zero are compatible (1.0);
6. practically important harm `>=+25 s` is not compatible with this CI; only slight worsening up to +2 remains compatible (1.0);
7. crossing zero means the interval includes the null under this model/procedure; it does not prove no effect or tell practical importance by itself (1.0);
8. strongest conclusion: estimate favors benefit, but data remain compatible with practically important benefit and little/no difference; they exclude the prespecified large-harm threshold in the displayed interval (1.0).

**CRITICAL_FAIL:** `CI crosses zero, therefore no effect`, or statistical significance substituted for practical interpretation.

**Remediation:** F0.5 → F0.4 if interval/SE concepts broken.

## B3 — 4 points

Statement 1: false (2).
Repair: p=0.03 is a probability about data/test statistic extremeness under the specified null/model and assumptions; it is not `P(H0|data)` and does not state effect magnitude/importance.

Statement 2: false (2).
Repair: p=0.12 does not prove absence or practical irrelevance. Interpretation requires estimate, CI/compatible range, threshold, design/bias and context.

**CRITICAL_FAIL:** posterior probability reversal or p>0.05=no effect.

**Remediation:** F0.5.

## B4 — 4 points

Study B is more informative for the `-25 s` benefit threshold because its 95% CI `[-18,+2]` excludes benefits of 25 s or larger, whereas Study A `[-55,+19]` still allows large benefit and worsening (2.0).

The conclusion comes from observed estimate/precision relative to the threshold, not from a binary p-value (1.0).

Observed/post-hoc power computed from the observed effect is redundant/misleading for completed-study interpretation; prospective power belongs to design assumptions, while completed-study informativeness is visible in estimate/CI and design limitations (1.0).

**Remediation:** F0.6 → F0.5.

## B5 — 4 points

- multiplicity arises from six outcomes × three timepoints plus sex subgrouping, model choices and any pairwise/derived contrasts; the exact effective family depends on the claim/decision strategy rather than simple multiplication alone (1.5);
- a week-8 subgroup p=.03 cannot be declared prospectively confirmatory from the given information, especially when registry identifies a primary outcome at week 12 and no public SAP resolves subgroup/model plans (1.25);
- seek prospectively timestamped protocol/SAP/registry version history specifying outcome hierarchy, subgroup hypotheses, timepoints, models and multiplicity control (1.25).

**CRITICAL_FAIL:** highlighted p=.03 treated as confirmatory while obvious multiplicity is ignored.

**Remediation:** F0.6.

---

# Section C — 20 points

## C1 — 8 points

Full-credit elements:

- negative MD means faster/better performance for R (0.75);
- A/D have relatively narrow intervals and high displayed weights; E has wide CI/lower weight; weight reflects model-dependent precision/contribution, not study quality or certainty (1.25);
- pooled estimate `-17 s [−31,−3]`, favoring R on average under the random-effects synthesis (1.0);
- `I²=74%` indicates substantial statistical heterogeneity relative to sampling variation under its assumptions; it is not “74% of studies are heterogeneous,” a quality score, proof of invalid pooling, or proof all studies differ in one known way (1.5);
- plausible heterogeneity: trained vs recreational status; running/cycling/triathlon context; hot environment; possible intervention dose/duration/protocol differences represented by context (at least two = 1.5);
- scientific usefulness of pooling depends on construct/effect-measure/target compatibility and whether an average effect is meaningful despite clinical/methodological diversity; I² alone cannot answer that (2.0).

**CRITICAL_FAIL:** low/high I² used as automatic proof of sameness/invalidity in a structural way.

**Remediation:** F0.7 → F0.5/F0.6 as needed.

## C2 — 5 points

Trust/audit strengths, any two with explanation (up to 2): prospective protocol registration; duplicate independent screening; verification of extraction; structured RoB2; declared random-effects plan.

Potential missing-evidence/process limitations, any two (up to 1.5): only two bibliographic databases; English/full-text journal restriction; explicit absence of registry/grey-literature searching. These can miss eligible evidence and create dissemination/language/publication selection concerns.

Unclear rather than proven wrong (0.75): whether primary synthesis/outcome hierarchy matches the registered protocol; must compare documents rather than infer from missing statement.

PRISMA point (0.75): complete reporting makes methods visible but does not certify low review bias, low study-level RoB or high certainty.

**CRITICAL_FAIL:** PRISMA completeness = high quality/certainty.

**Remediation:** F0.7/F0.8.

## C3 — 7 points

Body A deserves substantially greater certainty for the stated target (1.5): randomized, direct, precise around/above the +0.6 threshold, broadly consistent, lower RoB.

Domains separating bodies (2.0): risk of bias/confounding/missingness; imprecision; inconsistency; indirectness (population, proxy outcome, short duration); possibly dissemination evidence if supplied—not invent if absent.

Applicability (1.25): A closely matches trained endurance athletes, validated outcome and duration; B is indirect due recreational/untrained populations, proxy outcome and 2–4 weeks.

Similar point estimates do not imply similar evidence strength (1.25): compatible ranges, bias mechanisms, directness and consistency differ markedly.

Recommendation boundary (1.0): certainty about one performance outcome is only one input; recommendation can also depend on harms, burden/cost, values/preferences, feasibility and other outcomes.

**CRITICAL_FAIL:** B low certainty translated to “no effect,” or A high certainty translated automatically to strong recommendation.

**Remediation:** F0.8 → F0.5/F0.7 if underlying reason.

---

# Section D — 25 points

## Source facts used for scoring

Assigned paper: Jagłowska et al., *Nutrients* 2026;18(15):2484, doi:10.3390/nu18152484.

The paper is open access under CC BY and is used as an appraisal object, not as a substantive recommendation.

### D1 — Question/estimand — 3 points

Expected reconstruction:

- trained adult male long-distance/endurance runners;
- multistrain probiotic for four weeks while receiving the standardized diet;
- matched placebo under the same diet/training instructions;
- primary performance outcome VO2peak from incremental treadmill testing;
- PRE→POST four-week horizon;
- primary effect is the between-group difference in change represented by the `group × phase` interaction.

The title is broader than the single primary estimand because it also speaks across exercise performance and inflammatory responses; the study legitimately includes many secondary outcomes, but those are distinct estimands/results.

Scoring: PICO/time 2; estimand/model contrast 0.75; title-scope audit 0.25.

### D2 — Design/selection — 3 points

Expected:

- preliminary/exploratory randomized double-blind parallel placebo-controlled trial;
- 30 randomized, 27 completed/analyzed (PRO 13, PLA 14);
- independent randomization list, coded identical containers/allocation concealment reported; blinding reportedly maintained through analysis;
- randomization protects baseline confounding in principle for assigned treatment contrast;
- remaining selection/generalizability constraints include modest sample, male-only competitive/trained long-distance runners and recruitment feasibility.

Do not require “low risk” label from design alone.

### D3 — Measurement/fidelity — 2 points

Credit any two material, correctly explained features, e.g.:

- standardized meal-box diet reduces dietary variability/co-intervention differences but adherence was verified partly by interview/report rather than perfect objective intake measurement;
- capsule adherence by count approximately 92% PRO vs 88% PLA;
- training load monitored with diaries/HR/RPE and reported comparable, but self-reported diaries introduce measurement error;
- placebo capsules matched in appearance/excipients;
- VO2peak/treadmill and Wingate provide direct measured performance physiology, but repeated testing/familiarization and instrument/protocol context still matter.

1 point each, max 2.

### D4 — Result-specific bias/missingness — 4 points

A strong appraisal for the primary VO2peak result should address:

- randomization/allocation: described independent sequence, concealment and blinding support the randomized contrast (0.8);
- deviations/adherence: similar diet/training instructions, matched placebo, adherence reasonably high; small adherence difference alone is not proof of bias (0.6);
- missingness/analysis population: three participants withdrew before POST; per-protocol/complete-case analysis excluded them and no imputation was used. Authors report personal reasons unrelated to intervention, but exclusion after randomization can still matter; mixed models retained isolated available measurements under MAR when applicable (1.0);
- measurement: primary VO2peak is comparatively objective, lowering concern from assessor subjectivity relative to subjective outcomes, but measurement/familiarization/protocol remain considerations (0.6);
- selective reporting: many outcomes and retrospective public registration make result-selection/multiplicity audit important; FDR was used, but public registry timing cannot prove prospective hierarchy. The paper also states gut-microbiota outcome is reported separately (1.0).

Accept a calibrated overall judgment such as low/some concerns for certain domains with some concern around missingness/selection-of-reported-result, provided reasoning is result-specific. Do not demand a single overall label.

### D5 — Analysis/prespecification/multiplicity — 3 points

Expected:

- a-priori calculation targeted total n=40, 80.4% power, one-sided alpha=.05 and large d=.82 anchored to a TNF-alpha effect from a different athletic population/formulation; only 30 randomized/27 completed, so target not reached and small/moderate effects are poorly excluded (0.75);
- VO2peak is designated primary performance outcome; many secondary performance/biomarker outcomes create multiplicity (0.5);
- linear mixed models and Benjamini–Hochberg FDR correction across the outcome family are reported; learner should distinguish correction from proof of prespecification (0.5);
- paper explicitly says registry `NCT07411482` was first submitted 31 Dec 2025 and posted 13 Feb 2026 after participant enrolment/study conduct, so public registry is retrospective and cannot independently prove prospective outcome/model specification (0.75);
- article claims primary/secondary outcomes and sample-size calculation were specified earlier in bioethics/grant documents. That may be relevant evidence if those timestamped documents are inspected, but the current public registry alone cannot verify it. Extra credit within existing points for noticing the article's institutional statement uses inconsistent “prospectively registered… prior to enrollment” wording; timeline should control the judgment (0.5 distributed within above categories).

### D6 — Effect/uncertainty — 4 points

Primary VO2peak group×phase estimate:

`-3.5 mL·kg^-1·min^-1` (paper reports approximately −3.54), `95% CI −7.0 to −0.1`, nominal `p=0.044`, Cohen d about −0.75; direction is opposite the hypothesized probiotic benefit because PRO decreased relative to PLA (1.0).

After Benjamini–Hochberg correction, adjusted `p=0.707`; therefore the nominal p=.044 is not treated as a multiplicity-controlled confirmatory signal (0.75).

CI interpretation (1.0): under the reported model/procedure, values from a small negative difference to a materially more negative difference remain compatible; the CI excludes exactly zero in the nominal unadjusted analysis but does not encode posterior probability and cannot by itself establish practical importance.

Binary-statistics boundary (0.75): neither nominal significance means “true harm” nor adjusted nonsignificance means “no effect.” Consider estimate, CI, multiplicity plan, achieved information, bias and target threshold.

Equivalence/practical-absence boundary (0.5): a defensible practical threshold/equivalence margin and appropriate design/analysis are needed; a nonsignificant multiplicity-adjusted superiority test is not formal equivalence.

### D7 — Applicability — 2 points

Relatively good: trained adult male long-distance/endurance runners using the same/similar probiotic formulation, four-week duration, standardized diet and comparable training/testing context.

Weaker: female endurance athletes; sedentary/recreational populations; other sports; longer durations; different strains/dose/diet; clinical populations; real-world diets/training without standardization; outcomes such as illness incidence or race performance not directly measured.

1 point for each side with structured reasoning.

### D8 — Authors' conclusion — 2 points

A strong answer recognizes that the authors are generally cautious: they explicitly frame the study as exploratory/preliminary, note modest sample, state “absence of demonstrable effect under these specific conditions” rather than universal inertness, and call for adequately powered/prespecified work.

Qualification required: phrases like “did not produce statistically significant effects” are accurate only in the multiplicity-adjusted/reporting sense and should not be read as evidence of equivalence or absence of potentially meaningful small/moderate effects. The nominal primary estimate was in the opposite direction and its CI/adjustment must remain visible.

Credit 1 for proportionality judgment + 1 for justified wording audit.

### D9 — What it does not prove — 2 points

Any three defensible boundaries, with at least one mechanism and one absence/generalization boundary. Examples:

- does not prove probiotics have no effect in endurance athletes;
- does not establish formal equivalence/inferiority/superiority around a prespecified practical margin;
- does not establish effects in women or different training populations;
- does not establish longer-term effects or other strains/doses;
- does not establish gut-microbiome mechanism because microbiome/metabolites were not directly measured in this reported paper;
- does not convert exercise-induced cytokine changes into a clinically meaningful health effect;
- does not establish body-of-evidence certainty from one trial.

Scoring: 0.5 each for first three valid boundaries + 0.5 for satisfying required mechanism + absence/generalization diversity.

**Section D cap:** checklist-only yes/no responding cannot exceed 15/25.

**Possible D critical fails:** within-group changes used as treatment effect; adjusted p=.707 interpreted as proof of no effect; nominal p=.044 treated as truth/importance without multiplicity; retrospective registry called prospectively prespecified without timeline; invented protocol facts; one-paper GRADE certainty rating.

**Remediation:** full-paper chain failures → F0.9, then earliest broken dependency (F0.1–F0.8) according to error.

---

# Section E — 10 points

Invariant core:

- target: trained adult endurance athletes, T vs placebo, 8–12 weeks, validated 5 km performance, lower better;
- MD `-9 s`;
- 95% CI `[-22,+4]`;
- practical-benefit threshold `-20 s`;
- interval crosses both null and threshold;
- moderate certainty, mainly imprecision;
- direct to trained endurance athletes, not established for sedentary/clinical populations;
- no formal equivalence claim.

## E1 + E2 scoring

### Epistemic calibration — 4 points

Both versions must communicate that the estimate favors a small benefit but uncertainty still includes a practically important benefit and little/no difference. Neither may say “works,” “doesn't work,” “equivalent,” or “proven.” Plain version cannot be more certain.

### Magnitude/uncertainty — 2 points

Technical should retain numerical MD/CI/threshold. Plain language may translate them but must preserve that `-20 s` lies within the compatible range and zero also lies within it.

### Scope/applicability — 2 points

Must retain trained-endurance context and avoid generalization to everyone/sedentary/clinical populations.

### Clarity without distortion — 2 points

Language should be readable and audience-appropriate while preserving certainty and boundaries.

One acceptable technical synthesis:

> Across seven direct randomized trials in trained endurance athletes, Intervention T was associated with a pooled 5 km time difference of −9 s versus placebo (95% CI −22 to +4 s). The point estimate favors T, but the interval includes both the prespecified practically important benefit threshold of −20 s and little/no difference. Certainty is moderate, limited mainly by imprecision around that threshold. These data therefore do not establish a clear practically important benefit, but they also do not exclude one. The evidence is reasonably direct for trained endurance athletes over 8–12 weeks and should not be generalized automatically to sedentary or clinical populations. This is not formal equivalence evidence.

One acceptable plain version:

> In trained endurance athletes, the best estimate was about 9 seconds faster with T, but the uncertainty is wide enough that the true effect could be a meaningful improvement or almost no difference. Confidence is moderate because the studies still do not pin down whether the benefit reaches the 20-second threshold considered important. The result applies most directly to trained endurance athletes studied for roughly 8–12 weeks and does not show that T is equivalent to placebo or that the same result applies to other populations.

**CRITICAL_FAIL:** simplified version materially more certain than technical; moderate certainty → definitive recommendation; `CI crosses zero = no effect`.

**Remediation:** F0.10 → F0.8/F0.5 depending cause.

---

# Section thresholds

Minimum section scores required for exit passage:

- A: `14/20`;
- B: `17.5/25`;
- C: `14/20`;
- D: `17.5/25`;
- E: `7/10`.

For operational scoring, half-points are allowed. Do not round a below-threshold section upward solely to create a pass.

---

# Final classification

## PASS

All:

- total `>=85`;
- every section >=70%;
- no critical fail;
- D shows integrated appraisal chain;
- E preserves uncertainty.

A first PASS supports evidence for `APPLIED` and potentially `INTEGRATED` across F0, subject to actual performance review. It does not automatically set `MASTERED`.

## NEAR_PASS / TARGETED_REMEDIATION

- total `75–84`;
- no critical fail;
- remediate the earliest broken dependency, then use new numbers/scenarios/paper for retest.

## BROADER_REMEDIATION

- total `<75`, or a pattern of section failures indicating structural gaps.

## CRITICAL_FAIL

Any global critical-fail misconception blocks passage and requires targeted conceptual repair before alternate-form retest.

---

# Remediation map

| Observed error | Earliest remediation |
|---|---|
| vague/unanswerable claim | F0.1 |
| design label without inference boundary | F0.2 |
| adjusted association asserted causal / collider-mediator error | F0.3 → F0.2 |
| distribution, SD/SE, absolute-relative confusion | F0.4 |
| CI/p-value/threshold/practical-significance error | F0.5 → F0.4 if necessary |
| power/multiplicity/prespecification error | F0.6 → F0.5 |
| pooled estimate/I²/heterogeneity error | F0.7 → F0.5/F0.6 |
| reporting completeness used as validity/certainty | F0.8 → F0.2/F0.3 |
| paper appraisal becomes summary/checklist only | F0.9 + earliest broken prior unit |
| simplified language becomes more certain / recommendation collapse | F0.10 → F0.8/F0.5 |

Actual persistent learner errors should be entered into `study/ERROR_LEDGER.md` only after observed administration. Production of this key creates no learner-state evidence.
