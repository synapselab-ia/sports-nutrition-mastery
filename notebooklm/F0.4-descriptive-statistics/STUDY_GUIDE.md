# F0.4 — Practical NotebookLM Study Guide

**Package version:** `1`
**Module:** `F0.4 — Descriptive statistics, distributions and sampling variation`
**Current learner state:** `UNSEEN`
**Current quantitative diagnostic state:** `UNOBSERVED`

This guide defines how to build and use the approved NotebookLM corpus for F0.4. Creating the notebook, reading sources or completing this guide does **not** change learner state. Any transition requires observed performance under the mastery protocol.

## 0. Before NotebookLM: preserve the entry diagnostic

If `ENTRY_DIAGNOSTIC.md` is still `UNOBSERVED`, do **not** start studying F0.4 first if the goal is honest learner validation.

Correct order:

1. open `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/ENTRY_DIAGNOSTIC.md`;
2. complete it independently, without NotebookLM, F0.4 lesson, AI or answer key;
3. submit the answers for scoring/routing;
4. complete any `P1_REPAIR` or conditional `P2-QB` work actually indicated by observed responses;
5. then begin this NotebookLM study sequence.

Do not open `ANSWER_KEY.md` before the first diagnostic attempt because it contains the diagnostic answers.

Merely reading this study guide does not produce a diagnostic result. Until actual responses exist, canonical state remains:

`F0.4 quantitative diagnostic = UNOBSERVED`

---

## 1. Create the notebook

Create one NotebookLM notebook named:

`Sports Nutrition Mastery — F0.4 Descriptive Statistics`

Do not merge the F0.1–F0.3 notebooks into this notebook. Their concepts remain prerequisites, but F0.4 needs a compact retrieval space focused on data description and sampling variation.

---

## 2. Add exactly four initial sources

### Source 1 — canonical F0.4 lesson — CORE

Repository file:

`foundations/F0-scientific-literacy/F0.4-descriptive-statistics/LESSON.md`

Preferred NotebookLM URL:

`https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.4-descriptive-statistics/LESSON.md`

Use it as the primary instructional spine for:

- variable types and measurement scales;
- distribution shape;
- center and dispersion;
- outliers;
- graphs;
- population/sample;
- parameter/statistic;
- sampling variability;
- sample distribution versus sampling distribution;
- SD versus SE;
- sample-size intuition;
- transformations at conceptual level;
- F0.5/F0.6 scope boundaries.

If NotebookLM cannot ingest the raw Markdown URL, upload the canonical Markdown file itself. Do not replace it with an AI-generated summary.

### Source 2 — NIST Exploratory Data Analysis chapter — CORE

Add as website:

`https://www.itl.nist.gov/div898/handbook/eda/eda.htm`

Use it primarily for:

- why exploratory data analysis precedes mechanical modeling/testing;
- graphical examination of data;
- revealing structure hidden by one-number summaries;
- outliers/anomalies;
- distribution shape;
- graphical techniques and their analytical role.

The NIST chapter links to many subpages. Use only the descriptive/EDA material needed for F0.4. Do not let NotebookLM drag later hypothesis-testing/modeling procedures into the unit.

### Source 3 — Altman & Bland on SD versus SE — SUPPORT

Add as website:

`https://www.bmj.com/content/331/7521/903`

Use it for:

- SD = variability among observations;
- SE = sampling variability/precision of an estimate;
- why mean ± SE is not a description of the spread of individuals;
- the simple relation `SE(mean) = SD/√n`.

Do not use this source to study confidence intervals yet. That belongs to F0.5.

### Source 4 — ICH E9/E9(R1) — CONTRAST

Add as website:

`https://www.ema.europa.eu/en/ich-e9-statistical-principles-clinical-trials-scientific-guideline`

Use only for this boundary question:

> How do objectives, variables/endpoints, estimands and analyses need to align, and why does a descriptive summary not by itself answer a treatment-effect question?

Do **not** learn regulatory submission detail, sensitivity-analysis machinery or advanced estimand implementation in F0.4.

---

## 3. Do NOT add these yet

Keep all of these outside the initial notebook:

- `ENTRY_DIAGNOSTIC.md` — prerequisite instrument must remain uncontaminated until completed;
- `EXERCISES.md` — independent F0.4 assessment;
- `ANSWER_KEY.md` — contains both diagnostic and exercise answers;
- F0.4 production `QA_REPORT.md` — production metadata, not study evidence;
- full `SOURCE_INDEX.md` — unnecessary retrieval noise;
- ASA p-value materials — F0.5/F0.6;
- sample-size/power source `F0-S13` — F0.6;
- effect-measure/meta-analysis chapters — later units;
- broad causal/risk-of-bias corpora — F0.2/F0.3 prerequisites, not first-pass F0.4 sources.

---

# 4. Study sequence

Follow the passes in order. Do not start with “summarize all four sources.”

## Pass 1 — classify the data object before calculating

Read the canonical lesson sections on observations, variables and scales.

Ask NotebookLM:

> Using only the F0.4 lesson, generate 12 variables from synthetic exercise/sports datasets. Mix nominal, ordinal, discrete numerical and continuous numerical variables. Present one at a time. Do not reveal the type until I answer. Require me to explain what the values represent and why storing a category as 1/2/3 does not make it a quantitative scale.

For every variable answer:

1. variable type;
2. measurement-scale intuition if useful;
3. meaningful summaries;
4. one meaningless operation or summary to avoid.

Required traps:

- jersey number stored as integer;
- ordinal effort category stored 1–5;
- number of sessions;
- exact time recorded to two decimals;
- binary event coded 0/1.

The goal is to classify from **meaning**, not software format.

---

## Pass 2 — distribution before summary

Use the lesson plus NIST EDA.

Ask:

> Give me six small numerical datasets. Include approximate symmetry, strong right skew, left skew, two clusters, a bounded variable and one dataset with an extreme value. Do not recommend a center/dispersion pair until I describe the distribution first.

For each dataset produce, in this order:

1. distribution features;
2. candidate center;
3. candidate dispersion;
4. why another common summary could mislead;
5. graph that would expose the relevant structure.

Then explain from memory:

- why equal means do not imply equal distributions;
- why mean and median answer different center questions;
- why median/IQR are often robust but not universally superior;
- why strong skew is about tail shape rather than a rigid `mean > median` rule.

---

## Pass 3 — center and dispersion calculations

Ask NotebookLM to create short datasets that allow manual calculation.

Without help, calculate:

- mean;
- median;
- mode when meaningful;
- range;
- sample variance using the convention in the canonical lesson;
- SD;
- Q1/Q3 and IQR using a convention stated in the question.

For each calculation, state the **unit** of the result.

Critical distinction:

- if the variable is `kg`, sample variance is in `kg²`;
- SD is back in `kg`.

Ask NotebookLM to grade arithmetic only after you show the work.

---

## Pass 4 — outliers: investigate, do not erase

Use the lesson plus NIST EDA.

Prompt:

> Generate six scenarios containing a visually extreme value. Alternate among data-entry error, unit-conversion error, sensor failure, plausible rare biological observation, genuine subgroup and unresolved anomaly. Present one scenario at a time. Require me to propose a verification plan before deciding whether to exclude, correct, retain or analyze separately.

Your response must follow:

`detect → verify origin → classify explanation → treatment decision → documentation → sensitivity implication if relevant`

Reject the rule:

> “Outlier = delete.”

Also reject the opposite rule:

> “Every extreme value must always remain unchanged regardless of proven measurement error.”

The correct answer depends on provenance and scientific context.

---

## Pass 5 — visualization as analysis

Use the lesson plus NIST EDA.

### 5A. Choose a graph

Ask NotebookLM to give a sequence of variable/question pairs. Choose among:

- dot/strip plot;
- histogram;
- boxplot;
- bar chart;
- scatterplot.

For every choice state:

1. what the graph exposes;
2. what it can hide;
3. what alternate graph would complement it.

### 5B. Audit misleading graphs

Use this prompt:

> Generate misleading visualization scenarios one at a time. Include truncated y-axes, bars of means that hide individual data, incompatible scales between panels, selective time windows, over/under-binned histograms and a scatterplot interpreted causally. Do not tell me the problem until I identify it.

For each scenario answer:

- what is numerically true;
- what visual encoding changes perception;
- what cannot be concluded;
- how to improve the display.

Critical rule:

> A truncated axis is not automatically fraudulent. The learner must identify exactly how the scale changes visual magnitude and still read the numerical difference correctly.

---

## Pass 6 — population, sample, parameter and statistic

Ask:

> Create ten statements using words like mean, proportion, median and SD. Sometimes the number refers to the entire target population and sometimes to an observed sample. Present one statement at a time and require me to label population/sample and parameter/statistic.

You must be able to explain:

- population = target collection of units;
- sample = observed units;
- parameter = numerical property of population;
- statistic = quantity calculated from sample.

Then create one synthetic sports-science example in which:

- target population is broader than recruited sample;
- sample mean is observed;
- population mean is unknown;
- F0.4 description stops before claiming how close the sample mean is to the population mean with a confidence interval.

---

## Pass 7 — sample distribution versus sampling distribution

This is a major gate.

Ask NotebookLM:

> Teach sample distribution versus sampling distribution using one fixed hypothetical population. First show one sample of 10 observations and ask me what the sample distribution contains. Then imagine drawing 10,000 independent samples of size 10 and computing a mean from each; ask me what the sampling distribution contains. Do not introduce confidence intervals or p-values.

You must answer without notes:

### Sample distribution

What varies?

`individual observed values within one sample`

### Sampling distribution of the mean

What varies?

`the sample mean across hypothetical repeated samples`

Then explain why the phrase “distribution of means” belongs to the second object, not the first.

Critical fail to prevent:

> “Sampling distribution is just the histogram of the participant values.”

---

## Pass 8 — SD versus SE

Use the canonical lesson plus Altman & Bland.

Ask:

> Compare SD and SE without using confidence intervals. For every example, force me to identify the object being described before choosing SD or SE.

Memorize meaning, not merely formula:

- `SD` → spread of observations around their mean;
- `SE` → sampling variability/precision of an estimator across repeated samples.

Then calculate these simple cases:

### Case A

`SD = 10`, `n = 25`

`SE(mean) = 10/√25 = 2`

### Case B

`SD = 10`, `n = 100`

`SE(mean) = 10/√100 = 1`

Explain why:

- SE halved;
- SD did not need to change;
- this does not mean people in n=100 were half as variable.

### Case C — predict before calculating

If n increases from 25 to 225 with same SD:

- n becomes 9× larger;
- √n becomes 3× larger;
- SE becomes approximately 1/3 as large.

### Scope guard

The formula is used only for the simple sample mean under the F0.4 independent-observation setting. Do not generalize it blindly to clustered, paired, weighted or model-based estimators.

---

## Pass 9 — what larger n changes and does not change

Ask NotebookLM:

> Give me eight paired scenarios where sample size changes but the same data-generating population is assumed. Ask me to predict separately what happens to sample-mean stability, SE, observed SD, range, bias, representativeness and causal validity.

Required reasoning:

### Usually becomes more stable with larger n

- sample mean and many sample statistics;
- sampling distribution of mean becomes narrower under standard conditions;
- SE of mean decreases when SD is comparable.

### Does not automatically decrease

- population heterogeneity;
- individual SD;
- systematic measurement bias;
- confounding;
- selection bias.

### Can increase

- observed range, because larger samples have more opportunities to include extremes.

Reject:

> “Large n makes the study unbiased.”

Reject:

> “Large n guarantees a small SD.”

---

## Pass 10 — transformations: conceptual only

Return to the canonical lesson.

Ask:

> Give me five examples where a variable is positive and strongly right-skewed or naturally multiplicative. Explain conceptually what a log transformation changes about scale and shape, but do not teach regression diagnostics or hypothesis tests.

You must preserve these boundaries:

- a transformation changes representation/scale;
- it can make multiplicative structure easier to see;
- back-transformation changes interpretation;
- it does not erase confounding, selection bias, measurement error or poor design;
- it is not a trick for forcing a desirable p-value.

---

## Pass 11 — ICH E9 contrast: description is not the target effect

Use ICH E9/E9(R1) only after the descriptive concepts are stable.

Ask:

> At a basic F0.4 level, explain why the statistical summary must remain aligned with the scientific objective, variable/outcome and target quantity. Do not teach regulatory detail, formal estimand strategies, confidence intervals or sensitivity analyses.

Then critique this statement:

> “Group A had mean 50 and Group B mean 54, therefore the causal treatment effect is +4.”

Your answer must separate:

1. observed descriptive difference;
2. causal-design validity from F0.2/F0.3;
3. uncertainty/effect interpretation deferred to F0.5;
4. why a descriptive calculation alone cannot supply missing design information.

---

## Pass 12 — mixed F0.4 examiner

Use this exact prompt:

> Act as an F0.4 examiner. Present one unfamiliar synthetic dataset or graph scenario at a time. Randomly alternate among variable classification, distribution shape, center/dispersion choice, outlier handling, visualization audit, population/sample, parameter/statistic, sample versus sampling distribution, SD versus SE, larger-n prediction and conceptual transformation. Wait for my answer. Require the response fields relevant to the case. Never reveal answers before I attempt. Do not use confidence intervals, p-values, effect sizes, formal power or multiplicity as solutions. Cite only the approved four-source corpus when grading.

Continue until decisions are made from data structure rather than trigger words.

---

# 5. Source-comparison tasks

## Task A — canonical lesson versus NIST EDA

Ask:

> What does the project lesson standardize for F0.4, and what does NIST add about exploratory graphical inspection? Give examples where a one-number summary hides structure that a graph reveals.

Expected distinction:

- lesson = project-wide curriculum spine, formulas, vocabulary, scope and sports-flavored examples;
- NIST = external methodological anchor for EDA/graphics/outlier discovery;
- neither makes a graph self-interpreting without variable/context knowledge.

## Task B — Altman & Bland versus common reporting language

Ask:

> A paper reports 50 ± 2 but does not say whether 2 is SD or SE. Why is the notation scientifically ambiguous? What different questions would SD=2 and SE=2 answer?

Required conclusion:

- `mean ± SD` communicates individual spread around mean;
- `mean ± SE` communicates precision/sampling variability of mean;
- the same numeric value represents a different statistical object.

## Task C — NIST versus automatic outlier deletion

Ask:

> Why does detecting an outlier/anomaly during EDA not imply deleting it? Separate detection from provenance verification and scientific treatment.

## Task D — F0.4 versus ICH E9

Ask:

> What can F0.4 describe perfectly while still being insufficient to answer a treatment-effect question? Explain how objective/outcome/target quantity alignment constrains interpretation without importing F0.5 inference.

---

# 6. Required evidence-critique exercise inside NotebookLM

Use the synthetic report from the manifest:

> Group A mean 50, SE 1; Group B mean 54, SE 1; y-axis begins at 48; only bars are shown. Authors say Group B participants were much less variable and the intervention clearly produced a large improvement.

Before asking NotebookLM to grade you, answer:

1. What is descriptively observed?
2. What does SE=1 describe?
3. Why can individual variability not be inferred from SE alone without n/SD?
4. What does the y-axis choice change visually?
5. What graph would expose individual/distribution structure?
6. Why is “much less variable” unsupported?
7. Why is “large” not established by F0.4 alone?
8. Why is “produced” a causal claim requiring F0.2/F0.3?
9. What bounded conclusion is defensible?

Do not let NotebookLM answer before your attempt.

---

# 7. Independent assessment outside NotebookLM

After completing the study sequence:

1. open `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/EXERCISES.md`;
2. answer the full assessment **without NotebookLM and without `ANSWER_KEY.md`**;
3. only after the first attempt, use `ANSWER_KEY.md` or submit answers to ChatGPT for correction;
4. local gate is `>=80/100` plus no critical fail;
5. one strong attempt can support progression evidence but does not automatically mean `MASTERED`;
6. later cumulative retesting is still required by the mastery protocol.

The NotebookLM package itself does not change `UNSEEN`.

---

# 8. Critical-fail patterns to prevent

Treat these as structural errors even when arithmetic is good:

- calling categorical codes quantitative merely because they are numbers;
- choosing a center/dispersion pair without inspecting distribution structure;
- claiming median/IQR are always better than mean/SD;
- defining right skew solely as `mean > median`;
- automatically deleting outliers;
- confusing histogram with bar chart;
- interpreting scatterplot association as causality;
- reading effect magnitude only from visual bar/axis area;
- confusing population with sample or parameter with statistic;
- calling the histogram of participant values a sampling distribution of the mean;
- using SE to describe individual variability;
- claiming larger n automatically lowers SD;
- claiming larger n eliminates systematic bias;
- using F0.5/F0.6 concepts as though they were already taught.

---

# 9. What to send back to ChatGPT after study

For honest state updates, provide:

- the completed entry diagnostic if it has not yet been scored; and later
- completed F0.4 `EXERCISES.md` answers, or answers to a fresh equivalent assessment administered in chat.

Statements such as “I read everything” or “I understood” are not sufficient evidence for `RECALLED`, `APPLIED`, `INTEGRATED` or `MASTERED`.

---

# 10. When NotebookLM disagrees with GitHub

Use this order:

1. inspect the exact external source cited by NotebookLM;
2. inspect the canonical F0.4 lesson and manifest;
3. determine whether the discrepancy is source version, scope or interpretation;
4. if GitHub is demonstrably wrong/outdated, verify externally and update the repository;
5. do not silently treat NotebookLM output as canonical.

Particular boundary checks:

- NIST material may include methods beyond F0.4;
- Altman & Bland may mention CI, which belongs to F0.5;
- ICH E9/E9(R1) contains regulatory/estimand detail beyond the assigned contrast role.

---

# 11. Package completion criterion

The F0.4 notebook is correctly configured when:

- exactly four approved sources are loaded;
- diagnostic, exercises and answer key are absent;
- the diagnostic was completed first if learner validation is being pursued;
- variable meaning is classified before summary selection;
- distribution is inspected before center/dispersion choice;
- outliers trigger investigation rather than automatic deletion;
- graphs are used as analytical objects;
- sample/population and statistic/parameter are separated;
- sample distribution and sampling distribution are separated;
- SD and SE are explained as different objects;
- simple `SE(mean) ≈ SD/√n` reasoning is fluent;
- larger n is not confused with lower individual variability or lower bias;
- transformations remain conceptual;
- F0.5/F0.6 content is not pulled forward;
- final assessment is completed independently outside NotebookLM.
