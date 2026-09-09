# F0.4 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-09`
**Learner state affected:** none
**Quantitative diagnostic state affected:** none (`UNOBSERVED` remains canonical until real responses exist)

This manifest defines the approved, deliberately small NotebookLM corpus for `F0.4 — Descriptive statistics, distributions and sampling variation`. GitHub remains canonical; NotebookLM is a source-controlled study layer.

The first-pass corpus is intentionally limited to **four sources**. F0.4 is not a literature-survey unit. Its purpose is to make the learner repeatedly execute the descriptive-statistics reasoning sequence:

`variable type → measurement scale/context → distribution shape → center + dispersion → outliers/anomalies → visualization → population/sample + parameter/statistic → sample distribution vs sampling distribution → SD vs SE → sample-size consequence → bounded conclusion`

The package deliberately stops before full confidence-interval, p-value and effect-size interpretation (F0.5) and before formal power, Type I/II error and multiplicity (F0.6).

```yaml
module_id: "F0.4"
module_title: "Descriptive statistics, distributions and sampling variation"
version: 1
learning_objectives:
  - "Classify variables as categorical nominal/ordinal or numerical discrete/continuous from what the values represent rather than from file encoding alone."
  - "Use nominal/ordinal/interval/ratio scale language as a reasoning aid without treating the taxonomy as an automatic analysis-selection machine."
  - "Inspect distribution shape before choosing a summary and describe symmetry, skew, multimodality, bounds and potential outliers."
  - "Choose and justify an appropriate measure of center: mean, median or mode."
  - "Choose and justify an appropriate measure of dispersion: range, variance/SD, IQR or quantiles."
  - "Explain why equal means can hide radically different distributions."
  - "Explain sample variance, SD and their units at an applied level without requiring proof-based statistics."
  - "Treat outliers as observations requiring verification and contextual investigation rather than automatic deletion."
  - "Choose and audit dot/strip plots, histograms, boxplots, bar charts and scatterplots for the question and variable type."
  - "Detect visual distortions caused by axis scale, aggregation, hidden distributions, incompatible scales or selective display windows."
  - "Distinguish population from sample and parameter from statistic."
  - "Explain sampling variability as the reason repeated samples from the same population can yield different statistics."
  - "Distinguish the distribution of observed sample values from the sampling distribution of a statistic across hypothetical repeated samples."
  - "Distinguish SD as individual-level spread from SE as sampling variability/precision of an estimate."
  - "Use SE(mean) ≈ SD/√n only in the simple independent-observation setting taught in F0.4."
  - "Predict that increasing n, with comparable underlying variability, usually reduces the mean SE but does not automatically reduce individual-level SD, systematic bias or the population's heterogeneity."
  - "Explain why sample range can increase as n grows even when the underlying distribution is unchanged."
  - "Treat transformations as changes of scale that may clarify skew/structure, not as tools for erasing bias or forcing acceptable results."
  - "Keep descriptive evidence separate from causal, significance and practical-effect claims that require later modules."

sources:
  - source_id: "F0-R04"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.4 — Estatística descritiva, distribuições e variação amostral. Canonical project lesson, version current at manifest v1."
    url_or_doi: "https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.4-descriptive-statistics/LESSON.md"
    why_included: "Primary instructional spine. It defines the exact F0.4 scope, vocabulary, formulas, worked examples, anti-errors and curricular boundaries. It also translates general statistical concepts into synthetic exercise/nutrition-flavored examples without making substantive nutrition recommendations."
    limitation: "Project-authored teaching material, not an independent external authority. Material claims must remain traceable to the registered methodological sources and later modules must replace F0.4 simplifications when more formal inference is introduced."

  - source_id: "F0-S12"
    priority: "CORE"
    citation: "NIST/SEMATECH. e-Handbook of Statistical Methods. National Institute of Standards and Technology. Relevant first-pass material: Chapter 1, Exploratory Data Analysis."
    url_or_doi: "https://www.nist.gov/publications/nistsematech-e-handbook-statistical-methods-chapter-1-exploratory-data-analysis"
    why_included: "Authoritative institutional anchor for exploratory data analysis: inspect data graphically, uncover structure, detect outliers/anomalies and avoid reducing analysis to one summary number. It directly supports F0.4 distribution-first and visualization-first habits."
    limitation: "The handbook is general/engineering-oriented and substantially broader than F0.4. The modern NIST publication page is preferred for stable access because the legacy framed e-Handbook interface may not ingest cleanly in NotebookLM. Use only descriptive/EDA concepts in this module; do not pull later testing/modeling machinery forward."

  - source_id: "F0-S27"
    priority: "SUPPORT"
    citation: "Altman DG, Bland JM. Standard deviations and standard errors. BMJ. 2005;331(7521):903. doi:10.1136/bmj.331.7521.903."
    url_or_doi: "https://www.bmj.com/content/331/7521/903"
    why_included: "Focused support for the highest-risk F0.4 misconception: SD describes variability of observations whereas SE describes sampling variability/precision of an estimate. It also gives the simple mean relation SE = SD/√n."
    limitation: "Short 2005 educational note, not a comprehensive statistics text. Its confidence-interval discussion is outside the F0.4 first-pass target and belongs to F0.5. The package uses only the stable SD/SE/sampling-variation distinction."

  - source_id: "F0-S14"
    priority: "CONTRAST"
    citation: "International Council for Harmonisation. ICH E9: Statistical Principles for Clinical Trials; ICH E9(R1) Addendum on Estimands and Sensitivity Analysis in Clinical Trials. Current Step 5 versions accessed through EMA."
    url_or_doi: "https://www.ema.europa.eu/en/ich-e9-statistical-principles-clinical-trials-scientific-guideline"
    why_included: "Boundary/contrast source. It situates descriptive summaries inside a larger chain where objectives, variables/endpoints, estimands and analyses must align. It is used to prevent the learner from treating a descriptive statistic as though it independently answered an inferential or causal question."
    limitation: "Regulatory clinical-trial guidance and much more technical than F0.4. Do not study regulatory detail, sensitivity-analysis machinery or formal estimand implementation here. Its role is contrast and scope control, not to dictate every descriptive summary."

claims_to_master:
  - "The first descriptive question is what kind of variable and data structure exist, not which statistical test to run."
  - "Categorical codes do not become meaningful numerical quantities merely because they are stored as numbers."
  - "A numerical variable can be discrete or continuous according to what it represents, not merely the number of decimal places in a file."
  - "Nominal/ordinal/interval/ratio language helps identify meaningful operations but does not mechanically determine every analysis."
  - "A distribution contains information about center, spread, shape, tails, clusters, bounds and unusual observations; a single mean can hide these features."
  - "Mean uses all magnitudes and is sensitive to extremes; median is order-based and more resistant to extremes; neither is universally superior."
  - "Mode is the most frequent category/value and may be non-unique or uninformative."
  - "Range uses only minimum and maximum; IQR describes the middle roughly 50% of ordered data and is less sensitive to extremes."
  - "Sample variance uses squared deviations and is expressed in squared units; SD is its square root and returns to the original unit."
  - "Quantile conventions can differ slightly in small samples; material calculations should specify the convention when needed."
  - "Right skew is defined by a longer upper/right tail, not by an absolute rule that mean must exceed median."
  - "An outlier is not automatically an error. The correct sequence is detect → verify origin → justify treatment → document."
  - "Histograms display distributions of numerical variables using bins; bar charts primarily display counts/proportions of categories."
  - "A boxplot is compact but can hide multimodality or individual observations; a dot/strip plot can expose small-sample structure more directly."
  - "A scatterplot can display association between two numerical variables but does not by itself establish causality."
  - "Axis truncation is not automatically invalid, but visual magnitude must be interpreted from the numerical scale and context rather than bar/line area alone."
  - "A population is the target set of units; a sample is the observed subset. A parameter describes a population and a statistic is computed from a sample."
  - "Different random samples from the same population can produce different sample means, medians, SDs and other statistics. That variation is sampling variability."
  - "The sample distribution is the distribution of observed values in one sample. The sampling distribution is the distribution of a statistic across hypothetical repeated samples."
  - "SD and SE describe different objects. SD describes variability among observations; SE describes variability/precision of an estimator across repeated samples."
  - "For the simple sample mean under the F0.4 assumptions, SE(mean) ≈ SD/√n."
  - "If SD is comparable, multiplying n by four approximately halves SE(mean); multiplying n by two reduces it by a factor of 1/√2, not by half."
  - "Increasing sample size does not automatically shrink individual SD, eliminate systematic bias or make the sample representative."
  - "Larger samples can show a wider observed range simply because more opportunities exist to encounter extreme observations."
  - "Transformations alter the scale/shape representation and may help with skew or multiplicative structure, but they do not erase bias or convert a poor design into a valid one."
  - "Descriptive statistics do not alone answer confidence-interval, p-value, effect-size, power, causal or practical-importance questions."

controversies_or_limits:
  - "Rules such as 'use mean/SD for normal data and median/IQR otherwise' are only rough heuristics. F0.4 requires the learner to justify the summary from the question, variable meaning, distribution shape and robustness needs."
  - "The classical nominal/ordinal/interval/ratio scale taxonomy is useful but can be oversimplified. The lesson deliberately avoids turning it into a mechanical decision tree for statistical procedures."
  - "Outlier identification can depend on visual/statistical criteria and scientific context. The package does not authorize automatic deletion based on a single cutoff."
  - "Histogram appearance depends on bin width and origin; one histogram is not a unique visual truth."
  - "Boxplot whisker conventions vary across software; the learner should inspect definitions before treating a flagged point as erroneous."
  - "The simple relation SE = SD/√n is taught for the sample mean in a basic independent-observation setting. Clustered, paired, weighted and model-based estimators need structure-specific standard errors later."
  - "The standard error usually becomes smaller with more independent information, but F0.4 does not derive asymptotic theory or formal estimator variance."
  - "The NIST handbook contains later inferential methods. NotebookLM must not use those to teach p-values/CI/power prematurely."
  - "Altman & Bland discuss confidence intervals, but CI interpretation belongs to F0.5 and is not a first-pass F0.4 objective."
  - "ICH E9/E9(R1) is a regulatory trial framework. Its presence is to reinforce alignment and inferential boundaries, not to make F0.4 a regulatory-statistics unit."
  - "Synthetic exercise/nutrition examples illustrate statistics only. They are not empirical evidence for nutrition interventions, dosing or performance claims."

active_recall:
  basic:
    - "Classify five variables as nominal, ordinal, discrete numerical or continuous numerical and justify each classification from meaning rather than file format."
    - "Define mean, median, mode, range, sample variance, SD, Q1, Q3 and IQR."
    - "What is the unit of variance if the original variable is in kilograms? What is the unit of SD?"
    - "Define population, sample, parameter and statistic."
    - "Define sample distribution and sampling distribution without using the word 'distribution' as the entire explanation."
    - "Define SD and SE in one sentence each."
  mechanism:
    - "Explain why one extreme high value can pull the mean much more than the median."
    - "Explain why two datasets can have the same mean and very different SD/distribution shape."
    - "Explain why an outlier must be investigated before deletion."
    - "Explain why a bar chart of group means can hide individual-level overlap or skew."
    - "Explain step by step why repeated random samples from one population do not produce identical sample means."
    - "Explain why increasing n can reduce SE while leaving the underlying individual SD similar."
    - "Explain why four times the sample size approximately halves SE(mean) when SD is comparable."
  evidence_critique:
    - "Using the NIST EDA source, explain why graphical inspection can reveal structure that a single center/spread summary misses."
    - "Using Altman & Bland, identify whether a reported number is intended to describe individual variability or uncertainty/precision of a mean, and state whether SD or SE is appropriate."
    - "Using the canonical lesson, audit a truncated-axis graph and state exactly what visual impression changes versus what numerical difference remains unchanged."
    - "Using ICH E9/E9(R1) only as a boundary source, explain why a perfectly calculated mean/SD does not by itself define the treatment effect or causal estimand a study is trying to answer."
  integration:
    - "For an unfamiliar dataset description, output: variable type → distribution features to inspect → center → dispersion → visualization → possible outlier handling → bounded descriptive conclusion."
    - "Compare a symmetric dataset and a strongly right-skewed dataset with the same sample size; choose summaries and justify differences."
    - "Given two samples from the same hypothetical population, explain why their means/SDs can differ without invoking bias automatically."
    - "Given identical SD=12 in n=25 and n=100, calculate the simple mean SE for each and explain which object changed and which did not."
    - "Predict what may happen to mean stability, SE, SD and range when sample size rises substantially while the data-generating distribution remains the same."
    - "Rewrite a claim that says 'the smaller SE group has less individual variability' into a correct statement."
    - "Rewrite a claim that says 'the scatterplot slopes upward, therefore nutrition strategy X causes performance improvement' into a bounded descriptive statement."

notebooklm_tasks:
  - "Act as a Socratic examiner. Present one dataset/graph scenario at a time and wait for the learner's classification and descriptive plan before grading."
  - "For every dataset scenario require exactly: 'Variable type:', 'Distribution features:', 'Center:', 'Dispersion:', 'Visualization:', 'Outlier/anomaly plan:', 'Bounded conclusion:'."
  - "Generate paired datasets with the same mean but different spread/shape and require the learner to identify why the mean alone is inadequate."
  - "Generate paired datasets with the same median/IQR but different tails or multimodality and require the learner to identify what a graph adds."
  - "Create outlier scenarios that alternate between data-entry error, instrument failure and plausible rare biological observation; never allow automatic deletion without a reason."
  - "Generate visual-audit tasks involving truncated axes, aggregated bars hiding distributions, incompatible group scales, selective time windows and misleading bin choices."
  - "Alternate histogram versus bar-chart decisions so the learner must classify the variable rather than recognize a visual keyword."
  - "Generate population/sample/parameter/statistic traps where the same word 'mean' refers once to a population parameter and once to a sample statistic."
  - "Generate repeated-sampling thought experiments and ask separately for the sample distribution and the sampling distribution of the mean."
  - "Generate SD-versus-SE traps where a paper reports mean ± SE and the learner must explain why this is not the spread of individual observations."
  - "Generate n-change scenarios including n×2, n×4 and n×9 with the same SD and ask the learner to predict the SE ratio before calculating."
  - "Ask what larger n does NOT guarantee: lower individual SD, absence of systematic bias, representativeness, causality or practical importance."
  - "Use ICH E9/E9(R1) only to reinforce question/variable/analysis alignment and the boundary between descriptive summaries and the target effect; do not teach advanced estimand or sensitivity-analysis machinery here."
  - "Never introduce p-value thresholds, CI interpretation, standardized effect sizes, formal power calculations or multiplicity as F0.4 answers."
  - "For every explanation, cite only the approved corpus and say when a conclusion needs F0.5/F0.6 or causal-design information rather than improvising it."

```

## Evidence-critique task

Use the canonical F0.4 lesson, NIST EDA source and Altman & Bland note to appraise this synthetic report:

> A sports-science report shows only one bar per group with mean ± SE. Group A has mean 50 and SE 1; Group B has mean 54 and SE 1. The y-axis begins at 48. The authors write: “Group B participants were much less variable and the intervention clearly produced a large improvement.” No individual points, SDs, sample sizes or distribution plots are shown.

The appraisal must:

1. identify what can be read directly from the plotted group means;
2. explain why SE=1 does **not** show that individual participants have SD=1;
3. state which missing information prevents reconstruction of the individual spread;
4. explain how the truncated y-axis can amplify the visual impression without changing the numerical difference of 4 units;
5. state what a dot/strip plot, histogram or other distribution-revealing plot could add;
6. explain why 'much less variable' is unsupported from identical SE alone when n and SD are not reported;
7. explain why 'large improvement' requires an effect/practical-importance framework beyond F0.4;
8. explain why 'produced' is a causal verb whose validity depends on design/bias information from F0.2/F0.3;
9. finish with a bounded descriptive conclusion that uses only the information given.

**Scoring principle:** correct object identification and inferential restraint matter more than advanced terminology.

## Corpus exclusions

Do **not** add these to the initial NotebookLM corpus:

- `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/ENTRY_DIAGNOSTIC.md` — must remain an uncontaminated prerequisite instrument until the learner responds;
- `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/EXERCISES.md` — independent unit assessment;
- `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/ANSWER_KEY.md` — contains both diagnostic and exercise answers; exclusion prevents answer leakage;
- `foundations/F0-scientific-literacy/F0.4-descriptive-statistics/QA_REPORT.md` — production metadata, not study evidence;
- full `SOURCE_INDEX.md` — registry metadata would add retrieval noise;
- ASA p-value statements — F0.5/F0.6, not F0.4;
- sample-size/power planning sources such as F0-S13 — formal power belongs to F0.6;
- full Cochrane effect-measure/meta-analysis chapters — F0.5/F0.7;
- risk-of-bias/causal-inference sources except knowledge already embedded in the canonical lesson's boundary reminders — F0.3 is a prerequisite conceptually but not part of this first-pass descriptive corpus.

### Diagnostic integrity rule

If the learner has **not yet completed** `ENTRY_DIAGNOSTIC.md`, the correct study order is:

1. complete the diagnostic independently first;
2. submit it for scoring/routing;
3. perform any required P1/P2-QB repair;
4. only then begin the NotebookLM F0.4 study sequence for learner-validation purposes.

Creating or reading this manifest does not itself change the diagnostic from `UNOBSERVED`.

## Version and access integrity — verified 2026-09-09

- The canonical F0.4 lesson exists on `main` and is `APPROVED`.
- NIST's current public page for *NIST/SEMATECH e-Handbook of Statistical Methods; Chapter 1: Exploratory Data Analysis* remains available. The page identifies Heckert & Filliben, the 2003 chapter, and an NIST page update of 12 October 2021. The legacy framed handbook URL remains accessible but can be awkward for modern ingestion, so the NIST publication page is the preferred first-pass NotebookLM URL.
- Altman & Bland's BMJ article remains available with DOI `10.1136/bmj.331.7521.903` and continues to state the SD/SE distinction used in F0.4.
- EMA's current ICH E9 page continues to list ICH E9 Step 5 and ICH E9(R1) Step 5 as current adopted versions.
- No source version change found on 2026-09-09 requires modification of the approved F0.4 lesson.

## Copyright/public-repository rule

The public GitHub repository stores only project-authored Markdown, citations and links. Do not commit third-party PDFs or copied chapters unless redistribution permission is explicit. NotebookLM may ingest official public webpages or files obtained lawfully by the learner without republishing them into this repository.

## Completion criterion

The first-pass F0.4 NotebookLM package is correctly configured when:

- exactly four approved sources are loaded;
- the entry diagnostic, exercises and answer key are absent;
- the learner classifies variables before choosing summaries;
- distribution shape is inspected before mean/median or SD/IQR are selected;
- outliers are investigated rather than automatically deleted;
- visualizations are audited rather than treated as decoration;
- population/sample and parameter/statistic are separated;
- sample distribution and sampling distribution are separated;
- SD and SE are never treated as synonyms;
- `SE(mean) ≈ SD/√n` is used only at the simple F0.4 level;
- larger n is not confused with smaller individual variability or removal of bias;
- CI/p-value/effect-size/power/multiplicity content is not pulled forward;
- independent assessment occurs outside NotebookLM;
- no learner or diagnostic state is changed without observed performance.
