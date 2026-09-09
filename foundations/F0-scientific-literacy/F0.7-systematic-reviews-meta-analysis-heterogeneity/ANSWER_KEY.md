# F0.7 — Gabarito comentado

**Purpose:** scoring/reference after an independent attempt.

**Do not use this file during the first attempt.**

**Total:** 100 pontos.

**Gate:** `>=80/100` + nenhum critical fail.

Partial credit is allowed when reasoning is directionally correct but one detail/calculation is incomplete. Structural misconceptions listed as critical fails block progression regardless of total score.

---

# Parte A — 15 pontos

## A1 — 5 pontos

Expected:

### Systematic review

A structured evidence-review process using explicit methods for question/protocol, eligibility, search, selection, extraction, appraisal, synthesis and interpretation.

### Meta-analysis

A statistical combination of effect estimates/results from two or more separate studies.

### Why review can exist without meta-analysis

Correct answers recognize that studies may be too clinically/methodologically/statistically incompatible for a meaningful pooled estimate. A structured narrative/tabular synthesis may be more defensible.

### Why meta-analysis can be weak without systematic selection

If study identification/inclusion is selective, the pooled number summarizes a biased subset regardless of the statistical sophistication.

**Critical fail:** systematic review and meta-analysis treated as synonyms.

## A2 — 6 pontos

Reasonable sequence:

1. protocol/question;
2. eligibility criteria;
3. search;
4. screening/selection;
5. extraction;
6. effect-measure choice/compatibility;
7. synthesis;
8. heterogeneity/missing-evidence interpretation.

Accept slight ordering nuance where effect-measure/synthesis planning is prespecified earlier, provided the learner explains that the synthesis plan should ideally be planned before seeing results.

Full credit requires each stage’s purpose, not only ordering.

## A3 — 4 pontos

Expected correction:

### What PRISMA does

- reporting guideline;
- improves transparency/completeness about question, eligibility, search, selection, synthesis, results, protocol/registration and related items;
- makes methods/results more auditable.

### What PRISMA does not do

- does not prove correct methods;
- does not certify low risk of bias;
- does not establish high certainty;
- does not make included studies valid.

**Critical fail:** PRISMA completion equated with study/review quality or low bias.

---

# Parte B — 20 pontos

## B1 — 6 pontos

1. A and B can provisionally be pooled directly as MD because they use the same effect measure and stated same scale/construct, subject to population/timepoint/unit compatibility.
2. C is SMD; `0.40 SD units` is not `0.40 original units`. It cannot simply be numerically appended to an MD synthesis.
3. D is RR for a binary outcome; it answers a different scale/type of outcome and null is 1 rather than 0. Directional favorability alone does not create numerical compatibility.
4. Needed checks include:
   - same/compatible construct;
   - outcome direction;
   - time point;
   - population/intervention/comparator;
   - unit-of-analysis structure;
   - valid transformation/conversion if used;
   - avoidance of duplicated participants/reports.

**Critical fail:** “same direction = directly poolable.”

## B2 — 6 pontos

Formula:

`inverse variance = 1/SE²`.

### Study A

`1 / 0.20² = 1 / 0.04 = 25`.

### Study B

`1 / 0.40² = 1 / 0.16 = 6.25`.

A gets more weight.

Ratio:

`25 / 6.25 = 4`.

So A receives about four times the inverse-variance weight in the simple setup.

Why this is not quality:

- weight describes statistical precision under the synthesis model;
- a precise large study can still be biased or methodologically inappropriate;
- bias/certainty need separate appraisal.

**Critical fail:** weight = quality/certainty.

## B3 — 8 pontos

1. **Incorrect.** Fixed/random models are synthesis models, not bias corrections.
2. **Correct**, as the F0.7 common interpretation of fixed effect.
3. **Correct.** Random effects permits different related underlying effects and summarizes an average under an assumed distribution.
4. **Incorrect.** Random effects models heterogeneity; it does not make diversity irrelevant or identify its causes.
5. **Incorrect.** Model choice should follow target quantity/model plausibility, not only a heterogeneity-test p-value.
6. **Correct.** Addition of between-study variance tends to make weights more similar; smaller studies receive relatively more weight than under fixed effect.

Full credit requires explaining that random-effects CI concerns the average effect and does not automatically describe the entire distribution of effects.

---

# Parte C — 25 pontos

## C1 — 7 pontos

Expected forest-plot elements include at least seven:

- study label;
- study point estimate;
- study CI line;
- null/reference line;
- effect measure/scale;
- study weight/marker size;
- pooled estimate diamond;
- pooled CI width;
- subgroup labels when present;
- heterogeneity statistics;
- direction labels.

Why diamond ≠ true effect:

It is a model-dependent summary estimate computed from selected/processed study estimates. Its meaning depends on effect compatibility, weights, model assumptions, heterogeneity and evidence quality.

## C2 — 8 pontos

1. Elite versus recreational → primarily **clinical diversity**.
2. Blinded versus unblinded outcome assessment → primarily **methodological diversity**.
3. Effects differ more than expected from sampling error → **statistical heterogeneity signal**.
4. 2 versus 12 weeks → primarily **clinical diversity** / question-time-horizon difference.
5. Crossover analyzed as independent groups → **methodological diversity/error**, potentially producing apparent statistical heterogeneity.
6. Laboratory versus field outcome method → can be both **clinical/contextual** and **methodological/measurement diversity** depending what is measured.

Strong answer explicitly says clinical/methodological diversity can generate statistical heterogeneity but the categories are not identical.

## C3 — 10 pontos

### 1. I²=0 proves identical studies

False. Low/zero observed statistical inconsistency does not erase clinical/methodological diversity and can arise with limited information.

### 2. I²=20% means 20% of studies are heterogeneous

False. I² concerns variability in effect estimates attributable to heterogeneity versus sampling error in the statistical framework; it does not count studies.

### 3. I²=85% automatically invalidates meta-analysis

False. High heterogeneity requires investigation and cautious interpretation; pooling may or may not remain useful depending on question, direction/magnitude, diversity and target of the random-effects average.

### 4. I² is quality score

False. It does not measure risk of bias or certainty.

### 5. Contextual interpretation

Correct. With few studies especially, I² may be uncertain. Interpret jointly with individual estimates/CIs, directions, study characteristics, tau²/prediction information when available, and methodological plausibility.

**Critical fails:** low I² = clinical identity; high I² = automatic invalidity.

---

# Parte D — 15 pontos

## D1 — 4 pontos

The sensitivity analysis excluding a study with a known unit-of-analysis error has a clear methodological rationale.

The analysis excluding the three smallest observed effects is outcome-driven unless justified independently; it selectively changes the evidence body based on results.

F0.6 application:

- prespecify important sensitivity analyses when feasible;
- document timing/rationale;
- report material variants rather than only the favorable version;
- classify post hoc analyses appropriately.

## D2 — 5 pontos

Expected critique:

- 12 moderator tests create multiplicity/selection opportunities;
- moderator was chosen after seeing heterogeneity/results;
- only 8 studies gives weak information for moderator estimation;
- study-level characteristics may be correlated/confounded;
- p=0.04 is not a causal mechanism certificate;
- direct interaction/meta-regression estimate + CI, prespecification, plausibility and replication/validation matter.

Best answers mention ecological/study-level inference limitations.

**Critical fail:** p=0.04 proves training status causes heterogeneity.

## D3 — 6 pontos

### Small-study effect

A pattern in which smaller/less precise studies tend to show different effect estimates from larger/more precise studies.

### Possible funnel-asymmetry explanations

Any four of:

- selective non-reporting/publication;
- higher bias in small studies;
- real clinical heterogeneity/effect modification;
- effect-measure/SE artefacts;
- chance;
- methodological differences correlated with study size.

### Why asymmetry ≠ publication-bias proof

Multiple mechanisms can generate asymmetry.

### Why symmetry ≠ no missing evidence

Missing studies/results can exist without a visible/asymmetric pattern; graphical power is limited.

### Five-study funnel plot

With very few studies, visual/statistical asymmetry assessment is weak; common Cochrane guidance treats formal asymmetry tests as generally inappropriate/low-powered below roughly 10 studies.

**Critical fails:** funnel asymmetry = proof; symmetry = proof of absence.

---

# Parte E — 25 pontos

Use **2.5 points per required block**, with partial credit.

## 1. Review process

Strengths visible from the report:

- prespecified protocol/question elements;
- multiple databases;
- trial registry;
- no language restriction;
- search date;
- complete PRISMA reporting.

But these features do not prove:

- complete identification of all eligible evidence;
- correct extraction;
- low study/review bias;
- valid pooling;
- high certainty.

## 2. Compatibility

A–E all use the same stated MD scale and can be considered for a common synthesis **provisionally**, subject to population/timepoint/design differences.

Study F reports SMD on a different questionnaire/construct. `0.60 SMD` cannot be appended as `0.60 MD`.

Direction agreement is not scale compatibility.

## 3. Weights

Inverse-variance weight reflects precision of each effect estimate under the model.

Lower SE → higher weight.

Random effects additionally incorporate between-study variance and often make weights more similar.

Weight does not measure quality/risk of bias.

## 4. Pooled result

`MD +1.4 [0.4,+2.4]`:

- target measure: mean difference on the shared scale;
- direction: favors Intervention X if higher is better;
- magnitude: average estimate +1.4 units;
- precision: pooled CI +0.4 to +2.4 for the average under the model;
- cannot be interpreted as universal effect for every athlete/context;
- practical importance still requires a justified threshold/context.

Do not award full credit for “significant therefore works.”

## 5. Heterogeneity

`I²=87%` indicates substantial observed inconsistency relative to sampling variation in this synthesis, but:

- does not automatically invalidate pooling;
- cannot be dismissed because random effects was used;
- requires clinical/methodological explanation and may make the pooled average insufficient as a summary.

## 6. Clinical/methodological alternatives

At least two plausible explanations, e.g.:

- recreational/trained/elite population differences;
- intervention duration;
- measurement setting;
- outcome implementation differences;
- risk-of-bias/design differences;
- correlated study characteristics.

Strong answer notices elite status and measurement setting are nearly collinear, so attributing variation to elite status alone is weak.

## 7. Subgroup/meta-regression

Problems:

- moderators largely post hoc;
- multiple tests;
- few studies;
- collinearity;
- p=0.04 alone does not prove effect modification or cause;
- planned trained/recreational subgroup has stronger design status than newly invented elite/setting stories, but still requires cautious interaction interpretation.

## 8. Missing evidence

Five studies are too few for strong funnel-plot inference.

Apparent symmetry does not prove absence of publication/non-reporting bias.

Need broader evidence: search completeness, registries/protocols, known missing results, study/result availability and other sensitivity checks.

## 9. PRISMA

Complete PRISMA reporting improves transparency, not methodological validity, risk-of-bias status or certainty.

Formal certainty/risk-of-bias synthesis remains F0.8.

## 10. Pooling decision + calibrated conclusion

Defensible answers may differ.

A strong answer may say:

- show A–E individually;
- optionally present the prespecified random-effects pooled MD because they share scale/question enough for a summary;
- prominently state substantial heterogeneity and that the pooled mean may not generalize across contexts;
- do not add F directly without a defensible common effect transformation/construct decision;
- present prespecified and post hoc moderator analyses separately;
- do not claim elite causality;
- consider sensitivity/narrative stratification if measurement/population differences make a single average misleading.

Example calibrated conclusion:

> Across the five studies using the common score, the random-effects model estimates an average MD of about +1.4 units (95% CI +0.4 to +2.4), but study-specific effects vary markedly and the pooled mean should not be treated as a universal athlete effect. Important population, duration and measurement differences may contribute to the heterogeneity. The post hoc elite-status interaction is hypothesis-generating rather than a proven explanation, and the five-study funnel plot cannot establish absence of missing evidence. Study F requires a separate or methodologically justified harmonized synthesis rather than direct numeric pooling with MDs.

---

# Critical-fail enforcement

Block progression regardless of score for any of these:

1. pooled estimate treated as automatically true/superior;
2. low I² treated as proof of clinical/methodological identity;
3. high I² treated as automatic invalidation;
4. PRISMA compliance treated as low risk/high quality certification;
5. incompatible effect measures/scales pooled directly by sign;
6. random effects treated as eliminating heterogeneity;
7. statistical weight treated as quality;
8. subgroup significance-label comparison used as interaction evidence;
9. post hoc subgroup/meta-regression treated as proven explanation;
10. funnel symmetry/asymmetry treated as diagnostic proof;
11. pooled estimate interpreted without magnitude/CI/context;
12. clearly outcome-driven sensitivity analysis relabeled as prespecified confirmation.

---

# Scoring summary

| Part | Points |
|---|---:|
| A — review workflow/reporting | 15 |
| B — compatibility/weights/models | 20 |
| C — forest plot/heterogeneity | 25 |
| D — sensitivity/subgroup/missing evidence | 15 |
| E — integrated performance task | 25 |
| **Total** | **100** |

The local gate applies only after an actual independent learner attempt. Production of this key changes no learner state.
