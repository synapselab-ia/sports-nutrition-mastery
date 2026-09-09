# F0.6 — Practical NotebookLM Study Guide

**Package version:** `1`
**Module:** `F0.6 — Power, Type I/II error, multiplicity and analytical flexibility`
**Current learner state:** `UNSEEN`
**F0.4 quantitative diagnostic:** `UNOBSERVED`

This guide defines how to build and use the approved NotebookLM corpus for F0.6. Creating the notebook, reading sources or completing these study passes does **not** change learner state. Any transition requires observed performance under the mastery protocol.

## 0. Prerequisite integrity

F0.6 learner validation requires F0.4 + F0.5 as P2.

The repository still records:

- F0.4 learner state: unvalidated;
- F0.4 quantitative diagnostic: `UNOBSERVED`;
- F0.5 learner state: unvalidated;
- F0.6 learner state: `UNSEEN`.

Do not infer mastery from package production or NotebookLM use. For honest learner validation, prerequisite diagnostic/study/assessment evidence must be observed separately.

Keep the F0.4 entry diagnostic outside this notebook.

---

## 1. Create the notebook

Create one NotebookLM notebook named:

`Sports Nutrition Mastery — F0.6 Power, Multiplicity and Analytical Flexibility`

Keep it separate from F0.5.

F0.5 remains the interpretation layer for completed estimates, confidence intervals, p-values and practical thresholds. F0.6 adds repeated-use error rates, prospective power, sample-size rationale, multiplicity, analytical flexibility and prespecification auditing.

Core rule:

> **Planning uses alpha/beta/power under specified effects and assumptions; completed-study interpretation uses estimate + CI + practical threshold; multiplicity and prespecification describe the inferential process, not the truth of a single result.**

---

## 2. Add exactly eight initial sources

### Source 1 — canonical F0.6 lesson — CORE

Repository file:

`foundations/F0-scientific-literacy/F0.6-power-multiplicity-analytical-flexibility/LESSON.md`

Preferred URL:

`https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.6-power-multiplicity-analytical-flexibility/LESSON.md`

Use as the instructional spine for:

- Type I/II error;
- alpha/beta/power;
- power curve intuition;
- power versus precision;
- observed-power misuse;
- sample-size justification;
- family of hypotheses and FWER intuition;
- endpoints/timepoints/subgroups/models/stopping choices;
- endpoint hierarchy and conceptual adjustment strategies;
- subgroup interaction safeguard;
- researcher degrees of freedom;
- trial registration/preregistration/protocol/SAP;
- timing/versioning/deviations;
- confirmatory versus exploratory outputs;
- ten-field integrated audit.

If the raw URL cannot be ingested, upload the canonical Markdown file itself. Do not substitute an AI summary.

### Source 2 — ASA Statement on p-values (2016) — CORE

Add:

`https://www.amstat.org/asa/files/pdfs/P-ValueStatement.pdf`

Use for:

- model-conditional p-value interpretation;
- threshold misuse;
- transparency/full reporting;
- effect magnitude/importance separation;
- selective reporting/p-hacking context.

Required skill: repair false statements without replacing one binary ritual with another.

### Source 3 — FDA Multiple Endpoints Guidance (2022) — CORE

Add:

`https://www.fda.gov/regulatory-information/search-fda-guidance-documents/multiple-endpoints-clinical-trials`

Use for:

- why multiple endpoints can increase false-conclusion risk;
- grouping/ordering endpoint families;
- hierarchy/gatekeeping intuition;
- multiplicity-management concepts.

Do **not** treat FDA regulatory requirements as universal legal requirements for exercise or sports-nutrition studies. Use the source for inferential principles only.

### Source 4 — Lakens 2022 Sample Size Justification — CORE

Add:

`https://online.ucpress.edu/collabra/article/8/1/33267/120491/Sample-Size-Justification`

Use for:

- sample-size justification tied to inferential goals;
- a-priori power;
- desired precision/accuracy;
- smallest effect of interest;
- finite-population/near-census reasoning;
- resource constraints and transparent limitations.

Do not reduce the article to “always use 80% power.”

### Source 5 — Greenland et al. 2016 — SUPPORT

Add:

`https://pmc.ncbi.nlm.nih.gov/articles/PMC4877414/`

Use for:

- probability reversals involving p-values and power;
- repeated-use/conditional interpretations;
- analysis-selection problems;
- why error rates are not posterior probabilities about hypotheses;
- continuity with F0.5 CI/p-value safeguards.

### Source 6 — Heinsberg & Weeks 2022 — SUPPORT

Add:

`https://pmc.ncbi.nlm.nih.gov/articles/PMC9452450/`

Use specifically for:

- why observed/post hoc power calculated from the observed effect is not informative for interpreting a completed study;
- why post-study interpretation should use estimates/CIs and design context;
- why prospective power remains a planning concept.

### Source 7 — CONSORT 2025 — SUPPORT

Add:

`https://www.bmj.com/content/389/bmj-2024-081123`

Use for:

- trial registration;
- protocol/SAP access;
- prespecified versus post hoc analyses;
- reporting important changes after trial commencement;
- audit-trail transparency.

Do not score study quality by checklist completion.

### Source 8 — ASA Task Force 2021 — CONTRAST

Add:

`https://magazine.amstat.org/blog/2021/08/01/task-force-statement-p-value/`

Use to answer:

> Why is the correct lesson neither “p<0.05 decides truth” nor “p-values are useless and should always be banned”?

Target synthesis:

- p-values/significance tests can be useful when properly applied;
- uncertainty, variability, multiplicity and replicability still matter;
- model choice, selective reporting and transparency matter;
- no single statistic replaces scientific reasoning.

---

## 3. Do NOT add these yet

Keep outside the initial notebook:

- F0.6 `EXERCISES.md` — independent assessment;
- F0.6 `ANSWER_KEY.md` — answer leakage;
- F0.6 production `QA_REPORT.md` — metadata;
- F0.4 `ENTRY_DIAGNOSTIC.md` — prerequisite diagnostic must remain uncontaminated;
- full `SOURCE_INDEX.md` — retrieval noise;
- exhaustive multiplicity-correction catalogs;
- software-specific power manuals/calculators as primary teaching sources;
- formal sequential/adaptive trial theory;
- systematic-review/meta-analysis/heterogeneity/I2/publication-bias corpora — F0.7;
- RoB 2/ROBINS-I/GRADE formal corpora — later modules;
- substantive sports-nutrition intervention papers — not needed for this methodological package.

---

# 4. Study sequence

Do not begin with “summarize all sources”. Complete the passes in order.

## Pass 1 — Type I error and alpha without probability reversal

Use canonical lesson + ASA 2016 + Greenland.

Prompt:

> Give me 10 decision-rule scenarios. For each, make me define Type I error and alpha in repeated-use terms. Reject any wording that treats alpha as P(H0 true|data), chance the paper is wrong, or chance the result happened by random chance alone.

Required answer structure:

1. null/model condition;
2. decision rule;
3. Type I event;
4. alpha interpretation;
5. what alpha does **not** mean.

Critical trap:

`alpha=.05` is not a posterior probability about one observed study.

---

## Pass 2 — Type II error, beta and power are effect-specific

Prompt:

> Give me eight prospective study-planning statements. Require me to identify the assumed true effect, n, variability, alpha, design and target power before interpreting the number.

For every case answer:

1. specified effect/alternative;
2. beta meaning;
3. power=`1-beta` meaning;
4. which assumptions make the statement conditional;
5. why power is not P(H1 true).

Do not accept “the study has 80% power” without “for which effect?”

---

## Pass 3 — power-curve intuition

Prompt:

> Hold design and alpha fixed. Vary true effect size, sample size and residual variability one factor at a time. Make me predict the direction of power change before you explain it.

Minimum contrasts:

- smaller versus larger true effect;
- n=30 versus n=120;
- low versus high residual variability;
- alpha=.05 versus .01;
- one case where design efficiency improves while total n stays fixed.

Required conclusion:

> Power is a function of effect + design + assumptions, not a permanent label attached to a sample.

---

## Pass 4 — power versus precision

Use F0.5 reasoning explicitly.

Prompt:

> Give me paired completed-study results with the same point estimate but different CI widths and a prespecified practical threshold. Ask me which is more precise and more informative. Do not let me answer using observed power.

For every result use:

`Target/measure:`
`Direction:`
`Magnitude:`
`Precision/CI:`
`Statistical output:`
`Practical meaning + unsupported claims:`

Then add:

`Prospective planning information:`

Critical rule:

> Prospective power describes a planned procedure; observed CI describes the uncertainty of the estimate actually obtained.

---

## Pass 5 — observed/post hoc power trap

Use Heinsberg & Weeks + Greenland + canonical lesson.

Prompt:

> Present one completed nonsignificant study at a time. Include estimate, 95% CI, p-value and an observed-power calculation made from the observed effect. Require me to explain why the observed-power number adds no independent result interpretation and to replace it with a CI-based conclusion.

Required repair sequence:

1. identify that the observed effect was fed back into a power formula;
2. reject observed power as posterior evidence;
3. interpret estimate + CI + practical threshold;
4. state what remains unresolved;
5. distinguish this misuse from prospective design sensitivity to an externally specified effect.

Never accept:

`low observed power → therefore false negative`.

---

## Pass 6 — sample-size justification by inferential goal

Use Lakens.

Prompt:

> Give me 12 study-planning scenarios and make me choose the most coherent sample-size justification: a-priori power, desired accuracy/precision, near-census, resource constraint, justified heuristic, or explicit absence of justification.

Require justification in words.

Include:

- confirmatory detection of a prespecified effect;
- estimation with target CI width;
- finite athlete population;
- expensive repeated-measures protocol;
- pilot/feasibility objective;
- no defensible rationale.

Critical rule:

> The sample-size rationale must match what the study needs to learn.

---

## Pass 7 — smallest effect / planning effect

Prompt:

> Give me planning effects from prior studies, practical thresholds and arbitrary conventional values. Make me judge which could be defensible and what evidence/logic is needed to justify each.

Required questions:

- Is this effect scientifically/practically meaningful?
- Is it merely the largest published significant effect?
- Is it plausible in the target population/design?
- Is precision rather than test rejection the real goal?
- Is the planning effect being confused with the observed effect?

Do not let the observed p-value define the planning effect.

---

## Pass 8 — multiplicity and simple family-wise risk

Use FDA + canonical lesson.

Prompt:

> Give me independent-test toy examples with m=1, 3, 5, 10 and 20, all relevant nulls true and per-test alpha=.05. Make me compute 1-.95^m and state the assumptions before interpreting the answer.

Required interpretation:

> Under the simplified stated assumptions, this is the repeated-use chance of at least one Type I rejection in the family.

Forbidden interpretation:

> “This is the probability the paper is wrong.”

Then ask why the formula cannot be copied mechanically to correlated outcomes/time points.

---

## Pass 9 — reconstruct the family before choosing a correction

Prompt:

> Give me trials with one primary endpoint, several key secondaries, exploratory biomarkers and multiple time points. Do not tell me the family. Make me infer which claims are intended as confirmatory and which tests must be considered jointly for the stated decision strategy.

For each scenario answer:

1. target confirmatory claim(s);
2. candidate hypothesis family;
3. exploratory analyses outside the confirmatory family;
4. whether artificial fragmentation is occurring;
5. what multiplicity strategy/documentation is needed.

Core rule:

> Family follows claims and decision strategy, not table layout.

---

## Pass 10 — hierarchy, alpha allocation and adjusted outputs

Use FDA at conceptual level.

Prompt:

> Give me five confirmatory-endpoint architectures. Make me choose among single-primary focus, hierarchy/gatekeeping, alpha allocation, adjusted p-values/intervals, or exploratory classification and explain one advantage and one limitation.

Include one simple Bonferroni example:

`family alpha .05 / 5 tests = .01 per test`.

Do not turn the pass into a catalog of corrections.

---

## Pass 11 — hypothesis multiplicity versus analytical-path multiplicity

Prompt:

> Give me one scientific outcome analyzed as raw endpoint, change score, ANCOVA, alternative covariate sets, with/without outliers and different transformations. Ask whether these are separate scientific hypotheses or alternative analytical paths, and what goes wrong if the smallest p-value is selected after seeing the data.

Required reasoning:

- model variants need not be independent hypotheses;
- they can still create selection opportunities;
- prespecified primary model/outlier/covariate rules improve auditability;
- sensitivity analyses are not automatically problematic when transparently planned/reported.

---

## Pass 12 — subgroup trap

Prompt:

> Present subgroup A with p=.03 and subgroup B with p=.20. Require me to explain why this does not prove an interaction. Then give an interaction estimate/CI and ask for the correct interpretation.

Required checks:

- direct interaction contrast;
- magnitude and CI;
- multiplicity;
- prespecification;
- plausibility;
- exploratory versus confirmatory status.

---

## Pass 13 — researcher degrees of freedom

Prompt:

> Generate a garden-of-forking-paths scenario with outcome definitions, time windows, exclusions, missing-data handling, transformations, covariates, subgroups, models and stopping/reporting decisions. Ask me to identify every decision that could become data-dependent.

Then require two lists:

1. legitimate flexibility that can be transparently handled;
2. flexibility that threatens confirmatory interpretation when selected after looking at results and incompletely reported.

Do not equate flexibility with misconduct automatically.

---

## Pass 14 — registration, preregistration, protocol and SAP

Use CONSORT 2025.

Prompt:

> Give me four document snippets with dates: registry entry, preregistration, protocol and SAP. Make me identify each document's role, detail level and what the timestamp proves or fails to prove.

Require checks for:

- document date/version;
- recruitment start;
- data availability/unblinding when relevant;
- primary/secondary outcomes;
- analysis population;
- covariates/model;
- missing-data handling;
- multiplicity strategy;
- subgroup/sensitivity analyses;
- deviations and rationale.

Critical rule:

`preregistered ≠ low risk of bias`.

---

## Pass 15 — confirmatory versus exploratory without stigma

Prompt:

> Give me 10 highlighted findings. Mix prespecified primary results, prespecified secondary results with unclear multiplicity control, post hoc subgroup discoveries and transparent exploratory analyses. Make me classify each as confirmatory, supportive/secondary, or exploratory and justify the language allowed.

Target lesson:

> Exploratory science is legitimate; undisclosed relabeling is the problem.

---

## Pass 16 — ASA 2016 versus ASA 2021

Use both ASA sources.

Prompt:

> Debate me in two rounds. First defend the false position “p<.05 is enough to confirm a scientific claim”. Then defend the opposite false position “p-values are intrinsically useless and should always be banned”. Make me rebut both using only the approved corpus.

Target synthesis:

- p-values can be useful statistical tools;
- thresholds do not replace effect magnitude, uncertainty, design or context;
- multiplicity/selective reporting can distort interpretation;
- transparent reporting and model awareness matter;
- no single statistic is a complete scientific conclusion.

---

## Pass 17 — ten-field integrated audit

For every synthetic paper, answer **all ten** fields in this order:

1. `Target claims:`
2. `Decision rules:`
3. `Power/sample-size assumptions:`
4. `Effective hypothesis family:`
5. `Analytical paths:`
6. `Prespecification evidence:`
7. `Multiplicity control:`
8. `Estimate/CI interpretation:`
9. `Confirmatory vs exploratory:`
10. `Transparent conclusion:`

Ask NotebookLM to generate at least six audits with increasing difficulty:

- one clean single-primary trial;
- one multiple-secondary trial with hierarchy;
- one many-endpoint trial with no multiplicity plan;
- one subgroup-heavy report;
- one model-selection/forking-paths report;
- one combined case with observed-power misuse and incomplete SAP reporting.

Never skip field 8. F0.6 cannot replace F0.5 estimate/CI interpretation.

---

# 5. Required integrated audit scenario

Use this exact synthetic case before the closed-book checkpoint:

- 120 athletes randomized to A or B;
- registry before recruitment:
  - primary: time-trial performance at week 12;
  - three secondary outcomes at week 12;
  - bilateral alpha `.05`;
  - planning effect `+2.0%`;
  - target power `80%`;
- no multiplicity strategy for secondary claims in the registry;
- no SAP linked by the paper;
- primary result: `+0.6%`, 95% CI `-0.5% to +1.7%`, `p=.28`;
- 20 outcomes × 4 time points;
- six subgroup definitions across the 20 week-12 outcomes;
- several covariate models;
- mood/week8 `p=.008` highlighted;
- high-baseline-fitness recovery subgroup `p=.03` highlighted;
- both called “confirmatory”;
- incomplete result reporting;
- observed power calculated from the observed primary effect to explain the nonsignificant primary result.

Required response: all ten audit fields.

Minimum correct conclusions:

- primary week-12 outcome is the clearly documented confirmatory target;
- 80% power is conditional on +2.0% and planning assumptions, not probability H1 is true;
- the primary estimate/CI must be interpreted directly;
- observed power does not rescue/explain the completed result;
- outcome/timepoint/subgroup/model choices create substantial multiplicity/selection opportunities;
- model variants are analytical paths, not automatically separate scientific hypotheses;
- registry supports some prespecification but missing SAP prevents full audit;
- mood/week8 and subgroup finding cannot be promoted to confirmatory from the information given;
- transparent reporting needs complete result families, estimates/CIs, multiplicity strategy and documented deviations.

---

# 6. Closed-book checkpoint

Without NotebookLM, notes or answer key, explain:

1. Type I error;
2. alpha;
3. Type II error;
4. beta;
5. power;
6. why power is effect/design dependent;
7. why `1-power` is not posterior false-negative probability;
8. power versus precision;
9. why observed power is generally uninformative;
10. what to use after study completion instead;
11. at least four defensible sample-size-justification strategies;
12. role of a smallest effect/planning effect;
13. family of hypotheses;
14. simple FWER complement calculation and its assumptions;
15. five sources of multiplicity;
16. hypothesis multiplicity versus analytical-path multiplicity;
17. endpoint hierarchy/gatekeeping concept;
18. subgroup-significance trap;
19. researcher degrees of freedom;
20. trial registration versus preregistration versus protocol versus SAP;
21. why timing/versioning matters;
22. why preregistration does not guarantee low bias;
23. confirmatory versus exploratory;
24. all ten fields of the F0.6 audit sequence.

Any answer containing a critical probability reversal requires repeating the relevant pass before independent assessment.

---

# 7. Independent assessment protocol

Only after study:

1. close NotebookLM;
2. complete `foundations/F0-scientific-literacy/F0.6-power-multiplicity-analytical-flexibility/EXERCISES.md` independently;
3. do not open `ANSWER_KEY.md` until the first attempt is complete;
4. submit the attempt for observed scoring;
5. route errors through the mastery/error protocol;
6. preserve F0.4/F0.5 prerequisite-state honesty;
7. do not infer `MASTERED` from one strong attempt alone.

Local unit gate remains:

`>=80/100 + no critical fail`

but applies only to actual observed performance.

---

# 8. Critical fails to detect during study

Any of these indicates structural misunderstanding:

- `power = P(H1 true)`;
- `1-power = P(this nonsignificant result is a false negative)`;
- observed/post hoc power used as evidence that a completed result missed or excluded an effect;
- many nominal unadjusted tests treated as independent confirmation merely because each uses alpha `.05`;
- subgroup A significant + subgroup B nonsignificant used as proof of interaction;
- preregistration treated as guarantee of low bias/validity;
- `p>.05` treated as proof of no effect when CI still permits important effects;
- completed-study interpretation omits estimate/CI and uses power instead.

---

# 9. Scope boundary with F0.7

Stop and label `F0.7` if a question requires full:

- systematic-review workflow;
- effect-measure compatibility for pooling;
- fixed-effect versus random-effects synthesis;
- inverse-variance weighting in meta-analysis;
- forest-plot pooled estimates;
- heterogeneity/I2 interpretation;
- sensitivity/subgroup/meta-regression in evidence synthesis;
- small-study effects/publication-bias diagnostics;
- decisions about whether studies should be pooled.

F0.6 may recognize that multiplicity and selective analysis affect the literature entering a meta-analysis, but it does not teach meta-analytic machinery.

---

# 10. Completion standard

The package has done its job when the learner can inspect an unfamiliar study and reliably produce:

`Target claims → Decision rules → Power/sample-size assumptions → Effective hypothesis family → Analytical paths → Prespecification evidence → Multiplicity control → Estimate/CI interpretation → Confirmatory vs exploratory → Transparent conclusion`

without:

- probability reversal for alpha/beta/power;
- observed-power rescue;
- treating high power as a cure for bias;
- ignoring practical thresholds and CI;
- mechanical counting of every model as a separate scientific hypothesis;
- uncritical acceptance of nominal p-values across many analyses;
- subgroup-significance comparison as interaction proof;
- equating preregistration with validity;
- treating exploratory findings as worthless;
- importing F0.7 meta-analysis machinery.

Package completion itself still changes no learner state.
