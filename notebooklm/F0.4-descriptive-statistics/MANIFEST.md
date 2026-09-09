# F0.4 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-09`
**Learner state affected:** none
**Quantitative diagnostic state affected:** none (`UNOBSERVED` remains canonical until real responses exist)

This manifest defines the approved, deliberately small NotebookLM corpus for `F0.4 — Descriptive statistics, distributions and sampling variation`. GitHub remains canonical; NotebookLM is a source-controlled study layer.

The first-pass corpus is intentionally limited to **four sources**. The required reasoning sequence is:

`variable type → measurement scale/context → distribution shape → center + dispersion → outliers/anomalies → visualization → population/sample + parameter/statistic → sample distribution vs sampling distribution → SD vs SE → sample-size consequence → bounded conclusion`

F0.4 stops before full confidence-interval, p-value and effect-size interpretation (F0.5) and before formal power, Type I/II error and multiplicity (F0.6).

```yaml
module_id: "F0.4"
module_title: "Descriptive statistics, distributions and sampling variation"
version: 1
learning_objectives:
  - "Classify variables as categorical nominal/ordinal or numerical discrete/continuous from what the values represent rather than file encoding alone."
  - "Use nominal/ordinal/interval/ratio scale language as a reasoning aid without treating the taxonomy as an automatic analysis-selection machine."
  - "Inspect distribution shape before choosing a summary and describe symmetry, skew, multimodality, bounds and potential outliers."
  - "Choose and justify center using mean, median or mode and dispersion using range, variance/SD, IQR or quantiles."
  - "Explain why equal means can hide different distributions and why graphs are analytical objects rather than decoration."
  - "Treat outliers as observations requiring verification/context rather than automatic deletion."
  - "Choose and audit dot/strip plots, histograms, boxplots, bar charts and scatterplots."
  - "Distinguish population/sample and parameter/statistic."
  - "Explain sampling variability and distinguish sample distribution from sampling distribution."
  - "Distinguish SD as individual-level spread from SE as sampling variability/precision of an estimate."
  - "Use SE(mean) ≈ SD/√n only in the simple independent-observation setting taught in F0.4."
  - "Predict what larger n changes and does not automatically change when underlying individual variability remains similar."
  - "Treat transformations as scale changes, not tools for erasing bias or forcing acceptable results."
  - "Keep descriptive evidence separate from causal, significance and practical-effect claims that require later modules."

sources:
  - source_id: "F0-R04"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.4 — Estatística descritiva, distribuições e variação amostral. Canonical project lesson, version current at manifest v1."
    url_or_doi: "https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.4-descriptive-statistics/LESSON.md"
    why_included: "Primary instructional spine defining the exact vocabulary, formulas, worked examples, error traps, sports/exercise-flavored synthetic transfer and curricular boundaries."
    limitation: "Project-authored teaching material, not an independent external authority; methodological claims remain traceable to the registered external sources."

  - source_id: "F0-S12"
    priority: "CORE"
    citation: "NIST/SEMATECH. e-Handbook of Statistical Methods. Chapter 1: Exploratory Data Analysis. National Institute of Standards and Technology."
    url_or_doi: "https://www.itl.nist.gov/div898/handbook/eda/eda.htm"
    why_included: "Institutional EDA anchor for graphical inspection, distribution structure, anomalies/outliers and the principle that a dataset should be explored rather than reduced immediately to one summary statistic."
    limitation: "General/engineering context and much broader than F0.4. Use the EDA/descriptive portions only; do not import later testing/modeling procedures. The modern NIST publication record remains useful for bibliographic verification, but this direct chapter endpoint is preferred for NotebookLM ingestion because it exposes the actual chapter content."

  - source_id: "F0-S27"
    priority: "SUPPORT"
    citation: "Altman DG, Bland JM. Standard deviations and standard errors. BMJ. 2005;331(7521):903. doi:10.1136/bmj.331.7521.903."
    url_or_doi: "https://www.bmj.com/content/331/7521/903"
    why_included: "Focused support for the major F0.4 misconception: SD describes variability of observations while SE describes sampling variability/precision of an estimate; also supports the simple mean relation SE = SD/√n."
    limitation: "Concise 2005 educational note, not a comprehensive statistics text. Confidence-interval discussion belongs to F0.5."

  - source_id: "F0-S14"
    priority: "CONTRAST"
    citation: "International Council for Harmonisation. ICH E9: Statistical Principles for Clinical Trials; ICH E9(R1) Addendum on Estimands and Sensitivity Analysis in Clinical Trials. Current Step 5 versions accessed through EMA."
    url_or_doi: "https://www.ema.europa.eu/en/ich-e9-statistical-principles-clinical-trials-scientific-guideline"
    why_included: "Boundary/contrast source showing that descriptive summaries sit within a larger objective → variable/outcome → target quantity/estimand → analysis chain and cannot independently answer a treatment-effect question."
    limitation: "Regulatory clinical-trial guidance substantially more technical than F0.4. Do not study regulatory detail, sensitivity-analysis machinery or formal estimand implementation here."

claims_to_master:
  - "Variable meaning comes before statistical procedure; numeric storage does not make a categorical code quantitative."
  - "Distribution shape, bounds, tails, clusters and extreme observations can make one-number summaries misleading."
  - "Mean is magnitude-sensitive and median is more resistant to extremes; neither is universally superior."
  - "Range and IQR describe different parts of spread; variance is in squared units and SD returns to the original unit."
  - "Right skew is defined by tail shape, not by an absolute rule that mean must exceed median."
  - "Outlier handling follows detect → verify origin → justify treatment → document, not automatic deletion."
  - "Histogram and bar chart answer different data-display problems; scatterplot association is not causality."
  - "Axis truncation is not automatically invalid, but visual magnitude must be read against the numerical scale."
  - "Population/sample and parameter/statistic are different objects."
  - "Different random samples from one population can yield different sample statistics: sampling variability."
  - "Sample distribution contains observed individual values; sampling distribution contains repeated-sample values of a statistic."
  - "SD describes variability among observations; SE describes sampling variability/precision of an estimator."
  - "For the simple sample mean, SE(mean) ≈ SD/√n."
  - "With comparable SD, quadrupling n approximately halves SE(mean); doubling n does not halve it."
  - "Larger n does not automatically reduce individual SD, eliminate systematic bias, guarantee representativeness or prove causality."
  - "Observed range can increase in larger samples because more extreme observations can be encountered."
  - "Transformations change scale/representation and do not repair confounding, selection bias, measurement error or poor design."
  - "Descriptive statistics alone do not establish confidence, significance, effect importance or causal effect."

controversies_or_limits:
  - "Mean/SD versus median/IQR rules are heuristics, not universal laws; choice depends on question, variable meaning, distribution and robustness needs."
  - "Nominal/ordinal/interval/ratio classification is useful but should not be treated as a complete automatic analysis decision tree."
  - "Outlier criteria and boxplot whisker conventions vary; a flagged observation is not automatically erroneous."
  - "Histogram appearance depends on bins; one histogram is not a unique visual truth."
  - "SE = SD/√n is taught only for the simple mean in the basic independent-observation setting; clustered, paired, weighted and model-based estimators require structure-specific standard errors later."
  - "NIST includes later inferential methods that are outside F0.4."
  - "Altman & Bland mention confidence intervals, but CI interpretation belongs to F0.5."
  - "ICH E9/E9(R1) is included only for alignment/scope contrast, not as a descriptive-statistics manual."
  - "Synthetic exercise/nutrition examples are statistical illustrations, not substantive intervention evidence."

active_recall:
  basic:
    - "Classify variables from meaning, then state one suitable and one unsuitable summary."
    - "Define mean, median, mode, range, sample variance, SD, Q1, Q3 and IQR."
    - "State the units of variance and SD for a variable measured in kilograms."
    - "Define population, sample, parameter and statistic."
    - "Define sample distribution and sampling distribution."
    - "Define SD and SE in one sentence each."
  mechanism:
    - "Explain why an extreme value can pull mean more than median."
    - "Explain how two datasets can share a mean but differ in spread/shape."
    - "Explain why outlier detection does not justify automatic deletion."
    - "Explain what a distribution-revealing plot can show that a bar of means hides."
    - "Explain why repeated samples from one population have different sample means."
    - "Explain why larger n can lower SE while individual SD remains similar."
  evidence_critique:
    - "Use NIST EDA to explain why graphical inspection can reveal hidden structure."
    - "Use Altman & Bland to decide whether SD or SE is appropriate for individual variability versus mean precision."
    - "Audit a truncated-axis graph and separate visual amplification from the unchanged numerical difference."
    - "Use ICH E9/E9(R1) only as a boundary source to explain why a descriptive mean difference does not itself define a causal treatment effect."
  integration:
    - "For an unfamiliar dataset output: variable type → distribution features → center → dispersion → visualization → outlier plan → bounded conclusion."
    - "Compare a symmetric and a right-skewed dataset and justify different summaries."
    - "Given identical SD with different n, calculate simple mean SE and identify which object changed."
    - "Predict mean stability, SE, SD, range and bias consequences when n increases while the generating distribution stays the same."
    - "Repair the false claim 'smaller SE means participants are less variable'."
    - "Repair the false claim 'upward scatterplot means nutrition strategy X causes improvement'."

notebooklm_tasks:
  - "Act as a Socratic examiner and present one synthetic dataset/graph scenario at a time. Wait for the learner before grading."
  - "Require variable type and distribution inspection before summary selection."
  - "Generate same-mean/different-shape datasets and same-median/IQR/different-tail datasets."
  - "Alternate real outliers, data-entry errors, sensor failures and unresolved anomalies; never permit automatic deletion without provenance reasoning."
  - "Generate visual audits involving truncated axes, aggregate bars, incompatible scales, selective windows and bin choices."
  - "Generate population/sample and parameter/statistic traps."
  - "Generate repeated-sampling thought experiments separating sample distribution from sampling distribution."
  - "Generate SD-versus-SE reporting traps and simple n-change calculations."
  - "Ask what larger n does not guarantee: lower individual SD, removal of systematic bias, representativeness, causality or practical importance."
  - "Never introduce p-value thresholds, CI interpretation, effect sizes, formal power or multiplicity as F0.4 answers."
  - "Cite only the approved four-source corpus and state when a conclusion requires F0.5/F0.6 or causal-design information."
```

## Evidence-critique task

Appraise this synthetic report using the F0.4 lesson, NIST EDA and Altman/Bland:

> Group A mean 50, SE 1; Group B mean 54, SE 1. Only bars are shown and the y-axis starts at 48. Authors state: “Group B participants were much less variable and the intervention clearly produced a large improvement.” Individual points, SDs, sample sizes and distribution plots are not shown.

Required outputs:

1. what is directly observed from the means;
2. why SE=1 does not mean individual SD=1;
3. what missing information prevents reconstruction of individual spread;
4. how the truncated axis changes visual impression without changing the numerical difference of 4;
5. what a distribution-revealing plot could add;
6. why “much less variable” is unsupported from identical SE alone when n/SD are unknown;
7. why “large improvement” requires F0.5 practical/effect interpretation;
8. why “produced” requires F0.2/F0.3 causal validity;
9. one bounded descriptive conclusion.

## Corpus exclusions

Do **not** add to the initial NotebookLM corpus:

- `ENTRY_DIAGNOSTIC.md` — prerequisite instrument must remain uncontaminated until completed;
- `EXERCISES.md` — independent unit assessment;
- `ANSWER_KEY.md` — contains diagnostic and exercise answers;
- production `QA_REPORT.md` — metadata, not study evidence;
- full `SOURCE_INDEX.md` — retrieval noise;
- ASA p-value materials — F0.5/F0.6;
- `F0-S13` sample-size/power planning — F0.6;
- Cochrane effect-measure/meta-analysis material — later units;
- broad causal/risk-of-bias corpora — prerequisites, not first-pass F0.4 sources.

## Diagnostic integrity rule

If `ENTRY_DIAGNOSTIC.md` is still `UNOBSERVED`, honest learner validation requires:

1. complete the diagnostic independently before F0.4 study;
2. submit it for scoring/routing;
3. perform any observed P1/P2-QB repair;
4. then begin the NotebookLM study sequence.

Creating this package does not itself change the diagnostic state.

## Version/access integrity — verified 2026-09-09

- Canonical F0.4 lesson exists on `main` and is `APPROVED`.
- NIST direct EDA chapter endpoint is accessible and exposes actual chapter content/navigation; NIST's modern publication record independently identifies Heckert & Filliben's Chapter 1 and records the NIST page update date as 12 October 2021.
- Altman & Bland's BMJ article remains available with DOI `10.1136/bmj.331.7521.903`.
- EMA continues to list ICH E9 Step 5 and E9(R1) Step 5 as current adopted versions.
- No source-version change found on 2026-09-09 requires modification of the approved F0.4 lesson.

## Copyright/public-repository rule

The public GitHub repository stores only project-authored Markdown, citations and links. Do not commit third-party PDFs or copied chapters unless redistribution permission is explicit.

## Completion criterion

The package is correctly configured when:

- exactly four approved sources are loaded;
- diagnostic/exercises/answer key are absent;
- variable meaning precedes summary selection;
- distribution is inspected before center/dispersion choice;
- outliers are investigated rather than automatically deleted;
- visualizations are audited;
- population/sample and parameter/statistic are separated;
- sample distribution and sampling distribution are separated;
- SD and SE are never treated as synonyms;
- simple `SE(mean) ≈ SD/√n` reasoning is fluent;
- larger n is not confused with lower individual variability or removal of bias;
- F0.5/F0.6 content is not pulled forward;
- assessment remains independent;
- no learner/diagnostic state changes without observed performance.
