# F0.6 — Gabarito comentado

**Purpose:** scoring/reference after an independent attempt.

**Do not use this file during the first attempt.**

**Total:** 100 pontos.

**Gate:** `>=80/100` + nenhum critical fail.

Partial credit is allowed when reasoning is directionally correct but one calculation/detail is incomplete. Probability reversals and structural misconceptions listed as critical fails block progression regardless of total score.

---

# Parte A — 20 pontos

## A1 — 8 pontos

### Type I error

Expected:

> Rejeitar H0 em uma repetição em que o null/model condition relevante é verdadeiro.

### Alpha

Expected:

> Taxa/probabilidade nominal de Type I rejection do procedimento sob H0 e suas assumptions em repeated sampling.

Do **not** award full credit for “probability H0 is false/true.”

### Type II error

Expected:

> Não rejeitar H0 quando um efeito alternativo verdadeiro especificado está presente, sob o design/model considered.

### Beta

Expected:

> Probabilidade desse Type II outcome para um efeito/assumptions específicos.

Must recognize beta varies with effect size and design.

### Power

Expected:

`power = 1 − beta`

and conceptually:

> probability, before observing data, that the specified test/procedure rejects H0 across hypothetical repetitions when a specified true effect and design assumptions hold.

### Repair statements

`alpha=0.05` repair:

> It is a repeated-use false-rejection rate under H0/model assumptions, not `P(H0|data)`.

`80% power` repair:

> It is not `P(H1 true)`; it is the rejection probability conditional on a specified true effect/design/model.

**Scoring suggestion:**

- Type I + alpha: 2;
- Type II + beta: 2;
- power definition: 2;
- two repaired statements: 2.

**Critical fail:** posterior-probability interpretation of alpha/power.

## A2 — 5 pontos

Order:

`delta 0.2 < delta 1.0 < delta 2.0` in expected power, all else equal.

Why “80% power” is incomplete:

- power depends on assumed true effect;
- also depends on n, variability, alpha/test/design and other assumptions.

Full credit requires effect-specific reasoning rather than “bigger effect easier” alone.

## A3 — 7 pontos

1. n increases → power typically increases, because SE/sampling uncertainty falls.
2. alpha `0.05→0.01` → power typically decreases at fixed n/effect, because rejection criterion becomes more stringent.
3. larger true effect → power increases.
4. larger residual variability → power decreases.

Accept qualifications that dependencies can be design-specific.

---

# Parte B — 20 pontos

## B1 — 6 pontos

1. **Study A** is more precise: CI width `1.0` versus `6.8`.
2. Study A is more informative for SESOI `+2.0`: its upper CI `+0.9` excludes benefit `>=+2.0` under the model/assumptions. Study B remains compatible with benefit above +2 and substantial harm.
3. Post-study interpretation should use observed estimate/CI relative to SESOI. Prospective power describes design performance under assumed effects; it is not the direct uncertainty of the observed estimate.

Do not award full credit if the learner uses “nonsignificant = no effect.”

## B2 — 7 pontos

Expected four-step critique:

1. **Observed power error:** plugging observed `MD=+1.1` into a power formula after seeing the data is not an independent explanation; in common tests it is largely/redundantly tied to the observed estimate/p-value.
2. `27%` is not `P(false negative | data)` and not probability a true effect exists.
3. CI `−1.5 to +3.7`, with SESOI `+2.0`, remains compatible with harm/trivial effects and benefits above the threshold; therefore the result is imprecise for practical interpretation.
4. Better conclusion: the point estimate is positive but uncertainty is wide; the data do not distinguish reliably among trivial, harmful and practically relevant beneficial effects. Design/bias should also be considered.

**Critical fail:** “27% observed power proves low power caused the result.”

## B3 — 7 pontos

### Scenario 1

Best: `desired accuracy/precision`.

Rationale: objective is CI width relative to a practical threshold.

### Scenario 2

Best: `a-priori power`.

Must identify pre-study target effect +2, alpha .05, power .90 and needed variance/design assumptions.

### Scenario 3

Best: `near-census/population` justification.

All 48 eligible units are invited; power can still be reported as a design property if useful, but the reason for n is finite population/access rather than a magic target.

Accept resource-constraint nuance only if learner explains that it is a distinct justification and discusses resulting informativeness.

---

# Parte C — 20 pontos

## C1 — 6 pontos

Formula:

`P(>=1 FP) = 1 − 0.95^m`.

### m=5

`1 − 0.95^5 = 1 − 0.7737809375 = 0.2262190625`

≈ **22.6%**.

### m=20

`1 − 0.95^20 ≈ 1 − 0.3584859224 = 0.6415140776`

≈ **64.2%**.

Interpretation:

> Under the illustrative assumptions of independent tests and all relevant nulls true, this is the probability of at least one Type I rejection among the m tests.

Not:

> “probability the paper is wrong.”

Why not universal:

- outcomes/timepoints may be correlated;
- hypothesis family and procedure matter;
- adjustment/hierarchy can change error behavior.

## C2 — 7 pontos

1. The **four key secondary claims** clearly need a multiplicity strategy if each is intended as an additional confirmatory efficacy claim at nominal .05.
2. The 30 biomarker-time analyses do not necessarily belong to the same **confirmatory** family if explicitly exploratory and not used as confirmatory claims. They still create selective-discovery/multiplicity context and must be transparently reported/labeled.
3. Per-test alpha .05 does not control the probability of at least one false rejection across the confirmatory family.

Strong answers mention that the one primary claim can have its own planned decision rule; family definition follows claims/design, not table layout.

## C3 — 7 pontos

### Single primary endpoint

Function: concentrates confirmatory error budget/claim on one prespecified target.

Limitation: may not capture all scientifically important dimensions; does not make the endpoint valid.

### Hierarchy/gatekeeping

Function: orders claims and allows later claims only when earlier criteria are satisfied under a defined procedure.

Limitation: ordering must be prespecified/justified; later useful findings may remain exploratory if gate fails.

### Bonferroni

Function: simple alpha allocation, e.g. .05/5=.01 per test, controlling familywise Type I error under broad dependence conditions.

Limitation: can be conservative; not universally optimal.

### Exploratory classification

Function: avoids pretending every analysis is confirmatory; preserves hypothesis-generation value with calibrated claims.

Limitation: does not “erase” multiplicity or prove findings; replication/validation is needed for stronger claims.

---

# Parte D — 15 pontos

## D1 — 5 pontos

1. No. The listed analyses may represent alternative analytical paths for the same scientific effect/claim rather than six independent hypotheses.
2. Main problem: data-driven model/outlier/path selection followed by reporting only the smallest p-value changes the inferential process and creates selection/analytical-flexibility bias/error inflation.
3. Needed SAP/protocol information:
   - prespecified outcome definition;
   - primary model;
   - covariates;
   - outlier rule;
   - scale/change-score choice;
   - sensitivity analyses;
   - timing/version/deviations.

## D2 — 4 pontos

Correct reasoning:

- “significant in A, nonsignificant in B” does not establish A differs from B;
- evaluate an interaction/treatment-by-subgroup contrast directly;
- interpret interaction estimate + CI, multiplicity, prespecification and plausibility.

**Critical fail:** concluding sex interaction solely from the two subgroup p-values.

## D3 — 6 pontos

### Trial registration

Public summary record with key design/outcome/timing information; often less detailed.

### Protocol

Broader document describing planned design/methods.

### SAP

Detailed analysis methods: populations, models, outcomes, covariates, missing data, multiplicity, subgroups, sensitivity analyses, etc.

### Timing/versioning

Needed to know what existed before data/results could influence decisions and to audit changes.

### Changes

Changes can be scientifically legitimate. They should be timestamped, justified and reported; changing a plan is not automatically misconduct.

### Preregistration limitation

It increases transparency/auditability but cannot guarantee:

- good measurement;
- valid causal design;
- correct analysis;
- low missingness;
- relevance/applicability;
- low risk of all biases.

**Critical fail:** `preregistered = valid/low bias`.

---

# Parte E — 25 pontos

Use 2.5 points per required block, with partial credit.

## 1. Target confirmatory claims

Expected:

- documented primary: time-trial performance at week 12;
- three secondaries were planned, but no multiplicity strategy is documented for confirmatory secondary claims;
- do not automatically promote them to independently confirmatory at .05.

## 2. Decision rule

`alpha=.05` is the planned repeated-use Type I threshold/rate for the specified procedure under null assumptions.

It is not:

- 5% chance H0 true;
- 5% false-paper probability.

## 3. Planning power

`80% for +2.0%` means:

> if the true effect were +2.0% and planning assumptions/design were correct, the prespecified test would reject H0 in about 80% of hypothetical repetitions.

It does not mean:

- 80% probability the true effect is +2%;
- 80% probability this study succeeds;
- 20% posterior false-negative probability.

## 4. Primary estimate/CI

`+0.6% [−0.5,+1.7]`:

- point estimate favors A by .6%;
- interval includes small harm/no effect and modest benefit;
- interval does not reach the +2.0% **planning effect**, but planning effect is not automatically identical to a valid practical threshold unless specified/justified;
- p=.28 does not prove no effect;
- observed power is unnecessary for interpretation.

Strong answer notes that if +2.0% were also the prespecified smallest important benefit, this CI would exclude benefit >=+2 under the model, but the prompt only establishes it as a planning effect.

## 5. Effective family

Expected:

- 80 outcome-time comparisons create substantial multiplicity/discovery opportunities;
- up to 120 subgroup interaction analyses add further hypothesis multiplicity;
- multiple covariate models add analytical-path multiplicity;
- do not mechanically call all model variants independent hypotheses;
- family must be defined relative to intended claims.

## 6. Subgroups

`p=.03` alone does not prove a true subgroup-specific effect.

Need:

- interaction estimate/test;
- CI;
- prespecification;
- multiplicity context;
- full subgroup family;
- plausibility/replication.

## 7. Prespecification evidence

Registry supports that primary week-12 time trial and three secondaries were listed before recruitment, assuming timestamp is verified.

Missing SAP means the reader cannot fully audit:

- exact models;
- covariates;
- interaction analyses;
- missing-data rules;
- multiplicity plan;
- analysis population;
- deviations.

Important: absence of linked SAP does **not** prove no SAP existed.

## 8. Confirmatory vs exploratory

Based only on given evidence:

- mood/week8 `p=.008`: exploratory/post hoc;
- high-fitness recovery subgroup `p=.03`: exploratory/post hoc;
- cannot call either confirmatory without documentation of prespecification and relevant multiplicity control.

## 9. Transparent reporting plan

Any six well-explained items, e.g.:

1. report primary regardless of significance;
2. provide registry link/timestamp;
3. protocol link/version;
4. SAP link/version/timing;
5. distinguish prespecified vs post hoc;
6. describe full hypothesis family;
7. report all outcomes/timepoints or accessible complete results;
8. explain multiplicity strategy/hierarchy;
9. report effect estimates + CIs, not p only;
10. identify model-selection deviations;
11. report subgroup interactions and full set;
12. label exploratory findings appropriately.

## 10. Calibrated conclusion

Model answer:

> The preregistered primary estimate was +0.6% with a 95% CI from −0.5% to +1.7%, so the observed data are relatively precise around effects smaller than the +2.0% effect used in planning, although that planning effect should not be assumed to be the practical threshold unless justified. The primary p=.28 does not prove absence of effect and post hoc observed power does not clarify the observed result. The many outcome-time, subgroup and model-selection opportunities create substantial multiplicity and analytical-flexibility concerns. Because the highlighted mood/week8 and high-fitness subgroup findings are not documented here as prespecified with appropriate multiplicity control, they should be presented as exploratory. Trial registration helps establish the planned primary outcome, but lack of accessible SAP leaves important analytical choices unauditable and preregistration itself does not guarantee low risk of bias.

Alternative wording is acceptable if all required boundaries are preserved.

---

# Critical-fail audit

Block progression if the response contains any uncorrected structural claim:

1. `power = P(H1|data)` or probability H1 true;
2. `1−power = probability this nonsignificant result is a false negative`;
3. observed power from observed effect used as proof/explanation of the result;
4. many nominal .05 tests treated as independent confirmatory proof without family reasoning;
5. preregistration treated as guarantee of low risk of bias/correct design;
6. nonsignificant primary treated as proof of zero effect;
7. subgroup significance comparison used as proof of interaction;
8. estimate/CI ignored in post-study interpretation.

If one appears but the learner explicitly identifies and repairs it later, do not automatically count as critical fail; score the final demonstrated reasoning.

---

# Interpretation of score

- `90–100` + no critical fail: strong local performance; eligible for progression evidence but not automatic `MASTERED`.
- `80–89` + no critical fail: local gate passed; errors should be logged/retested if recurring.
- `<80` or any critical fail: do not progress F0.6 learner state; route remediation to earliest broken prerequisite/concept.

Possible routing:

- SD/SE/CI confusion → F0.4/F0.5;
- p-value probability reversal → F0.5;
- power probability reversal → F0.6 sections 3–9;
- multiplicity failure → F0.6 sections 13–23;
- prespecification-as-guarantee → F0.3 + F0.6 sections 24–27.