# F0.6 — Production QA Report

**Unit:** `F0.6 — Power, Type I/II error, multiplicity and analytical flexibility`

**Reviewed:** `2026-09-09`

**Production decision:** `APPROVED`

This QA records curriculum production only. It does **not** record learner study/performance and changes no mastery state.

---

## 1. Scope gate — PASS

Required by `COURSE_MAP.md` / `F0-A12`:

- Type I error in repeated-use/decision-rule terms — covered;
- alpha — covered with probability-reversal protection;
- Type II error — covered as effect-specific;
- beta — covered as conditional on effect/design/assumptions;
- power = `1−beta` — covered;
- power as pre-study conditional probability — central teaching point;
- power not posterior probability of H1 — explicit critical fail;
- `1−power` not posterior false-negative probability — explicit critical fail;
- power curve intuition — P1 covered;
- power versus precision — explicitly separated;
- post hoc/observed power — covered and rejected as a result-interpretation tool;
- sample-size justification — covered;
- smallest effect of interest/planning effect — covered;
- multiplicity — endpoints/timepoints/subgroups/models/stopping choices covered;
- family of hypotheses — explicitly defined;
- family-wise false-positive risk — conceptual + numerical illustration;
- endpoint hierarchy/gatekeeping — covered conceptually;
- Bonferroni — single simple illustration, not exhaustive catalog;
- secondary outcomes — covered;
- subgroup analyses — covered with interaction safeguard;
- researcher degrees of freedom / analytical flexibility — central section;
- trial registration — covered;
- preregistration — covered;
- protocol — covered;
- SAP — covered;
- timing/versioning/deviations — covered;
- confirmatory versus exploratory — explicitly separated;
- preregistration does not guarantee low bias — explicit critical fail;
- F0.5 magnitude/CI interpretation preserved — integrated throughout;
- performance task audits multiple outcomes/timepoints/subgroups/models and reconstructs claims/family/paths/prespecification;
- full meta-analysis/heterogeneity — deferred to F0.7.

No required element is missing.

---

## 2. Current external source recheck — PASS

Verification date: `2026-09-09`.

### `F0-S01` — CONSORT 2025

Current BMJ statement and explanation/elaboration rechecked.

Verified:

- CONSORT 2025 remains the current general statement;
- published 14 April 2025;
- 30-item checklist;
- open-science section includes trial registration, protocol/SAP access, data/code sharing and funding/conflicts;
- explanation/elaboration explicitly states protocol helps expose prespecified methods and undeclared post hoc changes/selective outcome reporting;
- it asks authors to make protocol/SAP accessible and document changes with rationale/timing;
- reports should clarify prespecified versus post hoc analyses.

Instructional use:

- audit trail;
- registration/protocol/SAP distinction;
- prespecification/deviation transparency.

Limitation preserved:

- CONSORT is a reporting guideline, not a risk-of-bias score and not proof that the prespecified analysis was correct.

### `F0-S08` — ASA Statement on p-values

Official ASA PDF rechecked directly.

All six principles remain available and current, including:

- p-values indicate incompatibility with a specified statistical model;
- they do not provide `P(H|data)`;
- conclusions should not depend only on threshold crossing;
- proper inference requires full reporting/transparency;
- p-value/significance does not measure effect size/importance;
- p-value alone is not a sufficient evidence summary.

F0.6 uses principles 3–4 especially for multiplicity/selective analysis while preserving all F0.5 safeguards.

### `F0-S09` — ASA Task Force 2021

Current ASA-hosted page remains available.

Verified teaching points:

- properly applied p-values/significance tests remain useful statistical tools;
- uncertainty, variability, multiplicity and replicability must be considered;
- no single uncertainty measure serves every purpose.

F0.6 uses this source to prevent both ritual thresholding and the false overcorrection that p-values must be abandoned categorically.

### `F0-S10` — FDA Multiple Endpoints Guidance

Current FDA page rechecked.

Status:

- Final Guidance;
- October 2022;
- no newer replacement found on the current FDA guidance page.

Verified teaching points:

- multiple endpoints can increase chance of false conclusions if multiplicity is not appropriately addressed;
- guidance discusses grouping/ordering endpoints and statistical methods to manage multiplicity;
- purpose is control of erroneous drug-effect conclusions in regulatory confirmatory contexts.

Limitation preserved:

- regulatory drug/biologic-trial scope is not generalized as a universal legal requirement for sports/exercise research; mathematical/inferential principles are transferred cautiously.

### `F0-S13` — Lakens 2022

Current UCP/Collabra article rechecked.

Verified:

- six broad sample-size justification approaches;
- sample size should follow inferential goals;
- a-priori power and desired accuracy are distinct justifications;
- smallest effects of interest can inform sample-size decisions;
- planning should occur before data collection rather than inventing a rationale after a nonsignificant result.

F0.6 uses these concepts without implying all studies require one universal power target.

### `F0-S28` — Greenland et al. 2016

Current PMC record remains available.

Instructional use:

- probability-reversal safeguards for p-values/power;
- power and interval claims remain conditional on models/assumptions;
- observed results should not be converted into posterior claims by frequentist error rates.

### `F0-S29` — Heinsberg & Weeks 2022

New source used and verified:

- Heinsberg LW, Weeks DE. *Post hoc Power is Not Informative*. Genetic Epidemiology. 2022;46(7):390-394. doi:10.1002/gepi.22464;
- PubMed/PMC/Wiley records confirm publication details;
- article provides simulation/heuristic explanation of why observed/post hoc power calculated from the observed effect is misleading/redundant for interpreting already-observed results;
- recommends interpreting estimates/CIs/design limitations instead of using post hoc power to explain nonsignificance.

Limitations:

- focused methodological commentary/simulation rather than a complete power-analysis text;
- F0.6 uses it only for the observed-power misuse it directly addresses.

---

## 3. CONTENT_QA — PASS

### Type I / alpha

Verified:

- Type I error is false rejection under the relevant null/model condition;
- alpha is a repeated-use property/nominal rate of the decision rule under assumptions;
- alpha is not posterior probability that H0 is true/false.

### Type II / beta / power

Verified:

- Type II error is framed relative to a specified alternative/effect;
- beta changes with effect size and design assumptions;
- power=`1−beta`;
- power is defined before observing data as rejection probability under a specified effect/design/model;
- no statement equates power with probability H1 is true.

### Power curve

Verified:

- power is effect-dependent;
- “80% power” without effect/assumptions is identified as incomplete.

### Power determinants

Directionality checked:

- larger n → generally greater power;
- larger true effect → greater power;
- lower residual variability → greater power;
- stricter alpha at fixed n/effect → lower power.

All are qualified as holding other design components comparable.

### Power versus precision

Verified:

- power = pre-study decision-probability object;
- precision = post-study estimate uncertainty visible through SE/CI;
- F0.5 remains the correct framework for interpreting a completed estimate.

### Observed power

Verified:

- no use of observed power as posterior evidence;
- observed power computed with observed effect is identified as redundant/misleading for result interpretation;
- design sensitivity to externally specified effects is distinguished from observed-effect power.

### Sample-size justification

Verified:

- a-priori power and desired precision are different design goals;
- near-census/resource constraints can also be legitimate transparent justifications;
- SESOI/planning effect must be justified independently of a favorable observed result.

### Multiplicity

Verified:

- family concept is claim/decision dependent;
- multiplicity sources include outcomes, timepoints, subgroups, models and stopping/data-dependent analysis decisions;
- no claim says all p-values in a paper automatically belong to one family;
- no claim permits artificial fragmentation to evade multiplicity.

### FWER illustrative calculation

Formula is explicitly restricted to:

- independent tests;
- all relevant nulls true;
- identical alpha .05.

Rechecked values:

- m=3 → `1−.95^3 = 14.26%`;
- m=5 → `22.62%`;
- m=10 → `40.13%`;
- m=20 → `64.15%`.

The lesson explicitly states these are not universal numbers for correlated real-world outcomes.

### Adjustment/hierarchy

Verified:

- single primary/hierarchy/alpha allocation/adjusted outputs/exploratory labeling are presented as conceptual strategies;
- Bonferroni `.05/5=.01` arithmetic is correct;
- no claim that Bonferroni is universally optimal.

### Subgroups

Verified:

- `significant in A / not significant in B` is not equated with a subgroup interaction;
- direct interaction evaluation is required.

### Prespecification

Verified:

- trial registration, preregistration, protocol and SAP are distinct;
- timing/versioning/rationale for deviations matter;
- preregistration improves transparency but does not guarantee low risk of bias or valid design.

### Confirmatory/exploratory

Verified:

- exploratory analyses remain scientifically useful;
- undisclosed relabeling of post hoc discovery as prespecified confirmation is the target error.

---

## 4. EVIDENCE_QA — PASS

- power/error-rate claims use statistical/methodological sources;
- multiplicity claims use FDA guidance plus ASA principles;
- prespecification/transparency claims use current CONSORT 2025;
- sample-size justification uses Lakens 2022;
- observed-power critique uses a direct source dedicated to that problem;
- no synthetic sports/nutrition example is treated as empirical intervention evidence;
- no reporting guideline is converted into causal validity or risk-of-bias score;
- no claim that preregistration guarantees validity;
- no claim that high power repairs confounding, measurement bias or selection bias;
- no claim that a nonsignificant result becomes a false negative because of low calculated power.

No cherry-picking issue applies to a treatment-effect conclusion because F0.6 is methodological.

---

## 5. PEDAGOGICAL_QA — PASS

### P2 integrity

F0.6 learner validation requires F0.4 + F0.5.

The lesson explicitly reconnects:

- F0.4 sampling variation/SE/n;
- F0.5 estimates/CI/p-values/practical thresholds.

It does not reteach those modules as formula lists.

### Progression

The lesson follows:

`decision rule → Type I/alpha → Type II/beta → power → power curve → determinants → precision → observed-power misuse → sample-size goals → multiplicity → family/FWER → sources of multiplicity → control concepts → subgroups → analytical flexibility → registration/protocol/SAP → confirmatory/exploratory → integrated audit`.

### P1 bridges

- probability complement explicitly taught;
- FWER calculation worked;
- power-curve interpretation taught conceptually.

### Anti-memorization

Assessment requires:

- repairing probability reversals;
- comparing precision and power;
- interpreting post hoc power misuse;
- sample-size strategy selection;
- FWER calculation;
- defining a hypothesis family;
- evaluating subgroup inference;
- distinguishing registration/protocol/SAP;
- auditing a many-analysis synthetic study.

---

## 6. MASTERY_QA — PASS

Assessment mapping:

- `K1`: alpha/beta/power/family definitions;
- `K3`: power vs precision; family vs path multiplicity; confirmatory vs exploratory;
- `K4`: interpret planning assumptions and observed results;
- `K5`: predict power/multiplicity consequences;
- `K6`: complement/FWER calculation and sample-size reasoning;
- `K7`: integrate F0.4/F0.5 with transparency/multiplicity;
- `K8`: identify post hoc power, probability reversal and selective-analysis limits.

Local gate:

`>=80/100 + no critical fail`.

This gate can alter learner state only after actual observed responses.

Critical fails are explicit and structurally aligned with F0-A12.

---

## 7. Performance-task QA — PASS

Synthetic audit contains:

- prespecified primary + secondaries;
- target power/effect;
- primary estimate/CI/p-value;
- 20 outcomes × 4 timepoints = 80 main comparisons;
- 6 subgroup definitions × 20 outcomes at week12 = up to 120 interaction analyses;
- multiple covariate models;
- selected favorable p-values;
- incomplete reporting;
- observed-power misuse;
- missing SAP link.

Required response reconstructs:

- target claims;
- decision rule;
- power assumptions;
- effective family;
- analytical paths;
- prespecification evidence;
- multiplicity control;
- estimate/CI interpretation;
- confirmatory/exploratory status;
- transparent conclusion.

Important nuance preserved:

- alternative models are not mechanically counted as independent scientific hypotheses; they are analytical paths that can still create selection opportunities.

---

## 8. F0.6 → F0.7 boundary — PASS

F0.6 does not teach full:

- fixed/random-effects meta-analysis;
- inverse-variance pooling;
- I²;
- heterogeneity modeling;
- forest-plot synthesis;
- publication-bias diagnostics;
- meta-regression.

These remain F0.7.

---

## 9. Public repository / privacy / copyright — PASS

- no learner health/personal data;
- no fabricated performance;
- all applied examples are synthetic;
- no third-party PDF/full article is committed;
- only project-authored Markdown, references and links are stored;
- new source is cited/linked, not copied.

---

## 10. Production/learning separation — PASS

After F0-A12 production:

- F0.1 learner state remains pending;
- F0.2 remains pending;
- F0.3 remains pending;
- F0.4 remains pending;
- F0.4 quantitative diagnostic remains `UNOBSERVED`;
- F0.5 remains pending;
- F0.6 remains `UNSEEN`.

No mastery state is changed from curriculum production.

---

## 11. Final gate

> Can a learner with F0.4/F0.5 prerequisites define Type I/II error and power without probability reversals, plan/critique sample size relative to inferential goals, distinguish power from observed precision, reject observed-power misuse, recognize and reason about multiplicity/analytical flexibility, audit prespecification evidence and separate confirmatory from exploratory claims without needing F0.7 meta-analysis machinery?

**Decision:** yes.

**Production state:** `APPROVED`.