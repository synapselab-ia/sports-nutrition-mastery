# F0.9 — Gabarito comentado

**Assessment:** `EXERCISES.md`

**Total:** 100 points

**Pass gate:** `>=80/100 + no critical fail`

This key scores reasoning, not phrase matching. Equivalent technically defensible wording earns credit.

For the real-paper task, do not penalize a learner for marking genuinely unavailable information as `UNCLEAR / NOT REPORTED` when they explain why it matters.

---

# A — Paper anatomy and extraction discipline — 15 points

## A1 — 6 points

Full credit should include at least eight components with functions, for example:

- title/abstract: locate stated question/design/claims, not final appraisal;
- introduction: rationale/hypothesis;
- methods: eligibility, allocation/exposure, interventions, outcomes, sample-size logic, model, missingness;
- participant flow: randomized/eligible/analyzed/missing;
- results tables/figures: extract estimates and uncertainty independently;
- discussion: compare authors' interpretation with extracted evidence;
- supplement: recover omitted analyses/outcome definitions;
- registry/protocol/SAP: audit prespecification and deviations;
- data/code: auditability/reanalysis potential;
- version/correction notices: ensure the right evidentiary object is being appraised.

Required explanation: the abstract is compressed and can omit methods, uncertainty, multiplicity, prespecification and missing-data information.

Deduct heavily if abstract is treated as sufficient.

## A2 — 5 points

Expected extraction:

| Field | Expected answer |
|---|---|
| Population | sedentary adults 55–70 eligible for trial |
| Intervention | 12-week supervised resistance training + beverage X |
| Comparator | same training + placebo |
| Outcome | leg-press 1-RM change |
| Time | baseline to week 12 |
| Estimand/contrast | mean between-group difference in 12-week 1-RM change under the stated model |
| Analysis population needed | e.g. all randomized/ITT versus completers/per-protocol must be established |
| Target-context field | e.g. whether intended target is trained athletes, older adults, women, elite athletes, etc. |

Full credit requires a **between-group** estimand, not “change in the intervention group.”

## A3 — 4 points

Expected result record:

- outcome/timepoint: week-12 change in leg-press 1-RM;
- contrast: X vs placebo;
- effect measure: MD in change;
- estimate: +4.0 kg;
- 95% CI: −2.0 to +10.0 kg;
- p=0.18;
- analysis population: not specified in vignette;
- prespecification: not specified;
- practical threshold: not specified;
- caveat: interval includes values favoring control and potentially relevant benefit.

Acceptable sentence:

> The point estimate favors X by 4 kg, but the interval remains compatible with effects from 2 kg worse to 10 kg better than placebo, so the data do not establish absence or meaningful benefit without a defensible threshold.

No credit for `p=0.18 therefore no effect`.

---

# B — Prespecification, bias and inferential architecture — 20 points

## B1 — 7 points

Expected:

1. Registry/SAP can document what was declared by February/March 2024 and improve retrospective transparency.
2. Because final outcomes were collected by December 2023, those timestamps do not establish that the choices were fixed before results could be known.
3. Use wording such as `retrospectively documented/registered`, `reported in a post-completion registry/SAP`, or `prospective prespecification not verifiable from these documents`.
4. Retrospective registration does not erase randomization, measurements or observed data; it specifically weakens evidence that outcome/analysis choices were protected from result-driven selection.

Critical error: treating late registration as prospective solely because a registry exists.

## B2 — 7 points

### Sprint result

Likely concerns are relatively smaller from outcome measurement and missingness if timing is automated and missingness is low/balanced. Randomization process still needs its own evidence; selective result reporting remains an independent question.

### Recovery rating

Material concerns include:

- unblinded assessor for a subjective outcome;
- differential missingness plausibly related to symptoms/outcome;
- possible selection among multiple scoring methods if not prespecified.

A single score is invalid because mechanisms differ by **result** and can matter differently.

If scoring-method selection was not prospectively documented, correct answer is uncertainty about selective reporting/analysis, not an invented claim that selection definitely occurred.

## B3 — 3 points

Expected repair:

> CONSORT completeness improves reporting visibility. It does not establish low risk of bias; validity requires result-specific appraisal of randomization, deviations, missingness, measurement and selective reporting among other issues.

## B4 — 3 points

Expected:

- randomization protects the baseline assignment contrast against systematic confounding in expectation when implemented correctly, but post-randomization deviations, missingness, measurement and selective reporting can still bias a result;
- observational evidence requires stronger confounding/selection assumptions for causal intervention questions but can still be informative when design/data/analysis fit the question.

---

# C — Quantitative interpretation, multiplicity and robustness — 20 points

## C1 — 5 points

The treatment-effect result is the **between-group MD in change**:

`+3 [−1,+7]`.

Expected interpretation:

- point estimate favors intervention by 3 units;
- CI includes a small effect favoring control through a larger benefit;
- within-group p-values do not answer whether groups differ;
- practical meaning requires the outcome scale and a defensible threshold.

Critical error: concluding efficacy because the intervention improved with p<0.001 while control had p=0.01.

## C2 — 5 points

`p=0.31` does not demonstrate equivalence.

Full-credit answer should mention:

- direct effect estimate + CI for the group difference/interaction;
- a prospectively defensible equivalence or practical-importance margin;
- an analysis/design capable of evaluating that margin;
- enough precision for the interval to exclude effects outside the no-important-difference region.

For formal equivalence, an equivalence design/test and margin are required. For a less formal “no important difference” claim, threshold-aware interval reasoning is still needed.

## C3 — 4 points

Expected repair:

> Observed/post hoc power computed after seeing the data is not posterior probability of a false negative and does not provide independent evidence about whether the observed result is real. Interpret the completed study using the effect estimate, CI, practical threshold, design assumptions and bias/analysis context.

Prospective design power remains conceptually distinct.

## C4 — 6 points

Expected:

- the opportunity set includes multiple outcomes, times, subgroups and models;
- registry/protocol/SAP/timestamps are needed to determine prospective status;
- the unregistered subgroup result should generally be treated as exploratory/post hoc unless earlier documentation exists;
- subgroup inference requires a direct interaction/difference test, not significance in one subgroup and nonsignificance in another;
- robust reporting discloses all planned analyses, deviations, multiplicity strategy and exploratory status.

---

# D — Blind full-paper critical appraisal — 45 points

## Performance source

Klemp AO, Ormsbee MJ, Yeh M, et al. *Neither pre-sleep nor post-exercise protein consumption influences resistance exercise training adaptations in older adults*. J Int Soc Sports Nutr. 2025;22(1):2519511. doi:10.1080/15502783.2025.2519511.

This key is a structured appraisal of the **reported paper/registry**, not a formal misconduct judgment and not a complete GRADE rating of the literature.

## D1 — Provenance and article map — 3 points

Expected:

- peer-reviewed 2025 JISSN article; DOI above; open-access full text available via publisher/PMC;
- article is distributed under CC BY 4.0;
- ClinicalTrials.gov identifier `NCT05922475` exists;
- article identifies an OSF data repository;
- trial began in 2017 and completed in 2019;
- registry was first submitted/posted in 2023, after completion;
- therefore the registry is **retrospective** for this trial and cannot by itself establish prospective outcome/analysis prespecification.

Full credit requires temporal reasoning, not merely copying “retrospectively registered.”

## D2 — Question and estimand — 5 points

A strong extraction resembles:

| Field | Appraisal |
|---|---|
| Population | sedentary/untrained men aged 60–75; analyzed completers around mean age 65.7 y; baseline protein intake already roughly adequate in the paper's framing |
| Intervention 1 | supervised RET + 40 g mixed whey/casein protein immediately post-exercise; placebo at pre-sleep timing |
| Intervention 2 | same RET + placebo post-exercise + 40 g protein pre-sleep |
| Comparator | same supervised RET, no supplemental protein |
| Outcomes | quadriceps muscle thickness and 1-RM strength |
| Time | weeks 0, 6 and 12; main chronic comparison through 12 weeks |
| Main contrasts | PRP vs PSP tests timing among supplemented conditions; PRP/PSP vs RETO test supplemented strategies versus RET-only comparator |
| Analysis population | 30 completers analyzed from 32 randomized/enrolled |

Important distinction:

- `PRP vs PSP` is the cleanest timing contrast because both receive the same protein product at different times.
- `PRP/PSP vs RETO` is not a pure timing comparison; it also contrasts supplementation with no supplement and changes nutrient/energy exposure.

The precise causal estimand is not fully formalized in ICH-style terms in the paper; credit `not fully explicit` if the learner reconstructs the intended between-group longitudinal contrast.

## D3 — Design and sampling — 4 points

Expected:

- three-arm, parallel, randomized trial over 12 weeks;
- described as double-blind/placebo-controlled for the supplemented timing conditions;
- covariate-adaptive randomization intended to balance baseline protein intake, using randomizer.org;
- 32 randomized/enrolled; 30 completed/analyzed: PRP 9, PSP 11, RETO 10;
- two withdrawals/dropouts occurred, one from PSP and one RETO, reported as injuries;
- randomization supports baseline exchangeability of assignment in principle;
- it does not by itself settle allocation implementation, post-randomization deviations, outcome measurement, missingness, selective reporting or applicability.

Do not award full credit for merely saying “RCT = high quality.”

## D4 — Intervention/comparator and outcome measurement — 5 points

### Intervention exposure

PRP/PSP received a 40 g mixed protein supplement (whey/casein blend; the paper reports 265 kcal, 40 g protein, 15 g carbohydrate and 5 g fat) daily under different timing rules. Both performed the same supervised RET program.

RETO performed RET but received no protein supplement and therefore was not blinded to group assignment.

Training attendance and supplement compliance were high in the report (approximately 96% and 97%, respectively).

### Contrast contamination/interpretation

`PRP vs PSP` largely isolates timing of the same supplemental product.

`PRP or PSP vs RETO` does **not** isolate protein as a nutrient independently of all other exposure differences because supplemented groups receive extra energy/macronutrients/product while RETO does not receive an energy-matched nutritional comparator.

This issue would matter especially if one attempted a strong nutrient-specific causal claim.

### Outcomes

- ultrasound muscle thickness of VL/RF/VI;
- 1-RM leg press and chest press.

Reasonable limitations:

- muscle thickness at limited sites is not identical to whole-muscle hypertrophy/body composition;
- 1-RM can contain test familiarity/motivation components even though it is directly performance-related to the trained/tested movement;
- outcome-assessor blinding must be established from reported information rather than assumed from the word “double-blind.”

## D5 — Bias/confounding/missingness — 5 points

### Randomization process

Paper describes random allocation/covariate adaptation, which is favorable, but a formal RoB 2 judgment would still examine sequence/concealment and baseline evidence. Do not infer low risk solely from `randomized`.

### Deviations / knowledge of assignment

PRP/PSP used matched timing placebo/protein procedures; RETO received no supplement and knew its assignment. That asymmetry could affect behavior/expectations, although the materiality differs by outcome.

### Missing outcome data

Two of 32 randomized participants did not complete; analysis presented 30 completers. The reported reasons (injury, one in PSP and one in RETO) and small number reduce concern relative to substantial differential attrition, but do not justify ignoring analysis-population consequences.

### Measurement

Muscle thickness is more objective than a subjective self-report but assessor procedures/blinding must be verified rather than assumed. Strength testing may be influenced by effort/motivation/familiarization; standardized supervised testing helps but does not make measurement bias impossible.

### Selection of reported result

This is a material appraisal issue because:

- registry was retrospective;
- article states these data are a subset of a larger project with additional outcomes;
- therefore prospective protection against outcome/analysis selection cannot be demonstrated from the registry timestamp alone.

A defensible answer need not declare `high risk` mechanically. It must explain why selective-result bias is **not prospectively auditable** from the late registry.

## D6 — Sample size, analysis plan and prespecification — 6 points

Expected extraction:

- linear mixed-effects models with REML;
- fixed factors: time (0, 6, 12 weeks) and group (PRP, PSP, RETO);
- participant random intercept for repeated measurements;
- Kenward–Roger degrees of freedom/p-values;
- significance threshold p<0.05;
- Sidak-adjusted pairwise comparisons/CIs for significant effects;
- Q-Q checks and transformations where reported;
- n=30 analyzed.

### Sensitivity power analysis

The paper reports a post-study sensitivity power calculation using N=30 and model residual variability, yielding a minimum detectable f≈0.66 and translating this to about 0.21 cm total muscle thickness and ~11 kg total 1-RM under the stated assumptions.

Correct interpretation:

- it describes design sensitivity under chosen assumptions;
- it is **not** posterior probability that the null is true/false;
- it does not convert nonsignificant group×time interactions into equivalence;
- it does not substitute for direct between-group effect estimates/CIs relative to a meaningful threshold.

### Prespecification

- study completed in 2019;
- registry submitted/posted in 2023;
- prospective prespecification cannot be established from that registry;
- current registry can document what was later declared (including muscle thickness as primary and several secondary outcomes), but temporal protection from result-driven selection is absent.

Because the paper reports being a subset of a larger project with additional outcomes, multiplicity/selection opportunities deserve explicit attention; this is not proof of selective reporting by itself.

## D7 — Main estimates and uncertainty — 6 points

Full credit separates **time effects** from **between-group effects**.

Examples reported for week 0→12 across the trial/model include:

- VL muscle thickness: about `+0.16 cm [0.06,0.25]`;
- RF: about `+0.13 cm [0.03,0.23]`;
- VI: about `+0.18 cm [0.05,0.31]`;
- chest press 1-RM: about `+10.9 kg [5.50,16.3]`;
- leg press 1-RM: about `+28.3 kg [19.63,37.1]`.

These show improvement over time under the training program; they are not themselves estimates that PRP or PSP outperformed RETO.

The paper reports no statistically significant group-related/group×time differences for the main outcomes.

Key appraisal point:

> A nonsignificant interaction/group effect is not equivalent to a precise estimate of zero.

The report emphasizes time-effect CIs but does not make a complete set of directly interpretable **between-group treatment-effect CIs** central/visible enough to establish equivalence or rule out smaller meaningful added effects.

There is no clearly prospectively defined practical/equivalence threshold for the supplementation/timing contrast.

Therefore, a strong answer says:

- no differential adaptation was statistically detected in this sample/model;
- the study does not formally establish equivalence/no meaningful added effect across all plausible thresholds.

Do not require the learner to manufacture a CI that is not reported.

## D8 — Multiplicity and robustness — 3 points

Possible creditworthy features:

- multiple muscle-thickness sites;
- multiple strength outcomes;
- three measurement timepoints;
- pairwise comparisons after significant effects with Sidak adjustment;
- transformations/normality checks;
- post-study sensitivity power analysis;
- registry is retrospective;
- paper is a subset of a larger project with additional outcomes;
- public data repository improves auditability/reanalysis potential.

Classification rule:

- the late registry cannot establish that outcome hierarchy or analysis decisions were prospectively confirmatory;
- muscle thickness is listed as primary in the current registry and strength as secondary, but those labels were posted after study completion;
- where no earlier timestamped protocol/SAP is available, `prospective status unclear/not verifiable` is preferable to invented certainty.

## D9 — Applicability — 3 points

Target = trained competitive athletes.

Material mismatches include:

- study participants were older men, not a broad athlete population;
- they were sedentary/untrained before intervention;
- baseline protein intake was already around/above the study's “adequate” context;
- training was supervised resistance training twice weekly rather than high-volume competitive programming;
- specific 40 g mixed whey/casein product/timing rules were used;
- outcomes were local quadriceps thickness and machine 1-RM, not competition performance;
- duration was 12 weeks;
- women, younger athletes and lower-protein populations were not represented.

Mechanism matters: training status, habitual protein intake, age-related anabolic responsiveness, total training stimulus and outcome relevance can modify the practical effect of supplemental protein/timing.

Conclusion: applicability to trained competitive athletes is limited; this is separate from internal validity.

## D10 — Final synthesis — 5 points

### a. Strongest defensible inference

A model answer:

> In 30 completing previously untrained older men undertaking supervised twice-weekly resistance training, the study detected substantial 12-week increases in quadriceps thickness and 1-RM but did not detect differential adaptation among post-exercise protein, pre-sleep protein and training-only groups. Because direct between-group uncertainty relative to a prospectively defined meaningful margin is not fully demonstrated, and registration occurred after study completion, the result supports “no added difference detected under these conditions” more strongly than formal equivalence or a universal claim that protein timing/additional protein cannot matter.

Equivalent calibrated wording earns full credit.

### b. Authors' conclusion audit

Best-supported classification: **partly proportional**, with justification.

Why:

- proportional part: in this sample/model, no group-related difference was statistically detected while training adaptations occurred;
- stronger part: wording such as “does not enhance” and “timing should not be emphasized” can be read as an absence/equivalence conclusion broader than the directly visible between-group precision and prospective-prespecification evidence support;
- context qualification (untrained older adults with adequate baseline protein) improves proportionality and should receive credit;
- the learner should not claim the conclusion is simply “wrong.”

A learner may defend `proportional` or `overextended` for parts of the conclusion if the argument explicitly engages the contrast, CI visibility/thresholds, registration timing and population scope. The scoring target is calibrated reasoning, not one magic label.

### c. What the paper does not prove

Any five well-defended boundaries, such as:

- protein timing never matters;
- protein supplementation is useless in older adults;
- the three strategies are formally equivalent;
- smaller but meaningful group effects are excluded;
- results apply to women;
- results apply to younger/trained/elite athletes;
- results apply to people with low baseline protein intake;
- every protein source/dose/timing is equivalent;
- local muscle thickness equals whole-body hypertrophy;
- machine 1-RM results establish competition-performance effects;
- a post-study power calculation proves adequate/inadequate evidence for the observed null;
- the retrospective registry proves analyses were prospectively prespecified;
- one trial settles body-of-evidence certainty or recommendation strength.

---

# Critical fails — grading enforcement

Any material instance below blocks a pass until repaired:

1. abstract-only appraisal;
2. `RCT = valid/low bias` without mechanism-level appraisal;
3. checklist score as validity;
4. `p<0.05 = true/important`;
5. `p>0.05 = no effect/equivalence`;
6. observed/post hoc power used as posterior/rescue evidence;
7. retrospective registry called prospectively prespecified;
8. material multiplicity/selection opportunities ignored;
9. reporting completeness equated with low RoB;
10. one paper-level RoB/certainty score substituted for result-specific reasoning;
11. within-group time effect called between-group treatment effect;
12. unsupported acute→chronic/mechanistic→performance extrapolation;
13. conclusion copied rather than reconstructed;
14. missing methodological information invented;
15. single paper assigned body-of-evidence GRADE certainty as if equivalent objects.

---

# Remediation routing

- vague question/estimand → F0.1;
- design-label reasoning → F0.2;
- bias mechanism failure → F0.3;
- SD/SE/descriptive confusion → F0.4;
- p-value/CI/magnitude failure → F0.5;
- power/multiplicity/prespecification failure → F0.6;
- evidence-body/meta-analysis confusion → F0.7;
- RoB/certainty/applicability collapse → F0.8.

Do not mark F0.9 `MASTERED` from this production key. Mastery requires observed learner performance.
