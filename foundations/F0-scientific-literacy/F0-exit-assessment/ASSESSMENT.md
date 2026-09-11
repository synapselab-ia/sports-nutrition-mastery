# F0 Exit Assessment v1 — Scientific Literacy and Quantitative Reasoning

**Production state:** `READY_FOR_ADMINISTRATION`
**Assessment version:** `1`
**Total:** `100 points`
**Learner-state effect at authoring:** none

This is the cumulative exit assessment for F0. It tests transfer across F0.1–F0.10 rather than recall of isolated definitions.

## Administration rules

- Complete Sections A, B, C and E without consulting module answer keys.
- For Section D, use the assigned full paper, its public trial-registry record and materials directly linked from those sources. Do not use this assessment's `ANSWER_KEY.md`.
- If information is not reported or cannot be verified, write `NOT REPORTED`, `UNCLEAR` or equivalent. Do not invent missing information.
- Show reasoning where requested. A label without justification may receive little or no credit.
- Calculators are allowed. External generative assistance is not part of the intended independent administration.

## Exit gate

Pass requires all of the following:

1. total score `>=85/100`;
2. every section scores at least 70% of its available points;
3. no `CRITICAL_FAIL` occurs;
4. Section D demonstrates a defensible chain from question to conclusion;
5. Section E does not increase certainty when simplifying language.

`75–84` with no critical fail = `NEAR_PASS / TARGETED_REMEDIATION`.

Below `75` = broader remediation mapped to the earliest broken dependency.

A passing first attempt can support `APPLIED`/`INTEGRATED` evidence. It does not by itself establish `MASTERED`.

---

# Section A — Question, design and causal structure — 20 points

## A1. Operationalize a claim — 5 points

A company states:

> **“CarboMax improves 10 km running performance.”**

Turn this slogan into one empirically answerable effect question. Specify:

1. target population;
2. intervention/exposure, including enough operational detail to distinguish it from a brand label;
3. comparator;
4. outcome and measurement window;
5. effect/contrast of interest;
6. one plausible result that would count against the claim.

You may choose reasonable details, but they must be internally coherent.

---

## A2. Identify design and inference boundary — 7 points

For each study, identify the design, state the strongest defensible inference, and state one inference the design cannot establish by itself.

### Study A

Eighteen trained cyclists receive beverage X and matched placebo in randomized counterbalanced order, separated by a 7-day washout. They complete the same 20 km time trial two hours after each condition. Participants and outcome assessors are blinded.

### Study B

Three hundred recreational runners report habitual caffeine intake at baseline and are followed for 12 months for running injuries. Researchers adjust for age, sex, weekly running distance and prior injury.

### Study C

Six hundred gym users complete one survey about habitual protein intake and have maximal isometric strength measured during the same visit. Higher reported protein intake is correlated with greater strength.

Then answer one synthesis question:

> Why does “randomized” strengthen the causal architecture of Study A without making every possible causal conclusion automatically valid?

---

## A3. Causal structure and adjustment — 8 points

Consider an observational study of habitual high-carbohydrate strategy `X` and 10 km performance `Y`.

Assume the following causal structure:

```text
T → X
T → Y
X → G → Y
X → S ← U → Y
```

where:

- `T` = training volume;
- `G` = pre-race muscle glycogen availability;
- `S` = gastrointestinal-symptom status used as a stratification variable;
- `U` = underlying gastrointestinal susceptibility.

Answer:

1. Classify the role of `T`, `G` and `S` for the total effect of `X` on `Y`.
2. Explain why adjusting for `T` can be defensible.
3. Explain why adjusting for `G` changes the estimand if the target is the total effect.
4. Explain how conditioning on `S` can introduce bias through the path involving `U`.
5. State one reasonable adjustment strategy for estimating the total effect under this simplified graph.

Do not merely name “confounder/mediator/collider”; explain the path logic.

---

# Section B — Quantitative interpretation — 25 points

## B1. Descriptive statistics, uncertainty and graph reading — 5 points

### B1a — Distribution

Recovery time in hours for 12 athletes is:

`7, 8, 8, 9, 9, 9, 10, 10, 11, 12, 13, 46`

Would you summarize the center/spread primarily with mean/SD or median/IQR? Why?

### B1b — SD versus SE

Two samples have similar SDs, but Sample 2 is four times larger than Sample 1. Under the simple independent-sample intuition, what happens approximately to the SE of the mean in Sample 2? What does **not** necessarily happen to the SD of individual observations?

### B1c — Misleading graph

A bar graph compares mean VO2peak values of `58.8` and `59.6 mL/kg/min`, but its y-axis begins at `58.0` rather than zero. What visual interpretation error can this induce, and what numerical information should be reported before judging importance?

### B1d — Absolute versus relative change

A symptom occurs in 10% of a control group and 15% of an intervention group. State:

- absolute risk difference in percentage points;
- relative increase compared with control.

---

## B2. Estimate + CI + practical threshold — 8 points

In a randomized performance trial, lower time is better.

The estimated between-group mean difference is:

`MD = -18 seconds; 95% CI [-38, +2]`

Before seeing the data, the investigators defined a benefit of at least `25 seconds` as practically important. A practically important harm would be `+25 seconds` or worse.

Interpret the result in the following order:

1. direction;
2. point-estimate magnitude;
3. precision;
4. whether the interval is compatible with practically important benefit;
5. whether it is compatible with trivial/small effects;
6. whether it is compatible with practically important harm;
7. what crossing `0` does and does not establish;
8. the strongest short conclusion you would communicate.

---

## B3. Repair p-value statements — 4 points

For each statement, mark it false or defensible and repair it if false.

### Statement 1

> “p = 0.03 means there is a 3% probability that the null hypothesis is true.”

### Statement 2

> “p = 0.12 proves there is no meaningful treatment effect.”

A response that only says “false” earns no credit.

---

## B4. Power, precision and information — 4 points

The target effect is the same in two randomized trials, and a benefit of `25 seconds` or more is practically important.

- **Study A:** `n=24`, MD `-18 s`, 95% CI `[-55,+19]`.
- **Study B:** `n=160`, MD `-8 s`, 95% CI `[-18,+2]`.

Neither study reports a statistically significant superiority result.

Which study is more informative for deciding whether a benefit of at least 25 seconds remains plausible? Explain using precision and the threshold. Then explain why calculating “observed power” from each observed effect is not needed to interpret the completed studies.

---

## B5. Multiplicity and analytical flexibility — 4 points

A 12-week trial measures six performance/recovery outcomes at weeks 4, 8 and 12, reports analyses in men and women separately, and shows both unadjusted and covariate-adjusted models. The paper highlights one subgroup result at week 8 with `p=0.03`. The registry lists one primary outcome at week 12 but gives no public statistical analysis plan.

Answer:

1. What creates the effective family of analytical opportunities here?
2. Can the highlighted week-8 subgroup result be treated as prospectively confirmatory from the information given? Why or why not?
3. What timestamped material would you seek to classify the analysis more confidently?

---

# Section C — Systematic review and certainty — 20 points

## C1. Synthetic forest-plot interpretation — 8 points

A systematic review evaluates Intervention R versus placebo for endurance time-trial performance. All effects are mean differences in **seconds**, where negative values favor Intervention R.

```text
Study                     MD [95% CI]             Weight
A — trained runners       -8  [-22, +6]            25%
B — trained cyclists      -12 [-28, +4]            20%
C — recreational runners  -38 [-60, -16]           15%
D — trained triathletes   +2  [-14, +18]           25%
E — hot-environment study -48 [-79, -17]           15%
---------------------------------------------------------
Random-effects pooled     -17 [-31, -3]           100%
I² = 74%
```

Interpret this forest-plot extract. Address:

1. effect direction and scale;
2. which studies are more versus less precise and how the displayed weights relate conceptually to precision;
3. pooled estimate and its interval;
4. what `I²=74%` signals and what it does **not** mean;
5. at least two plausible clinical/methodological sources of heterogeneity visible from the labels/context;
6. why the pooled number alone cannot decide whether pooling is scientifically useful.

---

## C2. Review-method appraisal — 5 points

A review reports:

> The protocol was registered before searching. Eligible studies were randomized trials in adults undergoing exercise training. The authors searched PubMed and SPORTDiscus through March 2026 and restricted inclusion to English-language full-text journal articles. Trial registries and grey literature were not searched. Two reviewers independently screened titles/abstracts and full texts. One reviewer extracted data and a second reviewer verified the extraction. RoB 2 was used for included-trial results. Random-effects meta-analysis was planned. The article does not state in this methods extract whether the published primary synthesis/outcome hierarchy matches the registered protocol.

Identify:

1. two features that increase auditability/trustworthiness;
2. two features that could contribute to missing evidence or bias in the review process;
3. one issue that is **unclear from the extract** rather than demonstrated to be wrong;
4. why a complete PRISMA checklist would not by itself settle the review's risk of bias or certainty.

---

## C3. Certainty and applicability — 7 points

Target question:

> In **trained adult endurance athletes**, does Intervention S improve a validated performance score after approximately 12 weeks versus placebo? A change of `+0.6` or more is considered practically important.

### Evidence Body A

- seven randomized trials, mostly trained endurance athletes;
- same validated performance construct and 10–14 week follow-up;
- pooled effect `+0.8 [95% CI +0.5,+1.1]`;
- low risk of bias for the main outcome in most information-bearing studies;
- effects broadly consistent;
- no strong supplied signal of missing evidence.

### Evidence Body B

- five self-selected observational cohorts, mostly recreational/untrained adults;
- proxy outcome measured after 2–4 weeks;
- transformed effect `+0.9 [95% CI -0.4,+2.2]`;
- important residual confounding and differential loss to follow-up;
- effects vary substantially across studies.

Compare A and B:

1. Which body deserves greater certainty for the target question and why?
2. Identify the main certainty domains separating them.
3. Compare applicability/indirectness to the target.
4. Explain why the similar point estimates (`+0.8` vs `+0.9`) do not imply similar evidence strength.
5. Explain why even high certainty for this outcome would not automatically dictate a strong recommendation.

---

# Section D — Full-paper critical appraisal — 25 points

## Assigned paper

Jagłowska K, Folwarski M, Chroboczek M, Potrykus M, Kaczmarczyk M, Skonieczna-Żydecka K, Kaczor JJ. **Multistrain Probiotic Supplementation Combined with a Standardized Diet Did Not Significantly Affect Exercise Performance or Inflammatory Responses in Male Endurance Runners: A Randomized Controlled Trial.** *Nutrients*. 2026;18(15):2484. doi:10.3390/nu18152484.

Full text: https://pmc.ncbi.nlm.nih.gov/articles/PMC13468382/

DOI: https://doi.org/10.3390/nu18152484

Trial registry: https://clinicaltrials.gov/study/NCT07411482

### Neutral context box

This paper tests a multistrain probiotic versus placebo during a standardized diet in trained male endurance runners. You are **not** being tested on whether probiotics “should” work mechanistically. You are being tested on whether you can reconstruct what this trial estimated and how strongly its results support the authors' claims.

Use the full paper and registry. Check linked supplementary/open-science materials if they are relevant and accessible. If a detail cannot be verified, say so.

## D1. Question and estimand — 3 points

Reconstruct the primary causal/effect question in PICO/estimand form:

- population;
- intervention;
- comparator;
- primary outcome;
- time horizon;
- model contrast/effect of interest.

State whether the title's broad wording is narrower, equal to or broader than the primary estimand you reconstruct.

## D2. Design and selection — 3 points

Describe:

- randomization/blinding/parallel structure;
- recruitment/sample analyzed;
- what randomization protects against in principle;
- one selection/generalizability limitation that remains.

## D3. Measurement and intervention fidelity — 2 points

Identify two material measurement/fidelity features. At least one must concern how exposure/intervention adherence, training, diet or outcome measurement was operationalized rather than merely naming an instrument.

## D4. Bias, missingness and execution — 4 points

Choose the **primary performance result** and give a result-specific bias appraisal. Discuss at least:

- randomization/allocation information;
- deviations/adherence/co-interventions;
- missing outcome data/analysis population;
- outcome measurement;
- selection of reported result.

Do not convert this into a single numerical “quality score.”

## D5. Analysis, prespecification and multiplicity — 3 points

Reconstruct:

- sample-size justification versus achieved sample;
- primary/secondary outcome structure;
- multiplicity handling;
- what the public registry timing can and cannot establish about prospective prespecification.

If the article claims earlier prespecification in ethics/grant materials, distinguish that claim from what the public registry independently demonstrates.

## D6. Effect estimate and uncertainty — 4 points

For the primary performance outcome:

1. report the model-based between-group effect estimate and 95% CI;
2. distinguish the nominal p-value from the multiplicity-adjusted result;
3. explain what values remain compatible with the CI;
4. explain why neither the nominal result nor the adjusted result should be reduced to a binary truth statement;
5. state what additional threshold/margin information would be needed for a practical-equivalence claim.

## D7. Applicability — 2 points

Compare the study with at least two possible target populations/contexts, including one for which applicability is relatively good and one for which it is materially weaker. Use population, intervention, duration, diet/training context and outcome as appropriate.

## D8. Authors' conclusion — 2 points

Judge whether the authors' final conclusion is proportional to their methods/results. Identify one wording choice you consider appropriately cautious or one phrase that requires qualification, and justify your judgment.

## D9. What the study does not prove — 2 points

State at least three explicit boundaries on inference. At least one must concern mechanism and at least one must concern absence/equivalence or generalization.

A checklist-only Section D response cannot earn more than 60% of the section.

---

# Section E — Communication of uncertainty — 10 points

Use this **synthetic evidence result**; do not import the Section D paper.

Target: trained adult endurance athletes, Intervention T versus placebo, 8–12 weeks, validated 5 km performance time; lower is better.

Evidence body:

- seven direct randomized trials;
- pooled MD `-9 seconds`;
- 95% CI `[-22,+4]`;
- practical-benefit threshold prespecified at `-20 seconds`;
- no major supplied risk-of-bias concern in the information-bearing trials;
- moderate certainty, limited mainly by imprecision around the practical threshold;
- direct applicability to trained endurance athletes is reasonable; applicability to sedentary adults or clinical populations is not established;
- this was not designed as a formal equivalence/non-inferiority evidence package.

Produce both outputs:

### E1. Technical synthesis — maximum ~150 words

Preserve population/context, direction, magnitude, CI, threshold, certainty/major limitation, applicability and what is not established.

### E2. Plain-language synthesis — maximum ~100 words

Remove unnecessary jargon but preserve the **same epistemic content**. The plain-language version must not become more certain than E1.

---

# Critical-fail reminder

Any answer can trigger a `CRITICAL_FAIL` if it demonstrates a structural misconception such as:

- causal certainty from adjusted/significant observational association alone;
- `p>0.05 = no effect` when meaningful effects remain compatible;
- frequentist 95% CI interpreted as 95% posterior probability for the fixed parameter;
- significance = practical importance;
- reporting-checklist completion = low RoB/high quality;
- low I² = clinical/methodological identity;
- obvious multiplicity ignored while asserting confirmation;
- low/very-low certainty converted into a definitive recommendation without justification;
- absence of evidence confused with precise evidence excluding a meaningful effect;
- fabricated information.

Scoring and remediation rules are defined in `ANSWER_KEY.md` and must not be consulted during independent administration.
