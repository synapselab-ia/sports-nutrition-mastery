# F0.5 — Practical NotebookLM Study Guide

**Package version:** `1`
**Module:** `F0.5 — Estimates, confidence intervals, p-values, effect sizes and practical relevance`
**Current learner state:** `UNSEEN`
**F0.4 quantitative diagnostic:** `UNOBSERVED`

This guide defines how to build and use the approved NotebookLM corpus for F0.5. Creating the notebook, reading sources or completing these study passes does **not** change learner state. Any transition requires observed performance under the mastery protocol.

## 0. Prerequisite integrity

F0.5 learner validation requires F0.4 as P2. The repository also still records the F0.4 quantitative entry diagnostic as `UNOBSERVED`.

Do not use this package to infer that F0.4 was mastered. If the goal is honest learner validation, complete prerequisite diagnostic/study/assessment in the canonical order before claiming F0.5 progression.

The F0.4 diagnostic must stay outside this notebook.

---

## 1. Create the notebook

Create one NotebookLM notebook named:

`Sports Nutrition Mastery — F0.5 Estimates and Uncertainty`

Keep it separate from F0.4. F0.4 supplies the prerequisite objects (sampling variability, SD, SE); F0.5 is the interpretation layer for estimates, intervals, p-values and effect measures.

---

## 2. Add exactly six initial sources

### Source 1 — canonical F0.5 lesson — CORE

Repository file:

`foundations/F0-scientific-literacy/F0.5-estimates-confidence-pvalues-effect-sizes/LESSON.md`

Preferred URL:

`https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.5-estimates-confidence-pvalues-effect-sizes/LESSON.md`

Use as the instructional spine for:

- parameter/estimator/estimate;
- point versus interval estimate;
- SD versus SE bridge;
- confidence-interval interpretation;
- p-values and ASA principles;
- MD/SMD/RD/RR/OR;
- absolute versus relative effects;
- log-scale intuition;
- smallest-effect/decision-threshold reasoning;
- forest/trial interpretation;
- F0.6 boundary.

If the raw URL cannot be ingested, upload the canonical Markdown file itself. Do not substitute an AI summary.

### Source 2 — Cochrane Handbook Chapter 6 — CORE

Add:

`https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-06`

Use for:

- MD and SMD;
- RD, RR and OR;
- difference versus ratio measures;
- null values;
- uncertainty accompanying effect estimates;
- log-scale intuition for ratio measures.

Do not study meta-analysis or advanced unit-of-analysis mechanics yet.

### Source 3 — ASA Statement on p-values — CORE

Add:

`https://www.amstat.org/asa/files/pdfs/P-ValueStatement.pdf`

Use it to learn and restate all six principles without quoting mechanically.

Required skill: given a false p-value interpretation, identify exactly which ASA principle it violates and repair the statement.

### Source 4 — Greenland et al. 2016 — SUPPORT

Add:

`https://pmc.ncbi.nlm.nih.gov/articles/PMC4877414/`

Use for:

- p-value probability reversals;
- frequentist CI coverage logic;
- why large p does not establish the null;
- why significance categories lose information;
- compatibility-oriented interpretation.

Ignore the article's detailed power discussion for now.

### Source 5 — Lakens 2022 — SUPPORT

Add:

`https://online.ucpress.edu/collabra/article/8/1/33267/120491/Sample-Size-Justification`

Use only for:

- smallest effect size of interest;
- why a meaningful threshold must be justified;
- why informativeness depends on the effects the study needs to distinguish/exclude.

Do not study formal power calculations in this module.

### Source 6 — ASA Task Force 2021 — CONTRAST

Add:

`https://magazine.amstat.org/blog/2021/08/01/task-force-statement-p-value/`

Use to answer this contrast question:

> Why is the correct lesson neither “p<0.05 decides truth” nor “p-values should never be used”?

The target answer should emphasize uncertainty, variability, replicability, transparent analysis and context.

---

## 3. Do NOT add these yet

Keep outside the initial notebook:

- F0.5 `EXERCISES.md` — independent assessment;
- F0.5 `ANSWER_KEY.md` — answer leakage;
- F0.5 production `QA_REPORT.md` — metadata;
- F0.4 `ENTRY_DIAGNOSTIC.md` — prerequisite diagnostic must remain uncontaminated;
- full `SOURCE_INDEX.md` — retrieval noise;
- FDA multiplicity source `F0-S10` — F0.6;
- formal power/sample-size calculators — F0.6;
- broad RoB/GRADE corpora — later modules;
- substantive sports-nutrition intervention papers — not needed for this methodological package.

---

# 4. Study sequence

Do not begin with “summarize all sources”. Complete the passes in order.

## Pass 1 — identify the statistical object

Prompt:

> Generate 12 short result statements. For each, make me identify parameter/target, estimator or estimate, effect measure and null value before any interpretation. Mix MD, RD, RR, OR and SMD. Do not reveal the answer until I commit.

For each result answer:

1. target/parameter;
2. observed estimate;
3. effect measure;
4. original/standardized/absolute/relative scale;
5. null value.

Critical trap: never assume the sign alone tells which group is better; outcome direction matters.

---

## Pass 2 — frequentist CI without Bayesian language

Use canonical lesson + Greenland.

Prompt:

> Give me eight confidence intervals. Make me explain the frequentist 95% meaning before interpreting the interval. Include difference and ratio measures. Reject any posterior-probability wording.

Required explanation:

- confidence level belongs to repeated-sampling coverage of the procedure under assumptions;
- the fixed parameter is not assigned a 95% posterior probability by a frequentist CI;
- interval width carries precision information;
- systematic bias can coexist with a narrow CI.

Then classify each CI by the practical zones it spans, not merely whether it crosses the null.

---

## Pass 3 — six ASA p-value principles

Use the official ASA statement.

First, explain all six principles from memory.

Then prompt:

> Present one false p-value interpretation at a time. Require me to name the violated ASA principle and rewrite the sentence correctly. Include p=0.03 as probability of H0, p<0.05 as proof, p>0.05 as no effect, p as effect magnitude, p=0.049 versus 0.051 as opposite truths, and selective-reporting scenarios.

Do not accept “that statement is wrong” without a replacement interpretation.

---

## Pass 4 — p-value and CI together

Use canonical lesson + ASA + Greenland.

Practice these contrasts repeatedly:

1. small p + narrow CI + practically trivial magnitude;
2. large p + wide CI spanning important benefit/harm;
3. large p + narrow near-null CI excluding meaningful effects;
4. p values immediately around 0.05 with almost identical estimates/intervals.

For every result, output exactly:

`Target/measure:`
`Direction:`
`Magnitude:`
`Precision/CI:`
`Statistical output:`
`Practical meaning + unsupported claims:`

Do not use “significant” or “nonsignificant” as the final conclusion.

---

## Pass 5 — MD versus SMD

Use Cochrane + canonical lesson.

Prompt:

> Generate six continuous-outcome scenarios. Alternate between same scale across studies and different scales measuring a similar construct. Make me choose MD or SMD and justify why.

Required reasoning:

- MD retains the original unit;
- SMD divides by a dispersion quantity and is expressed in SD units;
- SMD is not automatically more useful;
- `0.2/0.5/0.8` must not become universal practical thresholds;
- if SMD is reported, ask what scale/SD/population generated it.

Include at least three manual SMD calculations from supplied MD and SD.

---

## Pass 6 — RD, RR and OR

Use Cochrane + canonical lesson.

Prompt:

> Give me 10 two-group binary tables. Require me to calculate risk in both groups, RD, RR, odds in both groups and OR. Mix common and rare outcomes. Do not let me call OR a risk ratio.

For each table answer:

1. baseline risk;
2. treated/exposed risk;
3. RD in percentage points;
4. RR;
5. OR;
6. which measures are absolute versus relative;
7. practical interpretation with baseline retained.

---

## Pass 7 — same relative effect, different baseline

Prompt:

> Generate paired scenarios with the same RR but very different baseline risks. Require me to calculate RD and explain why practical impact changes.

Minimum contrasts:

- 20% → 10% versus 2% → 1%;
- 40% → 20% versus 4% → 2%;
- one example where OR and RR visibly diverge because the event is common.

Required sentence structure:

> “The relative effect is ___, but the absolute effect is ___ because baseline risk is ___.”

---

## Pass 8 — practical thresholds / smallest effect of interest

Use Lakens + canonical lesson.

Prompt:

> Give me synthetic estimates and 95% CIs together with a prespecified practical threshold. Make the intervals alternate among: entirely meaningful, entirely trivial, spanning trivial and meaningful benefit, spanning harm and benefit, and precise near-null exclusion of meaningful effects.

For every case:

1. locate null;
2. locate practical threshold(s);
3. list practical zones included in the CI;
4. state what is resolved;
5. state what remains unresolved.

Do not let the p-value define the threshold.

---

## Pass 9 — ratio measures on log-scale intuition

Use Cochrane.

Without calculating logs manually, explain:

- why 0.5 and 2 are reciprocal effects;
- why 1 is null;
- why a log scale represents reciprocal ratios symmetrically;
- why forest plots of RR/OR are commonly displayed on log scales.

Ask NotebookLM to show visual/number-line thought experiments rather than advanced formulas.

---

## Pass 10 — forest-plot row interpretation

Ask NotebookLM to generate at least 12 single forest-plot rows, alternating:

- MD;
- SMD;
- RR;
- OR;
- intervals crossing and not crossing null;
- narrow and wide intervals;
- practical thresholds different from the null.

For every row use the six required blocks.

Critical rule:

> Crossing the null is one fact about the interval, not the whole interpretation.

---

## Pass 11 — synthetic trial-table interpretation

Prompt:

> Generate synthetic trial tables with group n, event counts or means/SDs, plus a model estimate, 95% CI, p-value and prespecified practical threshold. Require me to calculate/check the effect measure, then produce the six-block interpretation.

Include:

- one p-small/trivial-effect table;
- one p-large/imprecise table;
- one precise near-null table;
- one binary table requiring RD/RR/OR;
- one scenario with likely causal/bias questions that F0.5 alone cannot resolve.

---

## Pass 12 — balanced p-value view

Use ASA 2016 + ASA Task Force 2021.

Prompt:

> Debate me in two rounds. First defend the false position “p<0.05 should decide scientific truth”. Then defend the opposite false position “p-values are intrinsically useless and should always be banned”. Make me rebut both using only the approved corpus.

Target synthesis:

- p-values can be valid/useful statistical tools;
- they are model-conditional and easy to misuse;
- they cannot replace magnitude, uncertainty, design, transparency and context;
- multiplicity/replicability mechanics belong later.

---

# 5. Final closed-book checkpoint

Without NotebookLM, notes or answer key, explain:

1. parameter vs estimator vs estimate;
2. frequentist 95% CI meaning;
3. six ASA principles;
4. why p small ≠ large/important effect;
5. why p large ≠ no effect;
6. MD vs SMD;
7. RD vs RR vs OR;
8. why baseline risk is required for practical interpretation of relative effects;
9. what smallest effect of interest means;
10. difference between imprecision and precise exclusion of meaningful effects;
11. why narrow CI does not cure bias;
12. the six-block interpretation sequence.

If any answer collapses to threshold memorization, repeat the relevant pass before independent assessment.

---

# 6. Independent assessment protocol

Only after study:

1. close NotebookLM;
2. complete `foundations/F0-scientific-literacy/F0.5-estimates-confidence-pvalues-effect-sizes/EXERCISES.md` independently;
3. do not open `ANSWER_KEY.md` until the first attempt is complete;
4. submit the attempt for observed scoring;
5. route errors through the mastery/error protocol;
6. do not infer `MASTERED` from one strong attempt alone; cumulative retesting remains required.

Local unit gate remains:

`>=80/100 + no critical fail`

but it applies only to actual observed performance.

---

# 7. Scope boundary with F0.6

Stop and label `F0.6` if a question requires formal:

- alpha/beta operating characteristics;
- Type I or Type II error calculations;
- power calculation;
- observed/post hoc power critique in depth;
- multiplicity adjustment;
- FWER/FDR;
- endpoint hierarchy algorithms;
- subgroup multiplicity;
- sequential testing;
- analytical-flexibility/prespecification mechanics.

F0.5 may recognize that these issues matter but does not teach the machinery.

---

# 8. Completion standard

The study package has done its job when the learner can take an unfamiliar result and reliably produce:

`Target/measure → Direction → Magnitude → Precision/CI → Statistical output → Practical meaning + unsupported claims`

without:

- posterior-probability language for a frequentist CI;
- truth/no-effect claims from p thresholds;
- universal SMD labels;
- RR/OR confusion;
- relative effects without baseline context;
- confusing precision with validity;
- pulling F0.6 machinery forward.

Package completion itself still changes no learner state.