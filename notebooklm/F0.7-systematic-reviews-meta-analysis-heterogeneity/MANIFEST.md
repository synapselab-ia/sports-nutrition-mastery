# F0.7 — NotebookLM Manifest

**Package state:** `READY_FOR_STUDY`
**Manifest version:** `1`
**Built/verified:** `2026-09-09`
**Learner state affected:** none
**F0.4 quantitative diagnostic affected:** none; remains `UNOBSERVED`

This manifest defines the approved first-pass NotebookLM corpus for `F0.7 — Systematic reviews, meta-analyses and heterogeneity`. GitHub remains canonical; NotebookLM is a controlled study layer.

The corpus is intentionally limited to **five sources**. The required review-audit sequence is:

`Review question → Eligibility → Search/selection → Extraction/unit structure → Effect compatibility → Study estimates/precision → Weight/model → Clinical/methodological heterogeneity → Statistical heterogeneity → Sensitivity/subgroup/meta-regression prespecification → Missing-evidence/small-study signals → Pooling/conclusion defensibility`

F0.7 must preserve F0.5 magnitude/CI/effect-measure reasoning and F0.6 prespecification/multiplicity reasoning. It must not convert a pooled estimate into automatic truth, I² into a quality score, random effects into a heterogeneity cure, funnel asymmetry into a publication-bias diagnosis, or PRISMA completeness into low risk of bias/high certainty. Formal RoB/GRADE/applicability machinery remains F0.8.

```yaml
module_id: "F0.7"
module_title: "Systematic reviews, meta-analyses and heterogeneity"
version: 1
learning_objectives:
  - "Distinguish a systematic review as an explicit evidence-identification/synthesis process from meta-analysis as an optional statistical combination of study estimates."
  - "Reconstruct the review workflow from protocol/question through eligibility, search, screening, extraction, appraisal, effect measure, synthesis, heterogeneity, missing evidence and interpretation."
  - "Distinguish a study from one or more reports of that study and avoid counting duplicate reports as independent evidence."
  - "Require compatibility of construct, target contrast, effect measure/scale, timepoint and unit-of-analysis structure before numerical pooling."
  - "Preserve F0.5 distinctions among MD, SMD, RD, RR and OR and use log-scale reasoning for ratio measures when relevant."
  - "Explain a pooled estimate as a weighted combination of study-level effect estimates rather than an unweighted average of people."
  - "Use inverse-variance weighting intuition and explain why greater statistical weight reflects precision rather than methodological quality or certainty."
  - "Distinguish fixed-effect/common-effect and random-effects target quantities and assumptions without treating either as universally superior."
  - "Reject the claim that random-effects modelling solves, removes or explains heterogeneity."
  - "Distinguish uncertainty in the pooled mean effect from between-study variation and prediction-interval intuition."
  - "Identify forest-plot study estimates, confidence intervals, weights, null line, effect scale, pooled diamond and heterogeneity statistics."
  - "Interpret a forest plot using F0.5 magnitude/CI reasoning before discussing model, heterogeneity or pooling."
  - "Distinguish clinical diversity, methodological diversity and statistical heterogeneity."
  - "Interpret I2 cautiously as a model-dependent inconsistency statistic, not a percentage of bad studies, quality score, proof of sameness or automatic pooling ban."
  - "Make a defensible pool/no-pool decision from the scientific question and compatibility rather than treating meta-analysis as obligatory."
  - "Use sensitivity analyses as robustness checks rather than result-shopping."
  - "Apply F0.6 prespecification, multiplicity and direct-interaction safeguards to subgroup analyses and meta-regression."
  - "Explain why post hoc subgroup/meta-regression associations do not prove the cause of heterogeneity."
  - "Distinguish small-study effects from publication/non-reporting bias and explain why funnel-plot asymmetry is non-diagnostic."
  - "Explain why apparent funnel symmetry, especially with few studies, does not prove absence of missing evidence."
  - "Use PRISMA 2020 to audit reporting transparency while rejecting PRISMA-complete = low risk of bias/high quality/high certainty."
  - "Audit an unfamiliar heterogeneous evidence synthesis using all twelve F0.7 fields."
  - "Defer formal risk-of-bias tools, GRADE certainty and applicability/transportability judgments to F0.8."

sources:
  - source_id: "F0-R07"
    priority: "CORE"
    citation: "Sports Nutrition Mastery. F0.7 — Revisões sistemáticas, meta-análises e heterogeneidade. Canonical project lesson, version current at manifest v1."
    url_or_doi: "https://raw.githubusercontent.com/synapselab-ia/sports-nutrition-mastery/main/foundations/F0-scientific-literacy/F0.7-systematic-reviews-meta-analysis-heterogeneity/LESSON.md"
    why_included: "Primary instructional spine defining the exact project vocabulary, F0.5/F0.6 integration, worked heterogeneous synthesis, critical fails, twelve-field audit sequence and F0.8 boundary."
    limitation: "Project-authored teaching material, not an independent methodological authority. Material claims remain traceable to the external sources below."

  - source_id: "F0-S04"
    priority: "CORE"
    citation: "Deeks JJ, Higgins JPT, Altman DG, McKenzie JE, Veroniki AA, editors. Chapter 10: Analysing data and undertaking meta-analyses. In: Cochrane Handbook for Systematic Reviews of Interventions, version 6.5. Cochrane; 2024. Chapter last updated November 2024."
    url_or_doi: "https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-10"
    why_included: "Primary external methods anchor for meaningful pooling, inverse-variance weighting, fixed-effect/random-effects models, clinical/methodological/statistical heterogeneity, I2, tau2, prediction intervals, sensitivity analyses, subgroup/meta-regression cautions and forest-plot synthesis reasoning."
    limitation: "Technically broad methods chapter. F0.7 uses conceptual/applied portions only and does not require advanced estimator derivations, network meta-analysis or exhaustive model-selection algorithms."

  - source_id: "F0-S06"
    priority: "SUPPORT"
    citation: "Higgins JPT, Li T, Deeks JJ, editors. Chapter 6: Choosing effect measures and computing estimates of effect. In: Cochrane Handbook for Systematic Reviews of Interventions, version 6.5. Cochrane; 2024. Chapter last updated August 2023."
    url_or_doi: "https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-06"
    why_included: "Compatibility anchor for outcome data types, MD/SMD/RD/RR/OR scale logic, unit-of-analysis structure, conversion requirements and logarithmic handling of ratio measures before pooling."
    limitation: "Broader than F0.7 and includes technical extraction/computation details. It does not by itself determine whether a scientific pooling question is meaningful."

  - source_id: "F0-S05"
    priority: "SUPPORT"
    citation: "Page MJ, Higgins JPT, Sterne JAC. Chapter 13: Assessing risk of bias due to missing evidence in a meta-analysis. In: Cochrane Handbook for Systematic Reviews of Interventions, version 6.5. Cochrane; 2024. Chapter last updated August 2024."
    url_or_doi: "https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-13"
    why_included: "Focused support for missing-evidence/non-reporting reasoning, small-study effects, funnel-plot construction/limitations, alternative explanations for asymmetry and the warning that funnel asymmetry is not diagnostic of publication bias."
    limitation: "Chapter extends into formal missing-evidence risk-of-bias assessment and ROB-ME. F0.7 uses only introductory signals/limitations; formal ROB-ME judgments remain F0.8."

  - source_id: "F0-S03"
    priority: "CONTRAST"
    citation: "Page MJ, McKenzie JE, Bossuyt PM, et al. The PRISMA 2020 statement: an updated guideline for reporting systematic reviews. BMJ. 2021;372:n71. doi:10.1136/bmj.n71."
    url_or_doi: "https://www.prisma-statement.org/prisma-2020"
    why_included: "Contrast source for transparent reporting of review objectives, eligibility, information sources/search, selection, synthesis, heterogeneity investigations, sensitivity analyses, registration/protocol and flow. Its role is to train the distinction between visibility of methods and methodological validity."
    limitation: "Reporting guideline, not a study-level/review-level risk-of-bias tool, quality score or certainty framework. Checklist completion must not be converted into high-quality/high-certainty evidence."

claims_to_master:
  - "A systematic review and a meta-analysis are different objects: systematic review is a structured evidence process; meta-analysis is an optional numerical synthesis."
  - "A legitimate systematic review may not pool when numerical combination would not answer a scientifically coherent question."
  - "The review workflow begins before the forest plot: protocol/question, eligibility, search, screening, extraction and result selection determine the evidence universe that reaches the synthesis."
  - "One study can generate multiple reports; duplicate reports are not independent studies."
  - "Numerical pooling requires defensible compatibility of construct, target contrast, outcome direction, effect scale, timepoint and unit-of-analysis structure."
  - "Same sign or direction is not enough to pool MD, SMD, RR, OR or other incompatible quantities directly."
  - "Inverse-variance weight is approximately proportional to 1/SE^2 in the generic framework; it is a precision weight, not a quality/certainty score."
  - "A fixed-effect/common-effect synthesis and a random-effects synthesis target different model-dependent quantities; model choice is not a simple contest won by one universally superior method."
  - "Random-effects modelling allows different related effects but does not remove, explain or repair heterogeneity or bias."
  - "A random-effects pooled CI concerns uncertainty around the average effect; it does not describe the full spread of underlying effects."
  - "Prediction-interval intuition addresses between-study effect variation and is not interchangeable with the pooled-mean confidence interval."
  - "Clinical diversity concerns participants/interventions/outcomes/context; methodological diversity concerns design/measurement/analysis/bias; statistical heterogeneity concerns variability in observed effects beyond sampling error under the model."
  - "I2 is an inconsistency statistic whose importance depends on effect pattern, number/precision of studies, uncertainty and clinical/methodological context."
  - "Low I2 does not prove studies are clinically or methodologically identical; high I2 does not automatically invalidate meta-analysis."
  - "Sensitivity analyses should test robustness to defensible methodological decisions, not search for a preferred result."
  - "Subgroup and meta-regression findings require direct comparison/interaction reasoning and F0.6 multiplicity/prespecification safeguards."
  - "A post hoc study-level moderator association does not establish the causal source of heterogeneity."
  - "Small-study effects have multiple possible causes, including non-reporting bias, study bias, clinical differences, effect-measure artefacts and chance."
  - "Funnel-plot asymmetry is not diagnostic of publication/non-reporting bias; apparent symmetry does not prove that evidence is complete."
  - "PRISMA 2020 improves reporting transparency and auditability; it is not a low-risk/high-quality/high-certainty certificate."
  - "A pooled estimate remains subject to the validity and applicability of the underlying studies; averaging does not erase systematic bias."
  - "The final synthesis conclusion must preserve magnitude, confidence intervals, practical context, heterogeneity, model assumptions, prespecification and missing-evidence uncertainty."

controversies_or_limits:
  - "Effect compatibility is a scientific judgment, not a mechanical same-sign or same-p-value rule."
  - "SMD can harmonize different instruments for a sufficiently similar construct but cannot make genuinely different constructs equivalent."
  - "Inverse-variance methods are not universally optimal for every sparse-data situation; F0.7 uses them for core weighting intuition, not as a universal software recipe."
  - "Cochrane describes rough I2 interpretation ranges but explicitly warns that thresholds can mislead; F0.7 therefore forbids threshold-only conclusions."
  - "Fixed-effect and random-effects models can produce similar estimates when heterogeneity is negligible, but their interpretation and assumptions still differ."
  - "Random-effects estimates with few studies can be unstable because between-study variance is difficult to estimate."
  - "Prediction intervals depend on model/distribution assumptions and can behave poorly with few studies; F0.7 teaches only the conceptual distinction from a pooled CI."
  - "Subgroup/meta-regression analyses can be underpowered and confounded at the study level; multiple candidate moderators increase false-story risk."
  - "Funnel-plot tests often have low power and are usually considered only when enough studies are available; even then, alternative explanations remain."
  - "PRISMA 2020 is current reporting guidance, not evidence that the review question, search, analysis or underlying studies are valid."
  - "Synthetic exercise/nutrition examples in the canonical lesson are methodological exercises, not evidence about intervention efficacy."
  - "Formal RoB 2/ROBINS-I/ROB-ME/GRADE certainty and target-context applicability remain F0.8."

active_recall:
  basic:
    - "Define systematic review and meta-analysis and explain why one does not imply the other."
    - "State the systematic-review workflow from protocol/question through interpretation."
    - "Distinguish study from report."
    - "Define inverse-variance weight, fixed-effect synthesis, random-effects synthesis, heterogeneity, I2 and small-study effects."
    - "State the null values for difference and ratio effect measures before reading a forest plot."
    - "State PRISMA's purpose and one thing PRISMA completion cannot establish."
  mechanism:
    - "Explain why smaller SE produces greater inverse-variance weight without implying higher study quality."
    - "Explain why random effects gives relatively more weight to smaller studies when between-study variance is present."
    - "Explain why a narrow pooled CI can coexist with wide between-study variation."
    - "Explain how clinical or methodological diversity can generate statistical heterogeneity."
    - "Explain why a low I2 can occur without clinical/methodological sameness and why a high I2 does not automatically forbid pooling."
    - "Explain why funnel asymmetry has multiple possible causes."
  evidence_critique:
    - "Repair 'the pooled estimate is more true than every individual study'."
    - "Repair 'random effects solves heterogeneity'."
    - "Repair 'weight is study quality'."
    - "Repair 'I2=0 proves all studies are equivalent'."
    - "Repair 'I2=87% means the meta-analysis is invalid'."
    - "Repair 'the funnel plot is symmetric, so there is no publication bias'."
    - "Repair 'PRISMA-complete means low risk of bias/high certainty'."
    - "Repair 'significant subgroup A and nonsignificant subgroup B proves effect modification'."
  integration:
    - "Given multiple studies, decide which estimates are compatible for pooling and justify exclusions/conversions before calculating anything."
    - "Given study estimates and SEs, calculate relative inverse-variance weights at P1 level and state what the weights do not measure."
    - "Interpret fixed-effect and random-effects pooled outputs as different model-dependent summaries rather than competing truth scores."
    - "Read a heterogeneous forest plot using F0.5 estimate/CI reasoning plus compatibility, weight/model, heterogeneity and pooling-defensibility."
    - "Generate at least two plausible clinical/methodological explanations for statistical heterogeneity before accepting a subgroup story."
    - "Audit whether sensitivity/subgroup/meta-regression analyses were prespecified and multiplicity-aware."
    - "Complete all twelve F0.7 audit fields for the integrated synthetic review before writing a conclusion."

notebooklm_tasks:
  - "Act as a Socratic examiner. Never begin with the pooled diamond; first require review question, eligibility and which studies/results entered the synthesis."
  - "Generate review-flow scenarios in which duplicate reports, selective timepoints or changed eligibility criteria alter the apparent evidence body."
  - "Generate mixed MD/SMD/RR/OR result tables and require compatibility decisions before allowing pooling."
  - "Generate inverse-variance exercises using supplied SE values and require the learner to state 'weight is precision, not quality'."
  - "Generate paired fixed-effect/random-effects summaries and ask what quantity each model targets and which assumptions are being made."
  - "Generate cases with narrow pooled-mean CIs but substantial between-study variation and require prediction-interval reasoning at conceptual level."
  - "Generate forest plots with difference and ratio measures; require null identification, study-level magnitude/CI interpretation, weights, pooled estimate and heterogeneity."
  - "Generate low-I2/high-clinical-diversity and high-I2-but-scientifically-coherent cases to block threshold worship."
  - "Generate cases where no pooling is the defensible synthesis decision and require a narrative/tabular alternative."
  - "Generate sensitivity-analysis plans and distinguish robustness checks from result-shopping."
  - "Generate subgroup/meta-regression stories with multiple candidate moderators and require direct interaction reasoning, prespecification and multiplicity checks."
  - "Generate funnel-plot scenarios and require at least three possible explanations for asymmetry before discussing missing evidence."
  - "Use PRISMA as a reporting-audit source and reject any attempt to convert checklist completeness into low risk of bias/high certainty."
  - "Use the integrated synthetic review exactly as a twelve-field audit exercise before independent assessment."
  - "Cite only this approved five-source corpus and label any formal RoB/GRADE/applicability claim as F0.8/outside this notebook."
```

## Integrated evidence-synthesis audit

Use only the approved F0.7 corpus to audit this synthetic review.

Review question: `Intervention X versus control` for a synthetic performance score where higher is better.

Protocol before searching:

- trained/recreational adults;
- randomized parallel trials;
- primary outcome at 8–12 weeks;
- MD when the same scale is used;
- random-effects planned because clinical diversity is expected;
- subgroup trained versus recreational prespecified;
- sensitivity analysis excluding high attrition prespecified.

Search/reporting information:

- four databases plus a trial registry;
- no language restriction;
- search date reported.

Five compatible studies:

| Study | Population/context | MD | 95% CI | SE |
|---|---|---:|---:|---:|
| A | recreational; shorter duration | +0.2 | −0.5 to +0.9 | 0.35 |
| B | recreational | +0.5 | −0.3 to +1.3 | 0.40 |
| C | trained | +1.1 | +0.5 to +1.7 | 0.30 |
| D | elite; different measurement setting | +2.4 | +1.5 to +3.3 | 0.45 |
| E | elite; different measurement setting | +3.0 | +2.0 to +4.0 | 0.50 |

Software outputs:

- random-effects pooled MD `+1.4 [0.4, +2.4]`;
- `I² = 87%`;
- fixed-effect pooled MD `+1.18`.

Study F uses a different questionnaire/construct and reports `SMD = +0.60 [0.10, +1.10]`.

Post hoc, authors test duration, elite status, indoor/outdoor, baseline score and several leave-one-out variants. They highlight elite status with interaction `p=0.04`, although elite status is collinear with measurement setting and was not prespecified.

With only five compatible studies, a funnel plot appears symmetric and authors conclude “no publication bias”. The review also reports complete PRISMA adherence and calls the evidence “high certainty”.

Required output — all twelve fields:

1. `Review question` — define the target evidence question;
2. `Eligibility` — state what evidence universe the protocol intended to include;
3. `Search/selection` — identify what is visible and what still cannot be inferred merely from reporting;
4. `Extraction/unit structure` — state what must be checked before accepting study estimates as independent/comparable;
5. `Effect compatibility` — explain why A–E can enter the MD synthesis and why Study F cannot be directly added as `0.60` to that MD pool;
6. `Study estimates/precision` — interpret the individual MDs/CIs using F0.5 reasoning;
7. `Weight/model` — explain inverse-variance intuition and what the planned random-effects average represents;
8. `Clinical/methodological heterogeneity` — give at least two plausible explanations for the different effects before accepting the elite-status story;
9. `Statistical heterogeneity` — interpret `I²=87%` without automatic invalidation or threshold worship;
10. `Sensitivity/subgroup/meta-regression prespecification` — distinguish the prespecified subgroup/sensitivity analysis from post hoc moderator/result selection and apply F0.6 multiplicity safeguards;
11. `Missing-evidence/small-study signals` — explain why five-study funnel symmetry cannot establish absence of publication/non-reporting bias;
12. `Pooling/conclusion defensibility` — state whether A–E can be summarized by a random-effects average, what the pooled mean does and does not represent, whether Study F should remain separate unless a defensible harmonization is established, and why PRISMA completeness does not establish high certainty.

## Corpus exclusions

Do **not** add to the initial NotebookLM corpus:

- `foundations/F0-scientific-literacy/F0.7-systematic-reviews-meta-analysis-heterogeneity/EXERCISES.md` — independent assessment;
- `foundations/F0-scientific-literacy/F0.7-systematic-reviews-meta-analysis-heterogeneity/ANSWER_KEY.md` — answer leakage;
- F0.7 production `QA_REPORT.md` — production metadata, not study evidence;
- F0.4 `ENTRY_DIAGNOSTIC.md` — prerequisite diagnostic remains uncontaminated and `UNOBSERVED`;
- full `SOURCE_INDEX.md` — retrieval noise;
- formal RoB 2, ROBINS-I and ROB-ME tools — F0.8;
- GRADE certainty guidance — F0.8;
- applicability/transportability guidance — F0.8;
- advanced network meta-analysis/IPD/meta-analysis estimator catalogs — outside F0.7 core;
- substantive sports-nutrition intervention papers — this package teaches evidence-synthesis methodology, not efficacy of a nutrition intervention.

## Version/access integrity — verified 2026-09-09

- Canonical F0.7 lesson exists on `main` with production state `APPROVED`.
- Cochrane Chapter 10 official page remains `Analysing data and undertaking meta-analyses`; its citation states Handbook version 6.5 and chapter last updated November 2024. Current content continues to cover inverse-variance weighting, meaningful pooling, fixed/random-effects interpretation, heterogeneity, I2, prediction intervals, subgroup/meta-regression and sensitivity analysis.
- Cochrane Chapter 6 official page remains `Choosing effect measures and computing estimates of effect`; its citation states Handbook version 6.5 and chapter last updated August 2023. It continues to distinguish data/effect types, unit-of-analysis issues and log-scale handling of ratio measures.
- Cochrane Chapter 13 official page remains `Assessing risk of bias due to missing evidence in a meta-analysis`; its citation states Handbook version 6.5 and chapter last updated August 2024. It continues to warn that funnel asymmetry has multiple explanations and is not diagnostic of non-reporting bias.
- PRISMA's official site continues to identify PRISMA 2020 as the main reporting guideline and exposes the statement, 27-item checklist, expanded checklist, abstract checklist and flow diagrams.
- PRISMA is used here strictly as reporting guidance; formal risk-of-bias/certainty conclusions remain outside the package.
- No third-party full text is committed to GitHub by this package; it stores only project-authored Markdown, citations and links.

## Package authority

If NotebookLM produces a claim not supported by these five approved sources, treat it as an unverified lead. Do not write it back to the canonical repository without independent verification under the project research protocol.
